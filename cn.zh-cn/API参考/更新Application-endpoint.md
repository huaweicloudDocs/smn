# 更新Application endpoint<a name="smn_api_58002"></a>

## 功能介绍<a name="zh-cn_topic_0118694307_section663215"></a>

-   接口名称

    UpdateApplicationEndpoint

-   功能描述

    更新设备属性。


## URI<a name="zh-cn_topic_0118694307_section5968939"></a>

-   URI格式

    PUT /v2/\{project\_id\}/notifications/endpoints/\{endpoint\_urn\}

-   参数说明

    <a name="zh-cn_topic_0118694307_table61411666"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0118694307_row49774232"><th class="cellrowborder" valign="top" width="20.990000000000002%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0118694307_p5180964"><a name="zh-cn_topic_0118694307_p5180964"></a><a name="zh-cn_topic_0118694307_p5180964"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.75%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0118694307_p17004965"><a name="zh-cn_topic_0118694307_p17004965"></a><a name="zh-cn_topic_0118694307_p17004965"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="20.990000000000002%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0118694307_p35224963"><a name="zh-cn_topic_0118694307_p35224963"></a><a name="zh-cn_topic_0118694307_p35224963"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="38.269999999999996%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0118694307_p34649765"><a name="zh-cn_topic_0118694307_p34649765"></a><a name="zh-cn_topic_0118694307_p34649765"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0118694307_row39390935"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0118694307_p36549175"><a name="zh-cn_topic_0118694307_p36549175"></a><a name="zh-cn_topic_0118694307_p36549175"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.75%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0118694307_p7693179"><a name="zh-cn_topic_0118694307_p7693179"></a><a name="zh-cn_topic_0118694307_p7693179"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0118694307_p19167756"><a name="zh-cn_topic_0118694307_p19167756"></a><a name="zh-cn_topic_0118694307_p19167756"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.269999999999996%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0118694307_p9084369"><a name="zh-cn_topic_0118694307_p9084369"></a><a name="zh-cn_topic_0118694307_p9084369"></a>项目ID</p>
    <p id="zh-cn_topic_0118694307_p14650458"><a name="zh-cn_topic_0118694307_p14650458"></a><a name="zh-cn_topic_0118694307_p14650458"></a>获取项目ID请参考<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0118694307_row21768161"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0118694307_p18390601"><a name="zh-cn_topic_0118694307_p18390601"></a><a name="zh-cn_topic_0118694307_p18390601"></a>endpoint_urn</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.75%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0118694307_p13243689"><a name="zh-cn_topic_0118694307_p13243689"></a><a name="zh-cn_topic_0118694307_p13243689"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0118694307_p66105898"><a name="zh-cn_topic_0118694307_p66105898"></a><a name="zh-cn_topic_0118694307_p66105898"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.269999999999996%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0118694307_p52977523"><a name="zh-cn_topic_0118694307_p52977523"></a><a name="zh-cn_topic_0118694307_p52977523"></a>Endpoint的唯一资源标识，可通过<a href="查询Application的Endpoint列表.md">查询Application的Endpoint列表</a>获取该标识。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="zh-cn_topic_0118694307_section53720453"></a>

-   参数说明

    <a name="zh-cn_topic_0118694307_table45251091"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0118694307_row14981763"><th class="cellrowborder" valign="top" width="25%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0118694307_p5563313"><a name="zh-cn_topic_0118694307_p5563313"></a><a name="zh-cn_topic_0118694307_p5563313"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.06%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0118694307_p47975183"><a name="zh-cn_topic_0118694307_p47975183"></a><a name="zh-cn_topic_0118694307_p47975183"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="26.47%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0118694307_p60784581"><a name="zh-cn_topic_0118694307_p60784581"></a><a name="zh-cn_topic_0118694307_p60784581"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="26.47%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0118694307_p24604028"><a name="zh-cn_topic_0118694307_p24604028"></a><a name="zh-cn_topic_0118694307_p24604028"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0118694307_row30212363"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0118694307_p31282356"><a name="zh-cn_topic_0118694307_p31282356"></a><a name="zh-cn_topic_0118694307_p31282356"></a>enabled</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.06%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0118694307_p50842877"><a name="zh-cn_topic_0118694307_p50842877"></a><a name="zh-cn_topic_0118694307_p50842877"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.47%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0118694307_p24632334"><a name="zh-cn_topic_0118694307_p24632334"></a><a name="zh-cn_topic_0118694307_p24632334"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.47%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0118694307_p49062032"><a name="zh-cn_topic_0118694307_p49062032"></a><a name="zh-cn_topic_0118694307_p49062032"></a>设备是否可用，值为true或false字符串。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0118694307_row64305920"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0118694307_p41397042"><a name="zh-cn_topic_0118694307_p41397042"></a><a name="zh-cn_topic_0118694307_p41397042"></a>user_data</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.06%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0118694307_p64826129"><a name="zh-cn_topic_0118694307_p64826129"></a><a name="zh-cn_topic_0118694307_p64826129"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.47%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0118694307_p16425092"><a name="zh-cn_topic_0118694307_p16425092"></a><a name="zh-cn_topic_0118694307_p16425092"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.47%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0118694307_p55364084"><a name="zh-cn_topic_0118694307_p55364084"></a><a name="zh-cn_topic_0118694307_p55364084"></a>用户自定义数据，最大长度支持UTF-8编码后2048字节。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例

    ```
    PUT https://{SMN_Endpoint}/v2/{project_id}/notifications/endpoints/{endpoint_urn}
    {
        "enabled": "false", 
        "user_data": "This is a APNS token for user001"
    }
    ```


## 响应消息<a name="zh-cn_topic_0118694307_section13722030"></a>

-   要素说明

    <a name="zh-cn_topic_0118694307_table33599791"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0118694307_row25482430"><th class="cellrowborder" valign="top" width="29.872987298729875%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0118694307_p50810959"><a name="zh-cn_topic_0118694307_p50810959"></a><a name="zh-cn_topic_0118694307_p50810959"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="35.063506350635066%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0118694307_p22047016"><a name="zh-cn_topic_0118694307_p22047016"></a><a name="zh-cn_topic_0118694307_p22047016"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="35.063506350635066%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0118694307_p40977906"><a name="zh-cn_topic_0118694307_p40977906"></a><a name="zh-cn_topic_0118694307_p40977906"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0118694307_row17937528"><td class="cellrowborder" valign="top" width="29.872987298729875%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0118694307_p43653635"><a name="zh-cn_topic_0118694307_p43653635"></a><a name="zh-cn_topic_0118694307_p43653635"></a>request_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0118694307_p46283551"><a name="zh-cn_topic_0118694307_p46283551"></a><a name="zh-cn_topic_0118694307_p46283551"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0118694307_p57980147"><a name="zh-cn_topic_0118694307_p57980147"></a><a name="zh-cn_topic_0118694307_p57980147"></a>请求的唯一标识ID</p>
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

