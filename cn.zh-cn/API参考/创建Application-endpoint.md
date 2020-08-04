# 创建Application endpoint<a name="smn_api_58001"></a>

## 功能介绍<a name="zh-cn_topic_0118694341_section51620241"></a>

-   接口名称

    CreateApplicationEndpoint

-   功能描述

    创建应用平台的endpoint终端。


## URI<a name="zh-cn_topic_0118694341_section61928986"></a>

-   URI格式

    POST /v2/\{project\_id\}/notifications/applications/\{application\_urn\}/endpoints

-   参数说明

    <a name="zh-cn_topic_0118694341_table47631980"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0118694341_row23143009"><th class="cellrowborder" valign="top" width="20.990000000000002%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0118694341_p62644474"><a name="zh-cn_topic_0118694341_p62644474"></a><a name="zh-cn_topic_0118694341_p62644474"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.75%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0118694341_p41037639"><a name="zh-cn_topic_0118694341_p41037639"></a><a name="zh-cn_topic_0118694341_p41037639"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="20.990000000000002%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0118694341_p35714481"><a name="zh-cn_topic_0118694341_p35714481"></a><a name="zh-cn_topic_0118694341_p35714481"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="38.269999999999996%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0118694341_p7191839"><a name="zh-cn_topic_0118694341_p7191839"></a><a name="zh-cn_topic_0118694341_p7191839"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0118694341_row8127785"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0118694341_p54370837"><a name="zh-cn_topic_0118694341_p54370837"></a><a name="zh-cn_topic_0118694341_p54370837"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.75%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0118694341_p41961637"><a name="zh-cn_topic_0118694341_p41961637"></a><a name="zh-cn_topic_0118694341_p41961637"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0118694341_p43449409"><a name="zh-cn_topic_0118694341_p43449409"></a><a name="zh-cn_topic_0118694341_p43449409"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.269999999999996%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0118694341_p29741266"><a name="zh-cn_topic_0118694341_p29741266"></a><a name="zh-cn_topic_0118694341_p29741266"></a>项目ID</p>
    <p id="zh-cn_topic_0118694341_p66344810"><a name="zh-cn_topic_0118694341_p66344810"></a><a name="zh-cn_topic_0118694341_p66344810"></a>获取项目ID请参考<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0118694341_row20211337"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0118694341_p26505564"><a name="zh-cn_topic_0118694341_p26505564"></a><a name="zh-cn_topic_0118694341_p26505564"></a>application_urn</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.75%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0118694341_p66575977"><a name="zh-cn_topic_0118694341_p66575977"></a><a name="zh-cn_topic_0118694341_p66575977"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0118694341_p23945046"><a name="zh-cn_topic_0118694341_p23945046"></a><a name="zh-cn_topic_0118694341_p23945046"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.269999999999996%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0118694341_p60500555"><a name="zh-cn_topic_0118694341_p60500555"></a><a name="zh-cn_topic_0118694341_p60500555"></a>Application的唯一资源标识，可通过<a href="查询Application.md">查询Application</a>获取该标识。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="zh-cn_topic_0118694341_section20489970"></a>

