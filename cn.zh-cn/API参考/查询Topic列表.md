# 查询Topic列表<a name="ZH-CN_TOPIC_0036016755"></a>

## 功能介绍<a name="zh-cn_topic_0025373767-chtext"></a>

-   接口名称

    ListTopics


-   功能描述

    分页查询Topic列表，Topic列表按照Topic创建时间进行降序排列。分页查询可以指定offset以及limit。如果不存在Topic，则返回空列表。


## URI<a name="section30715040"></a>

-   URI格式

    GET /v2/\{project\_id\}/notifications/topics?offset=\{offset\}&limit=\{limit\}


-   参数说明

    <a name="table65858198"></a>
    <table><thead align="left"><tr id="row16627584"><th class="cellrowborder" valign="top" width="25%" id="mcps1.1.5.1.1"><p id="p4657088"><a name="p4657088"></a><a name="p4657088"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="25%" id="mcps1.1.5.1.2"><p id="p41679865"><a name="p41679865"></a><a name="p41679865"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.650000000000002%" id="mcps1.1.5.1.3"><p id="p20625874"><a name="p20625874"></a><a name="p20625874"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="27.35%" id="mcps1.1.5.1.4"><p id="p60083059"><a name="p60083059"></a><a name="p60083059"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row7485743"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.1 "><p id="p2365466"><a name="p2365466"></a><a name="p2365466"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.2 "><p id="p57385070"><a name="p57385070"></a><a name="p57385070"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.650000000000002%" headers="mcps1.1.5.1.3 "><p id="p17679057"><a name="p17679057"></a><a name="p17679057"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.35%" headers="mcps1.1.5.1.4 "><p id="p12240680154940"><a name="p12240680154940"></a><a name="p12240680154940"></a>项目ID</p>
    <p id="p22717550"><a name="p22717550"></a><a name="p22717550"></a>获取项目ID请参考<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    <tr id="row52313669"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.1 "><p id="p9548790"><a name="p9548790"></a><a name="p9548790"></a>offset</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.2 "><p id="p2088631120211"><a name="p2088631120211"></a><a name="p2088631120211"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.650000000000002%" headers="mcps1.1.5.1.3 "><p id="p37041500"><a name="p37041500"></a><a name="p37041500"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.35%" headers="mcps1.1.5.1.4 "><p id="p146581828102110"><a name="p146581828102110"></a><a name="p146581828102110"></a>偏移量</p>
    <p id="p21821344207"><a name="p21821344207"></a><a name="p21821344207"></a>偏移量为一个大于0小于资源总个数的整数，表示查询该偏移量后面的所有的资源数，默认值为0。</p>
    </td>
    </tr>
    <tr id="row51489795"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.1 "><p id="p9923843"><a name="p9923843"></a><a name="p9923843"></a>limit</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.2 "><p id="p65633828"><a name="p65633828"></a><a name="p65633828"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.650000000000002%" headers="mcps1.1.5.1.3 "><p id="p14739853"><a name="p14739853"></a><a name="p14739853"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.35%" headers="mcps1.1.5.1.4 "><a name="ul38160342182720"></a><a name="ul38160342182720"></a><ul id="ul38160342182720"><li>取值范围：1~100<p id="p3980022182720"><a name="p3980022182720"></a><a name="p3980022182720"></a>取值一般为10，20，50</p>
    </li><li>功能说明：每页返回的资源个数。</li></ul>
    <p id="p5184153012911"><a name="p5184153012911"></a><a name="p5184153012911"></a>默认值为100。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="section7999906"></a>

请求样例

```
GET https://{SMN_Endpoint}/v2/{project_id}/notifications/topics?offset=0&limit=100
```

## 响应消息<a name="section4890297"></a>

