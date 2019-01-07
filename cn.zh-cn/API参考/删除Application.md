# 删除Application<a name="ZH-CN_TOPIC_0118712460"></a>

## 功能介绍<a name="zh-cn_topic_0118694337_section64534832"></a>

-   接口名称

    DeleteApplication

-   功能描述

    删除平台应用。


## URI<a name="zh-cn_topic_0118694337_section43942582"></a>

-   URI格式

    DELETE /v2/\{project\_id\}/notifications/applications/\{application\_urn\}

-   参数说明

    <a name="zh-cn_topic_0118694337_table58711356"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0118694337_row35358604"><th class="cellrowborder" valign="top" width="20.990000000000002%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0118694337_p45474671"><a name="zh-cn_topic_0118694337_p45474671"></a><a name="zh-cn_topic_0118694337_p45474671"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.75%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0118694337_p59569743"><a name="zh-cn_topic_0118694337_p59569743"></a><a name="zh-cn_topic_0118694337_p59569743"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="20.990000000000002%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0118694337_p60419859"><a name="zh-cn_topic_0118694337_p60419859"></a><a name="zh-cn_topic_0118694337_p60419859"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="38.269999999999996%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0118694337_p62170404"><a name="zh-cn_topic_0118694337_p62170404"></a><a name="zh-cn_topic_0118694337_p62170404"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0118694337_row12345674"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0118694337_p60475569"><a name="zh-cn_topic_0118694337_p60475569"></a><a name="zh-cn_topic_0118694337_p60475569"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.75%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0118694337_p66682883"><a name="zh-cn_topic_0118694337_p66682883"></a><a name="zh-cn_topic_0118694337_p66682883"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0118694337_p32604458"><a name="zh-cn_topic_0118694337_p32604458"></a><a name="zh-cn_topic_0118694337_p32604458"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.269999999999996%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0118694337_p23715470"><a name="zh-cn_topic_0118694337_p23715470"></a><a name="zh-cn_topic_0118694337_p23715470"></a>项目ID</p>
    <p id="zh-cn_topic_0118694337_p12112642"><a name="zh-cn_topic_0118694337_p12112642"></a><a name="zh-cn_topic_0118694337_p12112642"></a>获取项目ID请参考<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0118694337_row14152581"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0118694337_p5508440"><a name="zh-cn_topic_0118694337_p5508440"></a><a name="zh-cn_topic_0118694337_p5508440"></a>application_urn</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.75%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0118694337_p43530475"><a name="zh-cn_topic_0118694337_p43530475"></a><a name="zh-cn_topic_0118694337_p43530475"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0118694337_p36307558"><a name="zh-cn_topic_0118694337_p36307558"></a><a name="zh-cn_topic_0118694337_p36307558"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.269999999999996%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0118694337_p55231090"><a name="zh-cn_topic_0118694337_p55231090"></a><a name="zh-cn_topic_0118694337_p55231090"></a>Application的唯一资源标示</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求<a name="zh-cn_topic_0118694337_section59938924"></a>

-   请求样例

    ```
    DELETE /v2/{project_id}/notifications/applications/{application_urn}
    ```


## 响应<a name="zh-cn_topic_0118694337_section2579412"></a>

-   要素说明

    <a name="zh-cn_topic_0118694337_table47591197"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0118694337_row62468609"><th class="cellrowborder" valign="top" width="29.872987298729875%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0118694337_p26792557"><a name="zh-cn_topic_0118694337_p26792557"></a><a name="zh-cn_topic_0118694337_p26792557"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="35.063506350635066%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0118694337_p22713469"><a name="zh-cn_topic_0118694337_p22713469"></a><a name="zh-cn_topic_0118694337_p22713469"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="35.063506350635066%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0118694337_p27851673"><a name="zh-cn_topic_0118694337_p27851673"></a><a name="zh-cn_topic_0118694337_p27851673"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0118694337_row64504088"><td class="cellrowborder" valign="top" width="29.872987298729875%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0118694337_p57448650"><a name="zh-cn_topic_0118694337_p57448650"></a><a name="zh-cn_topic_0118694337_p57448650"></a>request_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0118694337_p22829097"><a name="zh-cn_topic_0118694337_p22829097"></a><a name="zh-cn_topic_0118694337_p22829097"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0118694337_p37217564"><a name="zh-cn_topic_0118694337_p37217564"></a><a name="zh-cn_topic_0118694337_p37217564"></a>请求的唯一标示ID</p>
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

