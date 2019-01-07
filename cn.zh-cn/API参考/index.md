# 消息通知服务接口参考

-   [使用前必读](使用前必读.md)
-   [接口简介](接口简介.md)
-   [环境准备]
    -   [获取请求认证](获取请求认证.md)
    -   [获取项目ID](获取项目ID.md)

-   [接口调用方法]
    -   [REST API介绍](REST-API介绍.md)
    -   [示例](示例.md)

-   [API]
    -   [Topic操作]
        -   [创建Topic](创建Topic.md)
        -   [更新Topic](更新Topic.md)
        -   [删除Topic](删除Topic.md)
        -   [查询Topic列表](查询Topic列表.md)
        -   [查询Topic详情](查询Topic详情.md)
        -   [查询Topic属性](查询Topic属性.md)
        -   [更新Topic属性](更新Topic属性.md)
        -   [删除指定名称的Topic属性](删除指定名称的Topic属性.md)
        -   [删除所有Topic属性](删除所有Topic属性.md)

    -   [订阅操作]
        -   [查询订阅者列表](查询订阅者列表.md)
        -   [查询指定主题的订阅者列表](查询指定主题的订阅者列表.md)
        -   [订阅](订阅.md)
        -   [取消订阅](取消订阅.md)

    -   [模板操作]
        -   [创建消息模板](创建消息模板.md)
        -   [更新消息模板](更新消息模板.md)
        -   [删除消息模板](删除消息模板.md)
        -   [查询消息模板列表](查询消息模板列表.md)
        -   [查询消息模板详情](查询消息模板详情.md)

    -   [发布消息操作]
        -   [消息发布](消息发布.md)
        -   [使用消息结构体方式的消息发布](使用消息结构体方式的消息发布.md)
        -   [使用消息模板方式的消息发布](使用消息模板方式的消息发布.md)

    -   [短信操作]
        -   [发送短信验证码或短信通知](发送短信验证码或短信通知.md)
        -   [批量发送短信验证码或短信通知](批量发送短信验证码或短信通知.md)
        -   [批量发送不同内容的短信验证码或短信通知](批量发送不同内容的短信验证码或短信通知.md)
        -   [批量发送推广类短信](批量发送推广类短信.md)
        -   [批量发送不同内容的推广类短信](批量发送不同内容的推广类短信.md)
        -   [查询短信签名](查询短信签名.md)
        -   [删除短信签名](删除短信签名.md)
        -   [查询短信的发送状态](查询短信的发送状态.md)
        -   [查询已发送短信的内容](查询已发送短信的内容.md)
        -   [查询短信回调事件](查询短信回调事件.md)
        -   [更新短信回调事件](更新短信回调事件.md)
        -   [创建短信模板](创建短信模板.md)
        -   [查询短信模板](查询短信模板.md)
        -   [删除短信模板](删除短信模板.md)
        -   [查询短信模板详情](查询短信模板详情.md)

    -   [使用标签管理服务]
        -   [查询资源实例](查询资源实例.md)
        -   [批量添加删除资源标签](批量添加删除资源标签.md)
        -   [添加资源标签](添加资源标签.md)
        -   [删除资源标签](删除资源标签.md)
        -   [查询资源标签](查询资源标签.md)
        -   [查询项目标签](查询项目标签.md)

    -   [Application操作]
        -   [创建Application](创建Application.md)
        -   [更新Application](更新Application.md)
        -   [删除Application](删除Application.md)
        -   [查询Application](查询Application.md)
        -   [查询Application属性](查询Application属性.md)

    -   [Application endpoint操作]
        -   [创建Application endpoint](创建Application-endpoint.md)
        -   [更新Application endpoint](更新Application-endpoint.md)
        -   [删除Application endpoint](删除Application-endpoint.md)
        -   [查询Application的Endpoint列表](查询Application的Endpoint列表.md)
        -   [查询Application的Endpoint属性](查询Application的Endpoint属性.md)

    -   [Application直发消息操作]
        -   [App消息发布](App消息发布.md)
        -   [使用消息结构体方式的App消息发布](使用消息结构体方式的App消息发布.md)
    -   [查询版本操作]
        -   [查询SMN支持的API版本号信息](查询SMN支持的API版本号信息.md)
        -   [查询SMN API V2版本信息](查询SMN-API-V2版本信息.md)


-   [公共参数]
    -   [通用请求返回值]
        -   [异常响应](异常响应.md)
        -   [返回值](返回值.md)

    -   [错误码说明](错误码说明.md)

-   [附录]
    -   [结构体说明]
        -   [Topic结构体](Topic结构体.md)
        -   [Subscription结构体](Subscription结构体.md)
        -   [Message\_template结构体](Message_template结构体.md)
        -   [Sms\_sign结构体](Sms_sign结构体.md)
        -   [Sms\_statistic\_data结构体](Sms_statistic_data结构体.md)
        -   [Sms\_report\_data结构体](Sms_report_data结构体.md)
        -   [Sms\_callback结构体](Sms_callback结构体.md)
        -   [Sms\_template结构体](Sms_template结构体.md)
        -   [Sms\_commit\_result结构体](Sms_commit_result结构体.md)
        -   [Sms\_message结构体](Sms_message结构体.md)
        -   [Promotion\_sms\_commit\_result结构体](Promotion_sms_commit_result结构体.md)
        -   [Tags结构体](Tags结构体.md)
        -   [Match结构体](Match结构体.md)
        -   [Resource结构体](Resource结构体.md)
        -   [Resource\_tag结构体](Resource_tag结构体.md)
        -   [Application结构体](Application结构体.md)
        -   [Application\_attributes结构体](Application_attributes结构体.md)
        -   [Application\_endpoint结构体](Application_endpoint结构体.md)
        -   [Endpoint\_attributes结构体](Endpoint_attributes结构体.md)
        -   [Versions结构体](Versions结构体.md)
        -   [Links结构体](Links结构体.md)

    -   [审批失败错误码说明](审批失败错误码说明.md)
    -   [Topic属性表](Topic属性表.md)
    -   [Cmpp发送状态描述表](Cmpp发送状态描述表.md)
    -   [国家码和地区码](国家码和地区码.md)
    -   [短信回调事件说明](短信回调事件说明.md)
    -   [application消息体格式](application消息体格式.md)

