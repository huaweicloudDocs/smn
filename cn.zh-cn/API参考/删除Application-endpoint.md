# 删除Application endpoint<a name="smn_api_58003"></a>

## 功能介绍<a name="zh-cn_topic_0118694308_section24495972"></a>

-   接口名称

    DeleteApplicationEndpoint

-   功能描述

    删除设备。


## URI<a name="zh-cn_topic_0118694308_section19137160"></a>

-   URI格式

    DELETE /v2/\{project\_id\}/notifications/endpoints/\{endpoint\_urn\}

-   参数说明

    <a name="zh-cn_topic_0118694308_table4609929"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0118694308_row10805765"><th class="cellrowborder" valign="top" width="20.990000000000002%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0118694308_p2851790"><a name="zh-cn_topic_0118694308_p2851790"></a><a name="zh-cn_topic_0118694308_p2851790"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.75%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0118694308_p29668407"><a name="zh-cn_topic_0118694308_p29668407"></a><a name="zh-cn_topic_0118694308_p29668407"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="20.990000000000002%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0118694308_p54330728"><a name="zh-cn_topic_0118694308_p54330728"></a><a name="zh-cn_topic_0118694308_p54330728"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="38.269999999999996%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0118694308_p38712842"><a name="zh-cn_topic_0118694308_p38712842"></a><a name="zh-cn_topic_0118694308_p38712842"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0118694308_row55017151"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0118694308_p27204259"><a name="zh-cn_topic_0118694308_p27204259"></a><a name="zh-cn_topic_0118694308_p27204259"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.75%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0118694308_p56061334"><a name="zh-cn_topic_0118694308_p56061334"></a><a name="zh-cn_topic_0118694308_p56061334"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0118694308_p44674243"><a name="zh-cn_topic_0118694308_p44674243"></a><a name="zh-cn_topic_0118694308_p44674243"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.269999999999996%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0118694308_p61843920"><a name="zh-cn_topic_0118694308_p61843920"></a><a name="zh-cn_topic_0118694308_p61843920"></a>项目ID</p>
    <p id="zh-cn_topic_0118694308_p19724370"><a name="zh-cn_topic_0118694308_p19724370"></a><a name="zh-cn_topic_0118694308_p19724370"></a>获取项目ID请参考<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0118694308_row25704456"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0118694308_p1686169"><a name="zh-cn_topic_0118694308_p1686169"></a><a name="zh-cn_topic_0118694308_p1686169"></a>endpoint_urn</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.75%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0118694308_p2362032"><a name="zh-cn_topic_0118694308_p2362032"></a><a name="zh-cn_topic_0118694308_p2362032"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0118694308_p57106866"><a name="zh-cn_topic_0118694308_p57106866"></a><a name="zh-cn_topic_0118694308_p57106866"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.269999999999996%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0118694308_p62253449"><a name="zh-cn_topic_0118694308_p62253449"></a><a name="zh-cn_topic_0118694308_p62253449"></a>Endpoint的唯一资源标识，可通过<a href="查询Application的Endpoint列表.md">查询Application的Endpoint列表</a>获取该标识。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="zh-cn_topic_0118694308_section38016717"></a>

-   请求样例

    ```
    DELETE https://{SMN_Endpoint}/v2/{project_id}/notifications/endpoints/{endpoint_urn}
    ```


## 响应消息<a name="zh-cn_topic_0118694308_section6606141"></a>

-   要素说明

    <a name="zh-cn_topic_0118694308_table31562473"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0118694308_row1437453"><th class="cellrowborder" valign="top" width="29.872987298729875%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0118694308_p49324898"><a name="zh-cn_topic_0118694308_p49324898"></a><a name="zh-cn_topic_0118694308_p49324898"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="35.063506350635066%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0118694308_p35893824"><a name="zh-cn_topic_0118694308_p35893824"></a><a name="zh-cn_topic_0118694308_p35893824"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="35.063506350635066%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0118694308_p21718606"><a name="zh-cn_topic_0118694308_p21718606"></a><a name="zh-cn_topic_0118694308_p21718606"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0118694308_row23656219"><td class="cellrowborder" valign="top" width="29.872987298729875%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0118694308_p37105578"><a name="zh-cn_topic_0118694308_p37105578"></a><a name="zh-cn_topic_0118694308_p37105578"></a>request_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0118694308_p52761866"><a name="zh-cn_topic_0118694308_p52761866"></a><a name="zh-cn_topic_0118694308_p52761866"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0118694308_p45852771"><a name="zh-cn_topic_0118694308_p45852771"></a><a name="zh-cn_topic_0118694308_p45852771"></a>请求的唯一标识ID</p>
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

