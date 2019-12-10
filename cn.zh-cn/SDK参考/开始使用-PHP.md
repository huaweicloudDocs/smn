# 开始使用<a name="ZH-CN_TOPIC_0093269622"></a>

## 使用示例代码发送短信<a name="section1352094510584"></a>

以下给出了发送短信的代码，采用华为云账号密码的方式创建服务实例。如果需要自定义HTTP参数或者使用代理，请参考[HTTP参数设置和使用代理](#section42981531161017)。

```
<?php

require_once(__DIR__ . '/../smn-sdk-php/Bootstrap.php');
use SMN\Client\DefaultSmnClient as DefaultSmnClient;

$client = new DefaultSmnClient(
    'YourAccountUserName',
    'YourAccountDomainName',
    'YourAccountPassword',
    'YourRegionName');

$smnRequest = new SMN\Request\Sms\SmsPublishRequest();
$smnRequest->setEndpoint('86136*****587')
    ->setSignId('6be340e91e******d85837e6709104')
    ->setMessage('您的验证码是:12346，请查收');
$response = $client->sendRequest($smnRequest);
print_r($response->isSuccess());
print_r($response->body);
```

## 使用示例代码通过主题发布消息<a name="section21932166"></a>

以下给出了创建主题、添加订阅的示例代码，添加订阅成功会发送订阅确认消息给终端。

```
<?php
require_once(__DIR__ . '/../smn-sdk-php/Bootstrap.php');
use SMN\Client\DefaultSmnClient as DefaultSmnClient;

$client = new DefaultSmnClient(
    'YourAccountUserName',
    'YourAccountDomainName',
    'YourAccountPassword',
    'YourRegionName');

// 创建topic请求对象，并设置参数 
$topicRequest = new SMN\Request\Topic\CreateTopicRequest();
$topicRequest->setName('create_by_php_01')
    ->setDisplayName('topic display name');
$topicResponse = $client->sendRequest($topicRequest);
print_r($topicResponse->isSuccess());
print_r($topicResponse->body);

// 订阅请求对象，并设置参数
$smnRequest = new SMN\Request\Subscription\SubscribeRequest();
$smnRequest->setEndpoint('+86136*****587')
    ->setProtocol('sms')
    ->setTopicUrn($topicResponse->body->topic_urn);
$response = $client->sendRequest($smnRequest);

print_r($response->isSuccess());
print_r($response->body); 
```

终端确认订阅后，您可以向主题发布消息。

```
<?php
require_once(__DIR__ . '/../smn-sdk-php/Bootstrap.php');
use SMN\Client\DefaultSmnClient as DefaultSmnClient;

$client = new DefaultSmnClient(
    'YourAccountUserName',
    'YourAccountDomainName',
    'YourAccountPassword',
     'YourRegionName');

$smnRequest = new SMN\Request\Publish\PublishWithMessageRequest();
$smnRequest->setTopicUrn('urn:smn:cn-north-1:cffe4fc4c9a54219b60dbaf7b586e132:create_by_php_01')
    ->setMessage('test message by php sdk')
    ->setSubject('test message subject');

$response = $client->sendRequest($smnRequest);
print_r($response->isSuccess());
print_r($response->body);
```

## HTTP参数设置和使用代理<a name="section42981531161017"></a>

以下示例代码向您展示了如何自定义设置HTTP参数和使用代理：

1.  创建ClientConfiguration并设置相应参数。
2.  创建服务实例并设置ClientConfiguration。

```
$client = new DefaultSmnClient(
    'YourAccountUserName',
    'YourAccountDomainName',
    'YourAccountPassword',
    'YourRegionName');
// 设置代理
$config = new \SMN\Common\ClientConfiguration();
$config->setProxyHost('127.0.0.1');
$config->setProxyPort(8080);
$config->setTimeout(80);
$client->setClientConfiguration($config);
```

## 更多示例代码请参考github上的example项目<a name="section17161895276"></a>

[Example项目地址](https://github.com/SimpleMessageNotification/smn-sdk-php/tree/master/smn-sdk-php-example)

