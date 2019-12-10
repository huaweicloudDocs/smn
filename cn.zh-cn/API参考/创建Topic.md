# 创建Topic<a name="ZH-CN_TOPIC_0036017300"></a>

## 功能介绍<a name="section9931723184157"></a>

-   接口名称

    CreateTopic


-   功能描述

    创建Topic，单用户默认配额为3000。高并发场景下，可能会出现Topic数量超过3000仍创建成功的情况，此为正常现象。

    接口是幂等的，接口调用返回成功时，若已存在同名的Topic，返回的status code为200，否则返回的status code为201。


## URI<a name="section59578064184157"></a>

-   URI格式

    POST /v2/\{project\_id\}/notifications/topics


-   参数说明

    <a name="table29213141184157"></a>
    <table><thead align="left"><tr id="row19251397184157"><th class="cellrowborder" valign="top" width="18.3%" id="mcps1.1.5.1.1"><p id="p15859347184157"><a name="p15859347184157"></a><a name="p15859347184157"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="16.07%" id="mcps1.1.5.1.2"><p id="p9538705184157"><a name="p9538705184157"></a><a name="p9538705184157"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="24.83%" id="mcps1.1.5.1.3"><p id="p34437607184157"><a name="p34437607184157"></a><a name="p34437607184157"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="40.8%" id="mcps1.1.5.1.4"><p id="p37982782184157"><a name="p37982782184157"></a><a name="p37982782184157"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row29823245184157"><td class="cellrowborder" valign="top" width="18.3%" headers="mcps1.1.5.1.1 "><p id="p66872662184157"><a name="p66872662184157"></a><a name="p66872662184157"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.07%" headers="mcps1.1.5.1.2 "><p id="p47976511184157"><a name="p47976511184157"></a><a name="p47976511184157"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.83%" headers="mcps1.1.5.1.3 "><p id="p60892144184157"><a name="p60892144184157"></a><a name="p60892144184157"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.8%" headers="mcps1.1.5.1.4 "><p id="p59334239154910"><a name="p59334239154910"></a><a name="p59334239154910"></a>项目ID</p>
    <p id="p33316626184157"><a name="p33316626184157"></a><a name="p33316626184157"></a>获取项目ID请参考<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="section16815303184157"></a>

-   参数说明

    <a name="table65343646184157"></a>
    <table><thead align="left"><tr id="row24199091184157"><th class="cellrowborder" valign="top" width="21.10788921107889%" id="mcps1.1.5.1.1"><p id="p13969361184157"><a name="p13969361184157"></a><a name="p13969361184157"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="23.897610238976103%" id="mcps1.1.5.1.2"><p id="p57776496184157"><a name="p57776496184157"></a><a name="p57776496184157"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.377762223777623%" id="mcps1.1.5.1.3"><p id="p49384632184157"><a name="p49384632184157"></a><a name="p49384632184157"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="32.61673832616738%" id="mcps1.1.5.1.4"><p id="p40732240184157"><a name="p40732240184157"></a><a name="p40732240184157"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row16731537184157"><td class="cellrowborder" valign="top" width="21.10788921107889%" headers="mcps1.1.5.1.1 "><p id="p13077258184157"><a name="p13077258184157"></a><a name="p13077258184157"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.897610238976103%" headers="mcps1.1.5.1.2 "><p id="p52625012184157"><a name="p52625012184157"></a><a name="p52625012184157"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.377762223777623%" headers="mcps1.1.5.1.3 "><p id="p44473009184157"><a name="p44473009184157"></a><a name="p44473009184157"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.61673832616738%" headers="mcps1.1.5.1.4 "><p id="p45543947184157"><a name="p45543947184157"></a><a name="p45543947184157"></a>创建topic的名字。</p>
    <p id="p979550192113"><a name="p979550192113"></a><a name="p979550192113"></a>Topic名称只能包含大写字母、小写字母、数字、-和_，且必须由大写字母、小写字母或数字开头，长度为1到255个字符。</p>
    </td>
    </tr>
    <tr id="row49758753184157"><td class="cellrowborder" valign="top" width="21.10788921107889%" headers="mcps1.1.5.1.1 "><p id="p3927189184157"><a name="p3927189184157"></a><a name="p3927189184157"></a>display_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.897610238976103%" headers="mcps1.1.5.1.2 "><p id="p49666922184157"><a name="p49666922184157"></a><a name="p49666922184157"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.377762223777623%" headers="mcps1.1.5.1.3 "><p id="p35509001184157"><a name="p35509001184157"></a><a name="p35509001184157"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.61673832616738%" headers="mcps1.1.5.1.4 "><p id="p6330530816482"><a name="p6330530816482"></a><a name="p6330530816482"></a>Topic的显示名，推送邮件消息时，作为邮件发件人显示。</p>
    <p id="p11282828192211"><a name="p11282828192211"></a><a name="p11282828192211"></a>显示名的长度为192byte或64个中文。</p>
    <p id="p7371996273"><a name="p7371996273"></a><a name="p7371996273"></a>默认值为空。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   请求样例

    ```
    POST https://{SMN_Endpoint}/v2/{project_id}/notifications/topics
    ```

    ```
    {
        "name": "test_topic_v2",
        "display_name": "testtest"
    }
    ```


## 响应消息<a name="section26706597184157"></a>

-   要素说明

    <a name="table741793184157"></a>
    <table><thead align="left"><tr id="row65023299184157"><th class="cellrowborder" valign="top" width="21.13%" id="mcps1.1.4.1.1"><p id="p32395875184157"><a name="p32395875184157"></a><a name="p32395875184157"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="24.6%" id="mcps1.1.4.1.2"><p id="p6820199184157"><a name="p6820199184157"></a><a name="p6820199184157"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="54.269999999999996%" id="mcps1.1.4.1.3"><p id="p15565240184157"><a name="p15565240184157"></a><a name="p15565240184157"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row50957918184157"><td class="cellrowborder" valign="top" width="21.13%" headers="mcps1.1.4.1.1 "><p id="p33950725184157"><a name="p33950725184157"></a><a name="p33950725184157"></a>request_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.6%" headers="mcps1.1.4.1.2 "><p id="p65654167184157"><a name="p65654167184157"></a><a name="p65654167184157"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="54.269999999999996%" headers="mcps1.1.4.1.3 "><p id="p16387326184157"><a name="p16387326184157"></a><a name="p16387326184157"></a>请求的唯一标识ID</p>
    </td>
    </tr>
    <tr id="row983478184157"><td class="cellrowborder" valign="top" width="21.13%" headers="mcps1.1.4.1.1 "><p id="p12552895184157"><a name="p12552895184157"></a><a name="p12552895184157"></a>topic_urn</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.6%" headers="mcps1.1.4.1.2 "><p id="p10151609184157"><a name="p10151609184157"></a><a name="p10151609184157"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="54.269999999999996%" headers="mcps1.1.4.1.3 "><p id="p16974028184157"><a name="p16974028184157"></a><a name="p16974028184157"></a>Topic的唯一的资源标识，可通过<a href="查询Topic列表.md">查询Topic列表</a>获取该标识。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   响应样例

    ```
    {
        "request_id": "6a63a18b8bab40ffb71ebd9cb80d0085",
        "topic_urn": "urn:smn:regionId:f96188c7ccaf4ffba0c9aa149ab2bd57:test_topic_v2"
    }
    ```


## 返回值<a name="section15080701184157"></a>

请参考[返回值](返回值.md)。

## 错误码<a name="section73211020122511"></a>

请参考[错误码说明](错误码说明.md)。

