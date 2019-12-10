# 查询Application的Endpoint属性<a name="ZH-CN_TOPIC_0118712468"></a>

## 功能介绍<a name="zh-cn_topic_0118694310_section19253649"></a>

-   接口名称

    GetApplicationEndpointAttributes

-   功能描述

    获取endpoint的属性。


## URI<a name="zh-cn_topic_0118694310_section39065117"></a>

-   URI格式

    GET /v2/\{project\_id\}/notifications/endpoints/\{endpoint\_urn\}

-   参数说明

    <a name="zh-cn_topic_0118694310_table28010135"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0118694310_row48692557"><th class="cellrowborder" valign="top" width="20.990000000000002%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0118694310_p51783064"><a name="zh-cn_topic_0118694310_p51783064"></a><a name="zh-cn_topic_0118694310_p51783064"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.75%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0118694310_p33678668"><a name="zh-cn_topic_0118694310_p33678668"></a><a name="zh-cn_topic_0118694310_p33678668"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="20.990000000000002%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0118694310_p43617551"><a name="zh-cn_topic_0118694310_p43617551"></a><a name="zh-cn_topic_0118694310_p43617551"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="38.269999999999996%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0118694310_p43360780"><a name="zh-cn_topic_0118694310_p43360780"></a><a name="zh-cn_topic_0118694310_p43360780"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0118694310_row15605454"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0118694310_p56082276"><a name="zh-cn_topic_0118694310_p56082276"></a><a name="zh-cn_topic_0118694310_p56082276"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.75%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0118694310_p46370514"><a name="zh-cn_topic_0118694310_p46370514"></a><a name="zh-cn_topic_0118694310_p46370514"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0118694310_p65024193"><a name="zh-cn_topic_0118694310_p65024193"></a><a name="zh-cn_topic_0118694310_p65024193"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.269999999999996%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0118694310_p32468313"><a name="zh-cn_topic_0118694310_p32468313"></a><a name="zh-cn_topic_0118694310_p32468313"></a>项目ID</p>
    <p id="zh-cn_topic_0118694310_p23779363"><a name="zh-cn_topic_0118694310_p23779363"></a><a name="zh-cn_topic_0118694310_p23779363"></a>获取项目ID请参考<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0118694310_row55405230"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0118694310_p58638646"><a name="zh-cn_topic_0118694310_p58638646"></a><a name="zh-cn_topic_0118694310_p58638646"></a>endpoint_urn</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.75%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0118694310_p52109899"><a name="zh-cn_topic_0118694310_p52109899"></a><a name="zh-cn_topic_0118694310_p52109899"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0118694310_p60152276"><a name="zh-cn_topic_0118694310_p60152276"></a><a name="zh-cn_topic_0118694310_p60152276"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.269999999999996%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0118694310_p40496186"><a name="zh-cn_topic_0118694310_p40496186"></a><a name="zh-cn_topic_0118694310_p40496186"></a>Endpoint的唯一资源标识，可通过<a href="查询Application的Endpoint列表.md">查询Application的Endpoint列表</a>获取该标识。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="zh-cn_topic_0118694310_section16041741"></a>

-   请求样例

    ```
    GET https://{SMN_Endpoint}/v2/{project_id}/notifications/endpoints/{endpoint_urn}
    ```


## 响应消息<a name="zh-cn_topic_0118694310_section10157945"></a>