-   要素说明

    <a name="table32894845"></a>
    <table><thead align="left"><tr id="row40748571"><th class="cellrowborder" valign="top" width="31.59%" id="mcps1.1.4.1.1"><p id="p12299945"><a name="p12299945"></a><a name="p12299945"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="31.59%" id="mcps1.1.4.1.2"><p id="p56771492"><a name="p56771492"></a><a name="p56771492"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="36.82%" id="mcps1.1.4.1.3"><p id="p35088115"><a name="p35088115"></a><a name="p35088115"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row29721263"><td class="cellrowborder" valign="top" width="31.59%" headers="mcps1.1.4.1.1 "><p id="p58612075"><a name="p58612075"></a><a name="p58612075"></a>request_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="31.59%" headers="mcps1.1.4.1.2 "><p id="p49957660"><a name="p49957660"></a><a name="p49957660"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.82%" headers="mcps1.1.4.1.3 "><p id="p20038698"><a name="p20038698"></a><a name="p20038698"></a>请求的唯一标识ID。</p>
    </td>
    </tr>
    <tr id="row45587811"><td class="cellrowborder" valign="top" width="31.59%" headers="mcps1.1.4.1.1 "><p id="p1625174"><a name="p1625174"></a><a name="p1625174"></a>topic_count</p>
    </td>
    <td class="cellrowborder" valign="top" width="31.59%" headers="mcps1.1.4.1.2 "><p id="p64530307"><a name="p64530307"></a><a name="p64530307"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.82%" headers="mcps1.1.4.1.3 "><p id="p59572368"><a name="p59572368"></a><a name="p59572368"></a>返回的Topic个数。</p>
    <div class="note" id="note48698383125"><a name="note48698383125"></a><a name="note48698383125"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p452954191219"><a name="p452954191219"></a><a name="p452954191219"></a>该参数不受offset和limit影响，即返回的是您账户下所有的Topic个数。</p>
    </div></div>
    </td>
    </tr>
    <tr id="row8821459"><td class="cellrowborder" valign="top" width="31.59%" headers="mcps1.1.4.1.1 "><p id="p43449544"><a name="p43449544"></a><a name="p43449544"></a>topics</p>
    </td>
    <td class="cellrowborder" valign="top" width="31.59%" headers="mcps1.1.4.1.2 "><p id="p29752153"><a name="p29752153"></a><a name="p29752153"></a>Topic结构体数组</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.82%" headers="mcps1.1.4.1.3 "><p id="p15409255121419"><a name="p15409255121419"></a><a name="p15409255121419"></a>Topic详细信息。</p>
    <p id="p61114224"><a name="p61114224"></a><a name="p61114224"></a>请参见<a href="#table10636317195533">表1</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 1**  Topic结构体

    <a name="table10636317195533"></a>
    <table><thead align="left"><tr id="row28583391195533"><th class="cellrowborder" valign="top" width="29.69%" id="mcps1.2.4.1.1"><p id="p33553343195533"><a name="p33553343195533"></a><a name="p33553343195533"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="28.050000000000004%" id="mcps1.2.4.1.2"><p id="p33466243195533"><a name="p33466243195533"></a><a name="p33466243195533"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="42.26%" id="mcps1.2.4.1.3"><p id="p26411156195533"><a name="p26411156195533"></a><a name="p26411156195533"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row8508090195533"><td class="cellrowborder" valign="top" width="29.69%" headers="mcps1.2.4.1.1 "><p id="p18066721195533"><a name="p18066721195533"></a><a name="p18066721195533"></a>topic_urn</p>
    </td>
    <td class="cellrowborder" valign="top" width="28.050000000000004%" headers="mcps1.2.4.1.2 "><p id="p54118259195533"><a name="p54118259195533"></a><a name="p54118259195533"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="42.26%" headers="mcps1.2.4.1.3 "><p id="p21502874195533"><a name="p21502874195533"></a><a name="p21502874195533"></a>Topic的唯一的资源标识</p>
    </td>
    </tr>
    <tr id="row39230450195533"><td class="cellrowborder" valign="top" width="29.69%" headers="mcps1.2.4.1.1 "><p id="p23549883195533"><a name="p23549883195533"></a><a name="p23549883195533"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="28.050000000000004%" headers="mcps1.2.4.1.2 "><p id="p28492405195533"><a name="p28492405195533"></a><a name="p28492405195533"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="42.26%" headers="mcps1.2.4.1.3 "><p id="p26183496195533"><a name="p26183496195533"></a><a name="p26183496195533"></a>创建topi的名字</p>
    </td>
    </tr>
    <tr id="row28851380195533"><td class="cellrowborder" valign="top" width="29.69%" headers="mcps1.2.4.1.1 "><p id="p55260426195533"><a name="p55260426195533"></a><a name="p55260426195533"></a>display_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="28.050000000000004%" headers="mcps1.2.4.1.2 "><p id="p46909558195533"><a name="p46909558195533"></a><a name="p46909558195533"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="42.26%" headers="mcps1.2.4.1.3 "><p id="p41577821195533"><a name="p41577821195533"></a><a name="p41577821195533"></a>Topic的显示名，推送邮件消息时，作为邮件发件人显示。</p>
    </td>
    </tr>
    <tr id="row44134393195533"><td class="cellrowborder" valign="top" width="29.69%" headers="mcps1.2.4.1.1 "><p id="p18116055195533"><a name="p18116055195533"></a><a name="p18116055195533"></a>push_policy</p>
    </td>
    <td class="cellrowborder" valign="top" width="28.050000000000004%" headers="mcps1.2.4.1.2 "><p id="p58114317195533"><a name="p58114317195533"></a><a name="p58114317195533"></a>Int</p>
    </td>
    <td class="cellrowborder" valign="top" width="42.26%" headers="mcps1.2.4.1.3 "><p id="p9639236195533"><a name="p9639236195533"></a><a name="p9639236195533"></a>消息推送的策略，该属性目前不支持修改，后续将支持修改。</p>
    <a name="ul10412105324519"></a><a name="ul10412105324519"></a><ul id="ul10412105324519"><li>0表示发送失败，保留到失败队列</li><li>1表示直接丢弃发送失败的消息</li></ul>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "request_id": "70bb40bef50e4a14b116a5a527fd7432", 
        "topic_count": 1, 
        "topics": [
            {
                "topic_urn": "urn:smn:regionId:8bad8a40e0f7462f8c1676e3f93a8183:test_topic_v2", 
                "display_name": "testtest", 
                "name": "test_topic_v1", 
                "push_policy": 0            
            }
        ]
    }
    ```


## 返回值<a name="section44012677"></a>

请参考[返回值](返回值.md)。

## 错误码<a name="section73211020122511"></a>

请参考[错误码说明](错误码说明.md)。

