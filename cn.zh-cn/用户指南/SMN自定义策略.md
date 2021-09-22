# SMN自定义策略<a name="smn_ug_0038"></a>

如果系统预置的SMN权限，不满足您的授权要求，可以创建自定义策略。自定义策略中可以添加的授权项（Action）请参考《消息通知服务接口参考》中“  [策略及授权项说明](https://support.huaweicloud.com/api-smn/smn_api_80001.html)”章节_。_

目前华为云支持以下两种方式创建自定义策略：

-   可视化视图创建自定义策略：无需了解策略语法，按可视化视图导航栏选择云服务、操作、资源、条件等策略内容，可自动生成策略。
-   JSON视图创建自定义策略：可以在选择策略模板后，根据具体需求编辑策略内容；也可以直接在编辑框内编写JSON格式的策略内容。

具体创建步骤请参见：[创建自定义策略](https://support.huaweicloud.com/usermanual-iam/iam_01_0605.html)。本章为您介绍常用的SMN自定义策略样例。

## SMN自定义策略样例<a name="section7529733164812"></a>

-   示例1：授权用户创建主题

    ```
    {
        "Version": "1.1",
        "Statement": [
            {
                "Effect": "Allow",
                "Action": [
                    "smn:topic:create"
                ]
            }
        ]
    }
    ```

-   示例2：拒绝用户删除主题

    拒绝策略需要同时配合其他策略使用，否则没有实际作用。用户被授予的策略中，一个授权项的作用如果同时存在Allow和Deny，则遵循**Deny优先原则**。

    如果您给用户授予SMN FullAccess的系统策略，但不希望用户拥有SMN FullAccess中定义的删除主题权限，您可以创建一条拒绝删除主题的自定义策略，然后同时将SMN FullAccess和拒绝策略授予用户，根据Deny优先原则，则用户可以对SMN执行除了删除主题外的所有操作。拒绝策略示例如下：

    ```
    {
        "Version": "1.1",
        "Statement": [
            {
                "Effect": "Deny",
                "Action": [
                    "smn:topic:delete"
                ]
            }
        ]
    }
    ```

-   示例3：多个授权项策略

    一个自定义策略中可以包含多个授权项，且除了可以包含本服务的授权项外，还可以包含其他服务的授权项，可以包含的其他服务必须跟本服务同属性，即都是项目级服务或都是全局级服务。多个授权语句策略描述如下：

    ```
    {
        "Version": "1.1",
        "Statement": [
            {
                "Effect": "Allow",
                "Action": [
                    "smn:topic:create",
                    "smn:tag:create",
                    "smn:application:create"
                ]
            },
            {
                "Effect": "Allow",
                "Action": [
                    "elb:certificates:create",
                    "elb:whitelists:create",
                    "elb:pools:create",
                    "elb:members:create",
                    "elb:healthmonitors:create",
                    "elb:l7policies:create",
                    "elb:listeners:create",
                    "elb:loadbalancers:create"
                ]
            }
        ]
    }
    ```