-   参数说明

    <a name="zh-cn_topic_0118694341_table15085678"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0118694341_row21558799"><th class="cellrowborder" valign="top" width="25%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0118694341_p1432296"><a name="zh-cn_topic_0118694341_p1432296"></a><a name="zh-cn_topic_0118694341_p1432296"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.06%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0118694341_p48907186"><a name="zh-cn_topic_0118694341_p48907186"></a><a name="zh-cn_topic_0118694341_p48907186"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="26.47%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0118694341_p2059157"><a name="zh-cn_topic_0118694341_p2059157"></a><a name="zh-cn_topic_0118694341_p2059157"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="26.47%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0118694341_p32574008"><a name="zh-cn_topic_0118694341_p32574008"></a><a name="zh-cn_topic_0118694341_p32574008"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0118694341_row43444447"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0118694341_p29339315"><a name="zh-cn_topic_0118694341_p29339315"></a><a name="zh-cn_topic_0118694341_p29339315"></a>token</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.06%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0118694341_p27674344"><a name="zh-cn_topic_0118694341_p27674344"></a><a name="zh-cn_topic_0118694341_p27674344"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.47%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0118694341_p27029414"><a name="zh-cn_topic_0118694341_p27029414"></a><a name="zh-cn_topic_0118694341_p27029414"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.47%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0118694341_p41898900"><a name="zh-cn_topic_0118694341_p41898900"></a><a name="zh-cn_topic_0118694341_p41898900"></a>移动应用设备token，最大长度512个字节。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0118694341_row9765038"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0118694341_p52770604"><a name="zh-cn_topic_0118694341_p52770604"></a><a name="zh-cn_topic_0118694341_p52770604"></a>user_data</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.06%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0118694341_p46560535"><a name="zh-cn_topic_0118694341_p46560535"></a><a name="zh-cn_topic_0118694341_p46560535"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.47%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0118694341_p13306966"><a name="zh-cn_topic_0118694341_p13306966"></a><a name="zh-cn_topic_0118694341_p13306966"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.47%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0118694341_p4122450"><a name="zh-cn_topic_0118694341_p4122450"></a><a name="zh-cn_topic_0118694341_p4122450"></a>用户自定义数据，</p>
    <p id="zh-cn_topic_0118694341_p65482994"><a name="zh-cn_topic_0118694341_p65482994"></a><a name="zh-cn_topic_0118694341_p65482994"></a>最大长度支持UTF-8编码后2048字节。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例

    ```
    POST https://{SMN_Endpoint}/v2/{project_id}/notifications/applications/{application_urn}/endpoints
    {
        "token": "3708232124742383445",
        "user_data": "This is token for user001"
    }
    ```


## 响应消息<a name="zh-cn_topic_0118694341_section50192009"></a>

-   要素说明

    <a name="zh-cn_topic_0118694341_table39838269"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0118694341_row58294142"><th class="cellrowborder" valign="top" width="29.872987298729875%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0118694341_p24205051"><a name="zh-cn_topic_0118694341_p24205051"></a><a name="zh-cn_topic_0118694341_p24205051"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="35.063506350635066%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0118694341_p14452096"><a name="zh-cn_topic_0118694341_p14452096"></a><a name="zh-cn_topic_0118694341_p14452096"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="35.063506350635066%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0118694341_p29769142"><a name="zh-cn_topic_0118694341_p29769142"></a><a name="zh-cn_topic_0118694341_p29769142"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0118694341_row28550227"><td class="cellrowborder" valign="top" width="29.872987298729875%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0118694341_p30867083"><a name="zh-cn_topic_0118694341_p30867083"></a><a name="zh-cn_topic_0118694341_p30867083"></a>request_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0118694341_p17205779"><a name="zh-cn_topic_0118694341_p17205779"></a><a name="zh-cn_topic_0118694341_p17205779"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0118694341_p51490835"><a name="zh-cn_topic_0118694341_p51490835"></a><a name="zh-cn_topic_0118694341_p51490835"></a>请求的唯一标识ID</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0118694341_row22964184"><td class="cellrowborder" valign="top" width="29.872987298729875%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0118694341_p48159629"><a name="zh-cn_topic_0118694341_p48159629"></a><a name="zh-cn_topic_0118694341_p48159629"></a>endpoint_urn</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0118694341_p8615862"><a name="zh-cn_topic_0118694341_p8615862"></a><a name="zh-cn_topic_0118694341_p8615862"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0118694341_p26796220"><a name="zh-cn_topic_0118694341_p26796220"></a><a name="zh-cn_topic_0118694341_p26796220"></a>Endpoint的唯一资源标识</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "request_id": "6a63a18b8bab40ffb71ebd9cb80d0085", 
        "endpoint_urn": "urn:smn:regionId:f96188c7ccaf4ffba0c9aa149ab2bd57:endpoint-APNS-example_application_name-37a2cb947fa43a20bc66e91281194e7a"
    }
    ```


## 返回值<a name="section242171292113"></a>

请参考[返回值](返回值.md)。

## 错误码<a name="section73211020122511"></a>

请参考[错误码说明](错误码说明.md)。

