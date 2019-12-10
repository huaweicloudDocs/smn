# 开始使用<a name="ZH-CN_TOPIC_0093269624"></a>

## 使用示例代码发送短信<a name="section1352094510584"></a>

以下给出了发送短信的代码，采用华为云账号密码的方式创建服务实例。如果需要自定义HTTP参数或者使用代理，请参考[HTTP参数设置和使用代理](#section42981531161017)。

```
package main
import (
    "github.com/smn-sdk-go/smn-sdk-go/client"
    "fmt"
)
func main() {
    // init client, you can init client only once
    smnClient, err := client.NewClient(
           "YourAccountUserName",
           "YourAccountDomainName",
           "YourAccountPassword",
           "YourRegionName")
    if err != nil {
           panic(err)
    }
    request := smnClient.NewSmsPublishRequest()
    request.EndPoint = "+86136*****587"
    request.SignId = "6be340e91e524******85837e6709104"
    request.Message = "您的验证码是:1234，请查收"
    response, err := smnClient.SmsPublish(request)
    if err != nil {
           fmt.Println("the request is error ", err)
           return
    }
    if !response.IsSuccess() {
           fmt.Printf("%#v\n", response.ErrorResponse)
           return
    }
    fmt.Printf("%#v\n", response)
}  
```

## 使用示例代码通过主题发布消息<a name="section7670737"></a>

以下给出了创建主题、添加订阅的示例代码，添加订阅成功会发送订阅确认消息给终端。

```
package main
import (
    "github.com/SimpleMessageNotification/smn-sdk-go/smn-sdk-go/client"
    "fmt"
)
func main() {
    // init client
    smnClient, err := client.NewClient(
           "YourAccountUserName",
           "YourAccountDomainName",
           "YourAccountPassword",
           "YourRegionName")
    if err != nil {
           panic(err)
    }
    createTopicReqeust := smnClient.NewCreateTopicRequest()
    createTopicReqeust.Name = "topicName_go"
    createTopicReqeust.DisplayName = " topicDisplayname"
    createTopicResponse, err := smnClient.CreateTopic(createTopicReqeust)
    if err != nil {
           fmt.Println("the request is error ", err)
           return
    }
    if !createTopicResponse.IsSuccess() {
           fmt.Printf("%#v\n", createTopicResponse.ErrorResponse)
           return
    }
    subscribeRequest := smnClient.NewSubscribeRequest()
    subscribeRequest.Endpoint = "+86136*****587"
    subscribeRequest.TopicUrn = createTopicResponse.TopicUrn
    subscribeRequest.Protocol = "sms"
    subscribeRequest.Remark = "subscribe sms"
    response, err := smnClient.Subscribe(subscribeRequest)
    if err != nil {
           fmt.Println("the request is error ", err)
           return
    }
    fmt.Printf("%#v\n", response)
}  
```

终端确认订阅后，您可以向主题发布消息。

```
package main
import (
    "github.com/SimpleMessageNotification/smn-sdk-go/smn-sdk-go/client"
    "fmt"
)
func main() {
    // init client
    smnClient, err := client.NewClient(
           "YourAccountUserName",
           "YourAccountDomainName",
           "YourAccountPassword",
           "YourRegionName")
    if err != nil {
           panic(err)
    }
    request := smnClient.NewPublishMessageRequest()
    request.TopicUrn = "urn:smn:cn-north-1:cffe4fc4c*************586e132:topic1_go"
    request.Message = "test content"
    response, err := smnClient.PublishMessage(request)
    if err != nil {
           fmt.Println("the request is error ", err)
           return
    }
    if !response.IsSuccess() {
           fmt.Printf("%#v\n", response.ErrorResponse)
           return
    }
    fmt.Printf("%#v\n", response)
}     
```

## HTTP参数设置和使用代理<a name="section42981531161017"></a>

以下示例代码向您展示了如何自定义设置HTTP参数和使用代理：

1.  创建ClientConfiguration并设置相应参数。
2.  创建服务实例并设置ClientConfiguration。

```
proxy := func(_ *http.Request) (*url.URL, error) {
     return url.Parse("http://127.0.0.1:8080")
}
transport := &http.Transport{
     Proxy: proxy,
     TLSClientConfig:&tls.Config{InsecureSkipVerify:true}
}
config := commom.NewClientConfig()
config.SetTimeout(20 * time.Second)
config.SetTransport(transport)

// 初始化
smnClient, err := client.NewClientWithConfig(
     "YourAccountUserName",
     "YourAccountDomainName",
     "YourAccountPassword",
     "YourRegionName",
     config)
```

## 更多示例代码请参考github上的example项目<a name="section15191111018346"></a>

[Example项目地址](https://github.com/SimpleMessageNotification/smn-sdk-go/tree/master/smn-sdk-go-example)

