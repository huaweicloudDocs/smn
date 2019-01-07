# 删除指定名称的Topic属性<a name="ZH-CN_TOPIC_0038364129"></a>

## 功能介绍<a name="section64935954"></a>

-   接口名称

    DeleteTopicAttributeByName


-   功能描述

    删除指定名称的Topic属性。


## URI<a name="section47552675"></a>

-   URI格式

    DELETE /v2/\{project\_id\}/notifications/topics/\{topic\_urn\}/attributes/\{name\}


-   参数说明

    <a name="table60453091"></a>
    <table><thead align="left"><tr id="row31471768"><th class="cellrowborder" valign="top" width="21.46%" id="mcps1.1.5.1.1"><p id="p66185246"><a name="p66185246"></a><a name="p66185246"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.7%" id="mcps1.1.5.1.2"><p id="p59404709"><a name="p59404709"></a><a name="p59404709"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="24.310000000000002%" id="mcps1.1.5.1.3"><p id="p47052116"><a name="p47052116"></a><a name="p47052116"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="31.53%" id="mcps1.1.5.1.4"><p id="p53125076"><a name="p53125076"></a><a name="p53125076"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row57297510"><td class="cellrowborder" valign="top" width="21.46%" headers="mcps1.1.5.1.1 "><p id="p10586695"><a name="p10586695"></a><a name="p10586695"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.7%" headers="mcps1.1.5.1.2 "><p id="p52215961"><a name="p52215961"></a><a name="p52215961"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.310000000000002%" headers="mcps1.1.5.1.3 "><p id="p1634435"><a name="p1634435"></a><a name="p1634435"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="31.53%" headers="mcps1.1.5.1.4 "><p id="p35765041155042"><a name="p35765041155042"></a><a name="p35765041155042"></a>项目ID</p>
    <p id="p65280430"><a name="p65280430"></a><a name="p65280430"></a>获取项目ID请参考<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    <tr id="row9249362"><td class="cellrowborder" valign="top" width="21.46%" headers="mcps1.1.5.1.1 "><p id="p11000853"><a name="p11000853"></a><a name="p11000853"></a>topic_urn</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.7%" headers="mcps1.1.5.1.2 "><p id="p18653909"><a name="p18653909"></a><a name="p18653909"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.310000000000002%" headers="mcps1.1.5.1.3 "><p id="p34571641"><a name="p34571641"></a><a name="p34571641"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="31.53%" headers="mcps1.1.5.1.4 "><p id="p48839530"><a name="p48839530"></a><a name="p48839530"></a>Topic的唯一的资源标识。</p>
    </td>
    </tr>
    <tr id="row5965394515386"><td class="cellrowborder" valign="top" width="21.46%" headers="mcps1.1.5.1.1 "><p id="p14783623153811"><a name="p14783623153811"></a><a name="p14783623153811"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.7%" headers="mcps1.1.5.1.2 "><p id="p56622849153811"><a name="p56622849153811"></a><a name="p56622849153811"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.310000000000002%" headers="mcps1.1.5.1.3 "><p id="p23048084153811"><a name="p23048084153811"></a><a name="p23048084153811"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="31.53%" headers="mcps1.1.5.1.4 "><p id="p54955495153811"><a name="p54955495153811"></a><a name="p54955495153811"></a>属性名称。</p>
    <p id="p2749131513324"><a name="p2749131513324"></a><a name="p2749131513324"></a>只支持特定的属性名称，请参见<a href="Topic属性表.md">Topic属性表</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求<a name="section25320898"></a>

请求样例

```
DELETE /v2/{project_id}/notifications/topics/{topic_urn}/attributes/access_policy
```

## 响应<a name="section26561495"></a>

-   要素说明

    <a name="table38552084"></a>
    <table><thead align="left"><tr id="row10058158"><th class="cellrowborder" valign="top" width="32.12678732126787%" id="mcps1.1.4.1.1"><p id="p9404449"><a name="p9404449"></a><a name="p9404449"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="32.12678732126787%" id="mcps1.1.4.1.2"><p id="p23562876"><a name="p23562876"></a><a name="p23562876"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="35.746425357464254%" id="mcps1.1.4.1.3"><p id="p29544808"><a name="p29544808"></a><a name="p29544808"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row33089041"><td class="cellrowborder" valign="top" width="32.12678732126787%" headers="mcps1.1.4.1.1 "><p id="p62966687"><a name="p62966687"></a><a name="p62966687"></a>request_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.12678732126787%" headers="mcps1.1.4.1.2 "><p id="p27997"><a name="p27997"></a><a name="p27997"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.746425357464254%" headers="mcps1.1.4.1.3 "><p id="p2267763"><a name="p2267763"></a><a name="p2267763"></a>请求的唯一标示ID。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "request_id":"6837531fd3f54550927b930180a706bf"
    }
    ```


## 返回值<a name="section37726867"></a>

请参考[返回值](返回值.md)。

## 错误码<a name="section73211020122511"></a>

请参考[错误码说明](错误码说明.md)。

