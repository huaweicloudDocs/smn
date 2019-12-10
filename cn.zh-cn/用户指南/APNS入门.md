# APNS入门<a name="smn_ug_0019"></a>

Apple Push Notification Service \(APNS\) 是用于推送iOS消息的服务。本节介绍如何使用APNS推送移动应用消息的准备工作。

## 使用APNS推送移动应用消息的准备工作<a name="section266667193418"></a>

要使用SMN推送iOS消息，需要获得：

-   获取申请iOS证书（.p12格式）
-   iOS应用集成苹果推送能力
-   获取设备token

如果您已做好这些准备工作，则可使用SMN控制台或SMN API将移动应用消息推送到iOS应用程序。

## 使用APNS的步骤<a name="section109741514173811"></a>

1.  注册Apple账号，进入苹果开发者中心，申请成为苹果的应用开发会员（Developer Program Membership），申请会员需要缴纳一笔费用。成为会员后，申请iOS推送证书（.p12）。
2.  开发人员在开发iOS应用时，集成iOS推送证书（.p12）。
3.  获取设备token。

    集成iOS推送的iOS应用安装到iOS设备（如iphone）上，就可以获取APNS给应用分配的设备token。


