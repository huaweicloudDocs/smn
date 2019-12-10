# 开始使用<a name="ZH-CN_TOPIC_0093269626"></a>

## 使用示例代码发送短信<a name="section89411748164514"></a>

以下给出了发送短信的代码，采用华为云账号密码的方式创建服务实例。如果需要自定义HTTP参数或者使用代理，请参考[HTTP参数设置和使用代理](#section1635184954510)。

```
using Smn;
using Smn.Request.Sms;
using Smn.Response.Sms;
using System;
namespace Smn.Example
{
    class SmnDemo
    {
        public static void Main(string[] args)
        {
            // 初始化client
            SmnClient smnClient = new SmnClient(
                    "YourAccountUserName",
                    "YourAccountDomainName",
                    "YourAccountPassword",
                    "YourRegionName");
            // 发送请求对象，并设置参数
            SmsPublishRequest request = new SmsPublishRequest
            {
                // 发送手机号码 号码格式 (+)(国家码)(手机号码)
                Endpoint = "+86136*****587",  
                // 短信签名必填,需要在消息通知服务的自助页面申请签名，申请办理时间约2天
                SignId = "6be340e91e5*********37e6709104", 
                Message = "您的验证码是:1234，请查收" 
            };
            try
            {
                // 发送请求并返回响应
                SmsPublishResponse response = smnClient.SendRequest(request);
                string result = response.MessageId;
                Console.WriteLine("{0}", result);
            }
            catch (Exception e)
            {
                // 处理异常
                Console.WriteLine("{0}", e.Message);
            }
        }
    }
}  
```

## 使用示例代码通过主题发布消息<a name="section1397319481450"></a>

以下给出了创建主题、添加订阅的示例代码，添加订阅成功会发送订阅确认消息给终端。

```
using Smn;
using Smn.Request.Subscription;
using Smn.Request.Topic;
using Smn.Response.Subscription;
using Smn.Response.Topic;
using Smn.Util;
using System;
namespace smn_sdk_net_example
{
    class TopicDocDemo
    {
        public static void Main(string[] args)
        {
            // 初始化client
            SmnClient smnClient = new SmnClient(
                    "YourAccountUserName",
                    "YourAccountDomainName",
                    "YourAccountPassword",
                    "YourRegionName");
             // 创建topic请求对象
            CreateTopicRequest createTopicRequest = new CreateTopicRequest
            {
                Name = "create_test_csharp3",
                DisplayName = "topic display name",
            };
            CreateTopicResponse createTopicResponse;
            try
            {
                // 发送请求并返回响应
                createTopicResponse = smnClient.SendRequest(createTopicRequest);
                string result = createTopicResponse.TopicUrn;
            }
            catch (Exception e)
            {
                // 处理异常
                Console.WriteLine("{0}", e.Message);
                Console.ReadLine();
                return;
            }
            // 设置请求对象
            SubscribeRequest subscribeRequest = new SubscribeRequest
            {
                TopicUrn = createTopicResponse.TopicUrn,
                Protocol = ProtocolType.SMS,
                Endpoint = "+86136*****587",
                Remark = "subscribe test"
            };
            try
            {
                // 发送请求并返回响应
                SubscribeResponse subscribeResponse = smnClient.SendRequest(subscribeRequest);
                string result = subscribeResponse.RequestId;
                Console.WriteLine("{0}", result);
                Console.ReadLine();
            }
            catch (Exception e)
            {
                // 处理异常
                Console.WriteLine("{0}", e.Message);
                Console.ReadLine();
            }
        }
    }
}  
```

终端确认订阅后，您可以向主题发布消息。

```
using Smn;
using Smn.Request.Publish;
using Smn.Response.Publish;
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
namespace smn_sdk_net_example
{
    class PublishDocDemo
    {
        public static void Main(string[] args)
        {
            // 初始化client
            SmnClient smnClient = new SmnClient(
                    "YourAccountUserName",
                    "YourAccountDomainName",
                    "YourAccountPassword",
                    "YourRegionName");
            // 设置请求对象
            PublishRequest request = new PublishRequest
            {
                TopicUrn = "urn:smn:cn-north-1:cffe4fc4c*b586e132:create_test_csharp3",
                Subject = "hello csharp",
                Message = "a test messag from csharp sdk"
            };
            try
            {
                // 发送请求并返回响应
                PublishResponse response = smnClient.SendRequest(request);
                string result = response.MessageId;
                Console.WriteLine("{0}", result);
                Console.ReadLine();
            }
            catch (Exception e)
            {
                // 处理异常
                Console.WriteLine("{0}", e.Message);
                Console.ReadLine();
            }
        }
    }
}     
```

## HTTP参数设置和使用代理<a name="section1635184954510"></a>

以下示例代码向您展示了如何自定义设置HTTP参数和使用代理：

1.  创建ClientConfiguration并设置相应参数。
2.  创建服务实例并设置ClientConfiguration。

```
     ClientConfiguration configuration = new ClientConfiguration
     {
        Timeout = 80000,
        ProxyHost = "127.0.0.1",
        ProxyPort = 808,
        ProxyUsername = "break",
        ProxyPassword = "123456"
      };
     smnClient = new SmnClient(
        "YourAccountUserName",
        "YourAccountPassword",
        "YourAccountDomainName",
        "YourRegionName",
        configuration);
```

## 更多示例代码请参考github上的example项目<a name="section1151104915458"></a>

[Example项目地址](https://github.com/SimpleMessageNotification/smn-sdk-net/tree/master/smn-sdk-net-example)

