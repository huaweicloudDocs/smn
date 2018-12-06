# 查询Topic列表<a name="ZH-CN_TOPIC_0036016755"></a>

## 功能介绍<a name="zh-cn_topic_0025373767-chtext"></a>

-   接口名称

    ListTopics


-   功能描述

    分页查询主题列表，主题列表按照主题创建时间进行降序排列。分页查询可以指定offset以及limit。如果不存在主题，则返回空列表。


## URI<a name="section30715040"></a>

-   URI格式

    GET /v2/\{project\_id\}/notifications/topics?offset=0&limit=2


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
    <p id="p22717550"><a name="p22717550"></a><a name="p22717550"></a>获取项目ID请参考<a href="获取项目编号.md">获取项目编号</a>。</p>
    </td>
    </tr>
    <tr id="row52313669"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.1 "><p id="p9548790"><a name="p9548790"></a><a name="p9548790"></a>offset</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.2 "><p id="p2088631120211"><a name="p2088631120211"></a><a name="p2088631120211"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.650000000000002%" headers="mcps1.1.5.1.3 "><p id="p37041500"><a name="p37041500"></a><a name="p37041500"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.35%" headers="mcps1.1.5.1.4 "><p id="p47571555"><a name="p47571555"></a><a name="p47571555"></a>分页列表的起始页，默认值为0。offset的必须大于等于0。</p>
    </td>
    </tr>
    <tr id="row51489795"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.1 "><p id="p9923843"><a name="p9923843"></a><a name="p9923843"></a>limit</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.2 "><p id="p65633828"><a name="p65633828"></a><a name="p65633828"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.650000000000002%" headers="mcps1.1.5.1.3 "><p id="p14739853"><a name="p14739853"></a><a name="p14739853"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.35%" headers="mcps1.1.5.1.4 "><p id="p53077479"><a name="p53077479"></a><a name="p53077479"></a>一次返回列表的最大条目数 。默认值为100。</p>
    <p id="p12553656275"><a name="p12553656275"></a><a name="p12553656275"></a>limit的值必须大于0且不大于100。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求<a name="section7999906"></a>

请求样例

```
GET /v2/{project_id}/notifications/topics?offset=0&limit=100
```

## 响应<a name="section4890297"></a>

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
    <td class="cellrowborder" valign="top" width="36.82%" headers="mcps1.1.4.1.3 "><p id="p20038698"><a name="p20038698"></a><a name="p20038698"></a>请求的唯一标示ID。</p>
    </td>
    </tr>
    <tr id="row45587811"><td class="cellrowborder" valign="top" width="31.59%" headers="mcps1.1.4.1.1 "><p id="p1625174"><a name="p1625174"></a><a name="p1625174"></a>topic_count</p>
    </td>
    <td class="cellrowborder" valign="top" width="31.59%" headers="mcps1.1.4.1.2 "><p id="p64530307"><a name="p64530307"></a><a name="p64530307"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.82%" headers="mcps1.1.4.1.3 "><p id="p59572368"><a name="p59572368"></a><a name="p59572368"></a>返回的Topic个数。</p>
    </td>
    </tr>
    <tr id="row8821459"><td class="cellrowborder" valign="top" width="31.59%" headers="mcps1.1.4.1.1 "><p id="p43449544"><a name="p43449544"></a><a name="p43449544"></a>topics</p>
    </td>
    <td class="cellrowborder" valign="top" width="31.59%" headers="mcps1.1.4.1.2 "><p id="p29752153"><a name="p29752153"></a><a name="p29752153"></a>Topic结构体数组</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.82%" headers="mcps1.1.4.1.3 "><p id="p61114224"><a name="p61114224"></a><a name="p61114224"></a>请参见<a href="Topic结构体.md">Topic结构体</a>。</p>
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

