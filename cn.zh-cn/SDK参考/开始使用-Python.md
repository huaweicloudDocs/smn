# 开始使用<a name="ZH-CN_TOPIC_0093269620"></a>

## 使用示例代码发送短信<a name="section1352094510584"></a>

以下给出了发送短信的代码，采用华为云账号密码的方式创建服务实例。

>![](public_sys-resources/icon-note.gif) **说明：**   
>-   存在问题：由于代码中有中文字符，若您直接把代码复制到Windows的文本中，因windows默认中文编码是GBK，执行代码时可能会报编码错误。  
>-   解决办法：  
>    1.  用Windows文本编辑器打开python脚本，选择“文件 \> 另存为”。  
>    2.  在弹出的对话框中，“保存类型”更改为“所有文件\(\*.\*\)”，“编码 ”由默认的“ANSI”改为“UTF-8”，文件名保持不变。  
>    3.  单击保存。  

```
# coding=utf-8
import time
from smnsdkcore.client import SMNClient
from smnsdkrequests.v20171105.SmsPublish import SmsPublish

def demoSendSms(sms_sign_id, endpoint, message):
    request = SmsPublish()
    request.set_endpoint(endpoint)
    request.set_message(message)
    request.set_sign_id(sms_sign_id)
    return client.send(request)

if __name__ == "__main__":
    client = SMNClient(username='YourAccountUserName', domain_name='YourAccountDomainName', password='YourAccountPassword', region_id='YourRegionName')
    #sms_sign_id为您使用的短信签名的签名ID
    sms_sign_id = 'a0f6d2****cd4ff8b70eeecb612511da'
    #phoneNumber为您要发送短信的手机号码
    phoneNumber = '+8618682****29'
    message = '您的验证码是:1234，请查收'

    status, headers, response_body = demoSendSms(sms_sign_id, phoneNumber, message)
    print status, response_body
```

## 使用示例代码通过主题发布消息<a name="section7670737"></a>

以下给出了创建主题、添加订阅的示例代码，添加订阅成功会发送订阅确认消息给终端。

创建Topic，并获取response返回的**topic\_urn**。

```
# coding=utf-8

from smnsdkcore.client import SMNClient
from smnsdkrequests.v20171105.CreateTopic import CreateTopic

def demoCreateTopic(topic_name, display_name):
    request = CreateTopic()
    request.set_topic_name(topic_name)
    request.set_display_name(display_name)
    return client.send(request)

if __name__ == "__main__":
    client = SMNClient(username='YourAccountUserName', domain_name='YourAccountDomainName', password='YourAccountPassword', region_id='YourRegionName')

    status, headers, response_body = demoCreateTopic('python-sdk', 'FromCloud')
    print status, response_body
```

向Topic添加订阅，获取response返回的**subscription\_urn**。代码中**test\_urn**是上述代码返回的**topic\_urn**，**endpoint\_phone**改成具体手机号

```
# coding=utf-8

from smnsdkcore.client import SMNClient
from smnsdkrequests.v20171105.Subscribe import Subscribe

def demoSubscribe(topic_urn, endpoint, remark):
    request = Subscribe()
    request.set_endpoint(endpoint)
    request.set_remark(remark)
    request.set_topic_urn(topic_urn)
    return client.send(request)   

if __name__ == "__main__":
    client = SMNClient(username='YourAccountUserName', domain_name='YourAccountDomainName', password='YourAccountPassword', region_id='YourRegionName')

    test_urn = 'urn:smn:cn-north-1:xxxx:python-sdk'
    endpoint_phone = '+8618682****29'
    endpoint_remark = 'this is pengzl phone'
    status, headers, response_body = demoSubscribe(test_urn, endpoint_phone, endpoint_remark)
    print status, response_body
```

手机终端收到订阅确认短信，点击订阅链接确认订阅后，您可以向主题发布消息。代码中**test\_urn**、**subscription\_urn**分别是上述返回的**topic\_urn**和**subscription\_urn**。

```
# coding=utf-8

from smnsdkcore.client import SMNClient
from smnsdkrequests.v20171105 import Publish
from smnsdkrequests.v20171105.Publish import PublishMessage

def demoPublishMessage(topic_urn, message):
    request = PublishMessage()
    request.set_topic_urn(topic_urn)
    request.set_subject("Subject, only display to email subscription")
    request.set_message(message)
    return client.send(request)

if __name__ == "__main__":
    client = SMNClient(username='YourAccountUserName', domain_name='YourAccountDomainName', password='YourAccountPassword', region_id='YourRegionName')

    test_urn = 'urn:smn:cn-north-1: xxxx:python-sdk'
    subscription_urn = 'urn:smn:cn-north-1: xxxx:python-sdk:xxxx'
    message = '您的验证码是:1234，请查收'

    status, headers, response_body = demoPublishMessage(test_urn, message)
    print status, response_body
```

## 更多示例代码请参考github上的example项目<a name="section49316177283"></a>

[Example项目地址](https://github.com/SimpleMessageNotification/smn-sdk-python/tree/master/smn-sdk-python-example)

