# 更新Application<a name="ZH-CN_TOPIC_0118712459"></a>

## 功能介绍<a name="zh-cn_topic_0118694336_section16390883"></a>

-   接口名称

    UpdateApplication

-   功能描述

    更新应用平台。


## URI<a name="zh-cn_topic_0118694336_section13300219"></a>

-   URI格式

    PUT /v2/\{project\_id\}/notifications/applications/\{application\_urn\}

-   参数说明

    <a name="zh-cn_topic_0118694336_table23280985"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0118694336_row7234794"><th class="cellrowborder" valign="top" width="20.990000000000002%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0118694336_p49147423"><a name="zh-cn_topic_0118694336_p49147423"></a><a name="zh-cn_topic_0118694336_p49147423"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.75%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0118694336_p21518341"><a name="zh-cn_topic_0118694336_p21518341"></a><a name="zh-cn_topic_0118694336_p21518341"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="20.990000000000002%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0118694336_p65264067"><a name="zh-cn_topic_0118694336_p65264067"></a><a name="zh-cn_topic_0118694336_p65264067"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="38.269999999999996%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0118694336_p51898114"><a name="zh-cn_topic_0118694336_p51898114"></a><a name="zh-cn_topic_0118694336_p51898114"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0118694336_row60264738"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0118694336_p49605586"><a name="zh-cn_topic_0118694336_p49605586"></a><a name="zh-cn_topic_0118694336_p49605586"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.75%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0118694336_p58629539"><a name="zh-cn_topic_0118694336_p58629539"></a><a name="zh-cn_topic_0118694336_p58629539"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0118694336_p51372220"><a name="zh-cn_topic_0118694336_p51372220"></a><a name="zh-cn_topic_0118694336_p51372220"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.269999999999996%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0118694336_p400326"><a name="zh-cn_topic_0118694336_p400326"></a><a name="zh-cn_topic_0118694336_p400326"></a>项目ID</p>
    <p id="zh-cn_topic_0118694336_p3602941"><a name="zh-cn_topic_0118694336_p3602941"></a><a name="zh-cn_topic_0118694336_p3602941"></a>获取项目ID请参考<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0118694336_row16578861"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0118694336_p710483"><a name="zh-cn_topic_0118694336_p710483"></a><a name="zh-cn_topic_0118694336_p710483"></a>application_urn</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.75%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0118694336_p57549199"><a name="zh-cn_topic_0118694336_p57549199"></a><a name="zh-cn_topic_0118694336_p57549199"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0118694336_p30973510"><a name="zh-cn_topic_0118694336_p30973510"></a><a name="zh-cn_topic_0118694336_p30973510"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.269999999999996%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0118694336_p25826402"><a name="zh-cn_topic_0118694336_p25826402"></a><a name="zh-cn_topic_0118694336_p25826402"></a>Application的唯一资源标识，可通过<a href="查询Application.md">查询Application</a>获取该标识。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="zh-cn_topic_0118694336_section52593113"></a>

-   参数说明

    <a name="zh-cn_topic_0118694336_table37413794"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0118694336_row37253958"><th class="cellrowborder" valign="top" width="24.997500249975%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0118694336_p64780582"><a name="zh-cn_topic_0118694336_p64780582"></a><a name="zh-cn_topic_0118694336_p64780582"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="14.708529147085292%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0118694336_p12735762"><a name="zh-cn_topic_0118694336_p12735762"></a><a name="zh-cn_topic_0118694336_p12735762"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="14.708529147085292%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0118694336_p24963827"><a name="zh-cn_topic_0118694336_p24963827"></a><a name="zh-cn_topic_0118694336_p24963827"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="45.58544145585442%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0118694336_p8804145"><a name="zh-cn_topic_0118694336_p8804145"></a><a name="zh-cn_topic_0118694336_p8804145"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0118694336_row50376418"><td class="cellrowborder" valign="top" width="24.997500249975%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0118694336_p53958053"><a name="zh-cn_topic_0118694336_p53958053"></a><a name="zh-cn_topic_0118694336_p53958053"></a>platform_principal</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.708529147085292%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0118694336_p8526181"><a name="zh-cn_topic_0118694336_p8526181"></a><a name="zh-cn_topic_0118694336_p8526181"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.708529147085292%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0118694336_p19532041"><a name="zh-cn_topic_0118694336_p19532041"></a><a name="zh-cn_topic_0118694336_p19532041"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="45.58544145585442%" headers="mcps1.1.5.1.4 "><a name="ul11518185512190"></a><a name="ul11518185512190"></a><ul id="ul11518185512190"><li>对于HMS平台是APP ID，只能包含英文字母和数字，最大20个字符。</li><li>对于苹果APNS、APNS_SandBox平台是推送证书，大小不超过8K，且是Base64编码。</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0118694336_row14576408"><td class="cellrowborder" valign="top" width="24.997500249975%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0118694336_p39838439"><a name="zh-cn_topic_0118694336_p39838439"></a><a name="zh-cn_topic_0118694336_p39838439"></a>platform_credential</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.708529147085292%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0118694336_p5688159"><a name="zh-cn_topic_0118694336_p5688159"></a><a name="zh-cn_topic_0118694336_p5688159"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.708529147085292%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0118694336_p58087719"><a name="zh-cn_topic_0118694336_p58087719"></a><a name="zh-cn_topic_0118694336_p58087719"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="45.58544145585442%" headers="mcps1.1.5.1.4 "><a name="ul1026444616231"></a><a name="ul1026444616231"></a><ul id="ul1026444616231"><li>对于HMS平台是APP SECRET，只能包含英文字母和数字，固定32个字符。</li><li>对于苹果APNS、APNS_SandBox平台是推送证书的私钥（private key），大小不超过8K，且是Base64编码。</li></ul>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例

    ```
    PUT https://{SMN_Endpoint}/v2/{project_id}/notifications/applications/{application_urn} 
    {
        "platform_principal": "appId", 
        "platform_credential": "appSecret"
    }
    ```


## 响应消息<a name="zh-cn_topic_0118694336_section3575973"></a>

-   要素说明

    <a name="zh-cn_topic_0118694336_table22715326"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0118694336_row534076"><th class="cellrowborder" valign="top" width="29.872987298729875%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0118694336_p43260163"><a name="zh-cn_topic_0118694336_p43260163"></a><a name="zh-cn_topic_0118694336_p43260163"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="35.063506350635066%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0118694336_p14412335"><a name="zh-cn_topic_0118694336_p14412335"></a><a name="zh-cn_topic_0118694336_p14412335"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="35.063506350635066%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0118694336_p26548520"><a name="zh-cn_topic_0118694336_p26548520"></a><a name="zh-cn_topic_0118694336_p26548520"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0118694336_row37341343"><td class="cellrowborder" valign="top" width="29.872987298729875%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0118694336_p4749933"><a name="zh-cn_topic_0118694336_p4749933"></a><a name="zh-cn_topic_0118694336_p4749933"></a>request_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0118694336_p49200296"><a name="zh-cn_topic_0118694336_p49200296"></a><a name="zh-cn_topic_0118694336_p49200296"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0118694336_p25801015"><a name="zh-cn_topic_0118694336_p25801015"></a><a name="zh-cn_topic_0118694336_p25801015"></a>请求的唯一标识ID</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
       "request_id": "6a63a18b8bab40ffb71ebd9cb80d0085"
    }
    ```


## 返回值<a name="section242171292113"></a>

请参考[返回值](返回值.md)。

## 错误码<a name="section73211020122511"></a>

请参考[错误码说明](错误码说明.md)。