-   要素说明

    <a name="zh-cn_topic_0118694310_table39016537"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0118694310_row38686068"><th class="cellrowborder" valign="top" width="29.872987298729875%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0118694310_p46563795"><a name="zh-cn_topic_0118694310_p46563795"></a><a name="zh-cn_topic_0118694310_p46563795"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="35.063506350635066%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0118694310_p13571075"><a name="zh-cn_topic_0118694310_p13571075"></a><a name="zh-cn_topic_0118694310_p13571075"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="35.063506350635066%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0118694310_p25515308"><a name="zh-cn_topic_0118694310_p25515308"></a><a name="zh-cn_topic_0118694310_p25515308"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0118694310_row36429702"><td class="cellrowborder" valign="top" width="29.872987298729875%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0118694310_p65124744"><a name="zh-cn_topic_0118694310_p65124744"></a><a name="zh-cn_topic_0118694310_p65124744"></a>request_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0118694310_p40612898"><a name="zh-cn_topic_0118694310_p40612898"></a><a name="zh-cn_topic_0118694310_p40612898"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0118694310_p1310461"><a name="zh-cn_topic_0118694310_p1310461"></a><a name="zh-cn_topic_0118694310_p1310461"></a>请求的唯一标识ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0118694310_row15802441"><td class="cellrowborder" valign="top" width="29.872987298729875%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0118694310_p4929340"><a name="zh-cn_topic_0118694310_p4929340"></a><a name="zh-cn_topic_0118694310_p4929340"></a>attributes</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.2 "><p id="p32101619144816"><a name="p32101619144816"></a><a name="p32101619144816"></a>Endpoint_attributes结构体</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0118694310_p62040064"><a name="zh-cn_topic_0118694310_p62040064"></a><a name="zh-cn_topic_0118694310_p62040064"></a>属性的键值对。</p>
    <p id="zh-cn_topic_0118694338_p49277517"><a name="zh-cn_topic_0118694338_p49277517"></a><a name="zh-cn_topic_0118694338_p49277517"></a>请参见<a href="#table219819244718">表1</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 1**  Endpoint\_attributes结构体

    <a name="table219819244718"></a>
    <table><thead align="left"><tr id="row1526011204718"><th class="cellrowborder" valign="top" width="34.33%" id="mcps1.2.4.1.1"><p id="p182602274711"><a name="p182602274711"></a><a name="p182602274711"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="25.369999999999997%" id="mcps1.2.4.1.2"><p id="p19260192154719"><a name="p19260192154719"></a><a name="p19260192154719"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="40.300000000000004%" id="mcps1.2.4.1.3"><p id="p126017204718"><a name="p126017204718"></a><a name="p126017204718"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row15260132164715"><td class="cellrowborder" valign="top" width="34.33%" headers="mcps1.2.4.1.1 "><p id="p8907105518498"><a name="p8907105518498"></a><a name="p8907105518498"></a>enabled</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.369999999999997%" headers="mcps1.2.4.1.2 "><p id="p129078554491"><a name="p129078554491"></a><a name="p129078554491"></a>boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.300000000000004%" headers="mcps1.2.4.1.3 "><p id="p390755554913"><a name="p390755554913"></a><a name="p390755554913"></a>设备是否可用</p>
    </td>
    </tr>
    <tr id="row926062154712"><td class="cellrowborder" valign="top" width="34.33%" headers="mcps1.2.4.1.1 "><p id="p1390725544917"><a name="p1390725544917"></a><a name="p1390725544917"></a>token</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.369999999999997%" headers="mcps1.2.4.1.2 "><p id="p18907455114917"><a name="p18907455114917"></a><a name="p18907455114917"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.300000000000004%" headers="mcps1.2.4.1.3 "><p id="p1190775544911"><a name="p1190775544911"></a><a name="p1190775544911"></a>设备Token</p>
    </td>
    </tr>
    <tr id="row2026012218470"><td class="cellrowborder" valign="top" width="34.33%" headers="mcps1.2.4.1.1 "><p id="p9907185512496"><a name="p9907185512496"></a><a name="p9907185512496"></a>user_data</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.369999999999997%" headers="mcps1.2.4.1.2 "><p id="p20907175511495"><a name="p20907175511495"></a><a name="p20907175511495"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.300000000000004%" headers="mcps1.2.4.1.3 "><p id="p11907145544910"><a name="p11907145544910"></a><a name="p11907145544910"></a>用户数据</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "request_id": "0e1bf654b29f56d297eca7c9502a96ba", 
        "attributes": 
            {
                "enabled": "true", 
                "token": "3708232124742383445",
                "user_data": "abc"
            }
    }
    ```


## 返回值<a name="section242171292113"></a>

请参考[返回值](返回值.md)。

## 错误码<a name="section73211020122511"></a>

请参考[错误码说明](错误码说明.md)。

