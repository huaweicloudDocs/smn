# JSON格式消息说明<a name="ZH-CN_TOPIC_0047574409"></a>

## JSON格式体说明<a name="section534667717028"></a>

JSON格式主要用来处理用户想对不同的订阅者类型发送不同的消息，目前支持的协议Default、SMS、HTTP、HTTPS、email、FunctionGraph（函数）、Functiongraph（工作流）、Application以及DMS，其中Default是必须的，Email的内容将发给邮件类型的订阅者，其它协议依次如下所示：

```
{
  "default": "Dear Sir or Madam, this is a default message.",
  "email": "Dear Sir or Madam, this is an email message.",
  "http": "{'message':'Dear Sir or Madam, this is an HTTP message.'}",
  "https": "{'message':'Dear Sir or Madam, this is an HTTPS message.'}",
  "sms": "This is an SMS message.",
  "functionstage": "Dear Sir or Madam, this is a functiongraph(function) message.",
  "functiongraph": "Dear Sir or Madam, this is a functiongraph(workflow) message.",
  "dms":"Dear Sir or Madam, this is a DMS message."
    }
```

推荐将Default设置为通用的消息内容，对于特殊的订阅者类型再设置相应消息内容。

以下示例展现由于短信内容长度有限制，将短信设置为特殊的消息，其中HTTP、HTTPS、Email、FunctionGraph（函数）、Functiongraph（工作流）、“Application”以及DMS类型的订阅收到"Dear Sir or Madam, this is a default message."的内容，而SMS类型的订阅者收到“This is an SMS message”。

```
{
  "sms": "This is an SMS message.",
  "default": "Dear Sir or Madam, this is a default message."
 }
```

## JSON格式约束<a name="section9710251165825"></a>

-   满足JSON格式要求。
-   JSON格式中必须有Default协议。
-   整个JSON消息的大小不超过256KB。

## JSON消息计算<a name="section11977745123756"></a>

选择不同的协议，生成的JSON格式消息的大小不同。JSON格式消息的字节数包含消息框中显示的花括号、双引号、空格、回车、协议名称和消息内容累计字节数。具体字节计算方式以输入消息“This is a default message.”为例。

消息：“This is a default message.”，消息本身包含26个字节。

输入消息，选择协议，生成JSON消息时，系统默认生成Default协议的消息。

```
{
  "default": "This is a default message.",
  "protocol1": "This is a default message.",
  "protocol2": "This is a default message.",
  ……
}
```

1个Default协议加上用户选择的协议个数，记为N。

消息体包含的固定字节数：

-   每种协议的消息包含3个空格，共N个协议：3× N = 3N
-   每种协议的消息包含4个双引号，共N个协议： 4 × N = 4N
-   每种协议的消息包含1个冒号，共N个协议：1 × N = N
-   每种协议的消息包含1条消息内容This is a default message.，共N个协议：26 × N = 26N
-   逗号（N - 1）个：1 × （N - 1） = （N - 1）
-   回车（N + 1）个：1 ×（N + 1） = （N + 1）
-   花括号2个：1 × 2 = 2
-   协议名称 default 1个：7 × 1 = 7

选择的协议字节数：

-   协议名称 HTTP 1个：4 × 1 = 4
-   协议名称 HTTPS1个：5 × 1 = 5
-   协议名称 email 1个：5 × 1 = 5
-   协议名称 sms 1个：3 × 1 = 3
-   协议名称 Functionstage 1个：13 × 1 = 13
-   协议名称 Functiongraph 1个：13 × 1 = 13
-   协议名称 DMS 1个：3 × 1 = 3
-   协议名称Application 1个：11×1=11

合计：36N + 9 + 选择的协议字节数

例如，您选择了“HTTP”、“HTTPS”和“email”3个协议，生成的消息如下：

```
{
  "default": "This is a default message.",
  "email": "This is a default message.",
  "http": "This is a default message.",
  "https": "This is a default message."
}
```

加上Default，则N的值为4，生成的JSON消息字节数计算如下：

-   固定字节数：36 × 4 + 9 = 153
-   协议名称 HTTP 1个：4 × 1 = 4
-   协议名称 HTTPS 1个：5 × 1 = 5
-   协议名称 email 1个：5 × 1 = 5

合计：153 + 4 + 5 + 5 = 167

