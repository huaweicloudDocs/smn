# 开始使用<a name="ZH-CN_TOPIC_0093269618"></a>

## 使用示例代码发送短信<a name="section1352094510584"></a>

以下给出了发送短信的代码，采用华为云账号密码的方式创建服务实例。如您需要使用AK/SK方式请参考[以AK/SK访问密钥方式创建服务实例](#section42981531161017)，如果需要自定义HTTP参数或者使用代理，请参考[HTTP参数设置和使用代理](#section931483112105)。

```
import com.smn.client.DefaultSmnClient;
import com.smn.client.SmnClient;
import com.smn.request.sms.SmsPublishRequest;
import com.smn.response.sms.SmsPublishResponse;
public class SmsDemo {
    public static void main(String[] args) {
        SmnClient smnClient = new DefaultSmnClient(
                "YourAccountUserName",
                "YourAccountDomainName",
                "YourAccountPassword",
                "YourRegionName");
        // 构造请求对象
        SmsPublishRequest smnRequest = new SmsPublishRequest();
        // 设置参数,接收手机号，短信内容，短信签名ID
        smnRequest.setEndpoint("+86136*****587")
                .setMessage("您的验证码是:1234，请查收")
                .setSignId("6be340e91e52******837e6709104");
        // 发送短信
        try {
            SmsPublishResponse res = smnClient.sendRequest(smnRequest);
            System.out.println("httpCode:" + res.getHttpCode()
                    + ",message_id:" + res.getMessageId()
                    + ", request_id:" + res.getRequestId()
                    + ", errormessage:" + res.getMessage());
        } catch (Exception e) {
            // 处理异常
            e.printStackTrace();
        }
    }
} 
```

## 使用示例代码通过主题发布消息<a name="section48812047"></a>

以下给出了创建主题、添加订阅的示例代码，添加订阅成功会发送订阅确认消息给终端。

```
import com.smn.client.DefaultSmnClient;
import com.smn.client.SmnClient;
import com.smn.request.subscription.SubscribeRequest;
import com.smn.request.topic.CreateTopicRequest;
import com.smn.response.subscription.SubscribeResponse;
import com.smn.response.topic.CreateTopicResponse;
public class TopicDemo {
    public static void main(String[] args) {
        // 初始化smn client实例
        SmnClient smnClient = new DefaultSmnClient(
                "YourAccountUserName",
                "YourAccountDomainName",
                "YourAccountPassword",
                "YourRegionName");

        // 构造创建主题请求对象
        CreateTopicRequest createTopicRequest = new CreateTopicRequest();
        // 设置创建主题请求对象的参数,别名和主题名
        createTopicRequest.setDisplayName("topic display name")
                .setName("test_topic_name");
        CreateTopicResponse createTopicResponse;
        // 发送请求
        try {
            createTopicResponse = smnClient.sendRequest(createTopicRequest);
            if (!createTopicResponse.isSuccess()) {
                System.out.println("create topic fail.");
                return;
            }
        } catch (Exception e) {
            // 处理异常
            return;
        }
        String topicUrn = createTopicResponse.getTopicUrn();
        // 构造订阅请求对象
        SubscribeRequest subscribeRequest = new SubscribeRequest();
        // 设置参数, topicUrn,协议，终端，备注
        subscribeRequest.setTopicUrn(topicUrn)
                .setProtocol("sms")
                .setEndpoint("13688807587")
                .setRemark("hehe");
        // 发送请求
        try {
            SubscribeResponse subscribeResponse = smnClient.sendRequest(subscribeRequest);
            if (!subscribeResponse.isSuccess()) {
                System.out.println("subscribe fail.");
                return;
            }
        } catch (Exception e) {
            // 处理异常
            e.printStackTrace();
        }
    }
} 
```

终端确认订阅后，您可以向主题发布消息。

```
import com.smn.client.DefaultSmnClient;
import com.smn.client.SmnClient;
import com.smn.request.publish.PublishRequest;
import com.smn.response.publish.PublishResponse;
public class PublishDemo {
    public static void main(String[] args) {
        SmnClient smnClient = new DefaultSmnClient(
                "YourAccountUserName",
                "YourAccountDomainName",
                "YourAccountPassword",
                "YourRegionName");

        // 构造发布消息请求对象
        PublishRequest smnRequest = new PublishRequest();
        // 设置参数,主题，消息内容，topicUrn
        smnRequest.setSubject("message subject")
                .setMessage("message test content")
                .setTopicUrn("urn:smn:cn-north-1:cffe4fc4*****86e132:testTopicUrn");
        // 发送请求
        try {
            PublishResponse res = smnClient.sendRequest(smnRequest);
            System.out.println("httpCode:" + res.getHttpCode()
                    + ",message_id:" + res.getMessageId()
                    + ", request_id:" + res.getRequestId()
                    + ", errormessage:" + res.getMessage());
        } catch (Exception e) {
            // 处理异常
            e.printStackTrace();
        }
    }
}
```

## 以AK/SK访问密钥方式创建服务实例<a name="section42981531161017"></a>

开始使用中的示例代码向您展示了使用华为云账号密码方式创建服务实例，如您需要使用AK/SK方式调用SDK，可以如下创建SmnClient服务实例。

```
// aksk authentication  SmnClient 
smnClient = new AkskSmnClient(
        "YourAccessKeyId",
        "YourSecretAccessKey",
        "YourRegionName"
);
```

## HTTP参数设置和使用代理<a name="section931483112105"></a>

以下示例代码向您展示了如何自定义设置HTTP参数和使用代理：

1.  创建ClientConfiguration并设置相应参数
2.  创建服务实例并设置ClientConfiguration

    ```
    //如果需要自定义http参数或者使用代理，可以实例化ClientConfiguration并设置相关参数，        
    //然后按以下方式实例化SmnClient          
    ClientConfiguration clientConfiguration = new ClientConfiguration();
    // 设置连接超时时间，单位毫秒， 默认60000
    clientConfiguration.setConnectTimeOut(80000);
    // 设置socket超时时间，单位毫秒， 默认60000
    clientConfiguration.setSocketTimeOut(80000);
    // 设置最大http连接数
    clientConfiguration.setMaxConnections(1000);
    // 设置每个路由最大连接数
    clientConfiguration.setMaxConnectionsPerRoute(1000);
    // 忽略客户端证书校验
    clientConfiguration.setIgnoreCertificate(true);
    // 设置代理地址
    clientConfiguration.setProxyHost("127.0.0.1");
    // 设置代理端口
    clientConfiguration.setProxyPort(808);
    // 设置代理认证用户名
    clientConfiguration.setProxyUserName("break");
    // 设置代理认证密码
    clientConfiguration.setProxyPassword("123456");
    // 设置失败自动重试
    clientConfiguration.setAutoFailRetry(true);
    //设置重试次数
    clientConfiguration.setMaxRetryNum(3);
    // 初始化
    SmnClient smnClient = new DefaultSmnClient(
          "YourAccountUserName",
          "YourAccountDomainName",
          "YourAccountPassword",
           "YourRegionName",
          clientConfiguration);
    ```


## 更多示例代码请参考github上的example项目<a name="section12267105012813"></a>

[Example项目地址](https://github.com/SimpleMessageNotification/smn-sdk-java2.0/tree/master/smn-sdk-java-example/lib)

