# 查询Topic详情<a name="ZH-CN_TOPIC_0036016756"></a>

## 功能介绍<a name="section64935954"></a>

-   接口名称

    QueryTopicDetail


-   功能描述

    查询Topic的详细信息。


## URI<a name="section47552675"></a>

-   URI格式

    GET /v2/\{project\_id\}/notifications/topics/\{topic\_urn\}


-   参数说明

    <a name="table60453091"></a>
    <table><thead align="left"><tr id="row31471768"><th class="cellrowborder" valign="top" width="23.82238223822382%" id="mcps1.1.5.1.1"><p id="p66185246"><a name="p66185246"></a><a name="p66185246"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.942194219421943%" id="mcps1.1.5.1.2"><p id="p59404709"><a name="p59404709"></a><a name="p59404709"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.012101210121013%" id="mcps1.1.5.1.3"><p id="p47052116"><a name="p47052116"></a><a name="p47052116"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.223322332233224%" id="mcps1.1.5.1.4"><p id="p53125076"><a name="p53125076"></a><a name="p53125076"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row57297510"><td class="cellrowborder" valign="top" width="23.82238223822382%" headers="mcps1.1.5.1.1 "><p id="p10586695"><a name="p10586695"></a><a name="p10586695"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.942194219421943%" headers="mcps1.1.5.1.2 "><p id="p52215961"><a name="p52215961"></a><a name="p52215961"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.012101210121013%" headers="mcps1.1.5.1.3 "><p id="p1634435"><a name="p1634435"></a><a name="p1634435"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.223322332233224%" headers="mcps1.1.5.1.4 "><p id="p61977638154952"><a name="p61977638154952"></a><a name="p61977638154952"></a>项目ID</p>
    <p id="p65280430"><a name="p65280430"></a><a name="p65280430"></a>获取项目ID请参考<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    <tr id="row9249362"><td class="cellrowborder" valign="top" width="23.82238223822382%" headers="mcps1.1.5.1.1 "><p id="p11000853"><a name="p11000853"></a><a name="p11000853"></a>topic_urn</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.942194219421943%" headers="mcps1.1.5.1.2 "><p id="p18653909"><a name="p18653909"></a><a name="p18653909"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.012101210121013%" headers="mcps1.1.5.1.3 "><p id="p34571641"><a name="p34571641"></a><a name="p34571641"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.223322332233224%" headers="mcps1.1.5.1.4 "><p id="p48839530"><a name="p48839530"></a><a name="p48839530"></a>Topic的唯一的资源标识。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求<a name="section25320898"></a>

请求样例

```
GET /v2/{project_id}/notifications/topics/urn:smn:regionId:8bad8a40e0f7462f8c1676e3f93a8183:test_create_topic_v2
```

## 响应<a name="section26561495"></a>

-   要素说明

    <a name="table38552084"></a>
    <table><thead align="left"><tr id="row10058158"><th class="cellrowborder" valign="top" width="25.81%" id="mcps1.1.4.1.1"><p id="p9404449"><a name="p9404449"></a><a name="p9404449"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.07%" id="mcps1.1.4.1.2"><p id="p23562876"><a name="p23562876"></a><a name="p23562876"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="52.12%" id="mcps1.1.4.1.3"><p id="p29544808"><a name="p29544808"></a><a name="p29544808"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row33089041"><td class="cellrowborder" valign="top" width="25.81%" headers="mcps1.1.4.1.1 "><p id="p62966687"><a name="p62966687"></a><a name="p62966687"></a>request_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.07%" headers="mcps1.1.4.1.2 "><p id="p27997"><a name="p27997"></a><a name="p27997"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="52.12%" headers="mcps1.1.4.1.3 "><p id="p2267763"><a name="p2267763"></a><a name="p2267763"></a>请求的唯一标示ID。</p>
    </td>
    </tr>
    <tr id="row42586845"><td class="cellrowborder" valign="top" width="25.81%" headers="mcps1.1.4.1.1 "><p id="p26982424"><a name="p26982424"></a><a name="p26982424"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.07%" headers="mcps1.1.4.1.2 "><p id="p38092711"><a name="p38092711"></a><a name="p38092711"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="52.12%" headers="mcps1.1.4.1.3 "><p id="p65610739"><a name="p65610739"></a><a name="p65610739"></a>创建Topic的名字。</p>
    </td>
    </tr>
    <tr id="row48717564"><td class="cellrowborder" valign="top" width="25.81%" headers="mcps1.1.4.1.1 "><p id="p53808606"><a name="p53808606"></a><a name="p53808606"></a>topic_urn</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.07%" headers="mcps1.1.4.1.2 "><p id="p63529816"><a name="p63529816"></a><a name="p63529816"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="52.12%" headers="mcps1.1.4.1.3 "><p id="p45641491"><a name="p45641491"></a><a name="p45641491"></a>Topic的唯一的资源标识。</p>
    </td>
    </tr>
    <tr id="row53759727"><td class="cellrowborder" valign="top" width="25.81%" headers="mcps1.1.4.1.1 "><p id="p59570626"><a name="p59570626"></a><a name="p59570626"></a>display_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.07%" headers="mcps1.1.4.1.2 "><p id="p60491410"><a name="p60491410"></a><a name="p60491410"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="52.12%" headers="mcps1.1.4.1.3 "><p id="p57656838184157"><a name="p57656838184157"></a><a name="p57656838184157"></a>Topic的别名，推送邮件消息时，作为邮件发件人显示。</p>
    </td>
    </tr>
    <tr id="row20888703"><td class="cellrowborder" valign="top" width="25.81%" headers="mcps1.1.4.1.1 "><p id="p14263389"><a name="p14263389"></a><a name="p14263389"></a>push_policy</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.07%" headers="mcps1.1.4.1.2 "><p id="p14483900"><a name="p14483900"></a><a name="p14483900"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="52.12%" headers="mcps1.1.4.1.3 "><p id="p32345284"><a name="p32345284"></a><a name="p32345284"></a>消息推送的策略。</p>
    <p id="p10916523273"><a name="p10916523273"></a><a name="p10916523273"></a>0表示发送失败，保留到失败队列，1表示直接丢弃发送失败的消息。</p>
    </td>
    </tr>
    <tr id="row24500989"><td class="cellrowborder" valign="top" width="25.81%" headers="mcps1.1.4.1.1 "><p id="p38423121"><a name="p38423121"></a><a name="p38423121"></a>create_time</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.07%" headers="mcps1.1.4.1.2 "><p id="p25265097"><a name="p25265097"></a><a name="p25265097"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="52.12%" headers="mcps1.1.4.1.3 "><p id="p33206990"><a name="p33206990"></a><a name="p33206990"></a>创建时间。</p>
    <p id="p12947570279"><a name="p12947570279"></a><a name="p12947570279"></a>时间格式为UTC时间。</p>
    </td>
    </tr>
    <tr id="row48704899"><td class="cellrowborder" valign="top" width="25.81%" headers="mcps1.1.4.1.1 "><p id="p52782726"><a name="p52782726"></a><a name="p52782726"></a>update_time</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.07%" headers="mcps1.1.4.1.2 "><p id="p47542385"><a name="p47542385"></a><a name="p47542385"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="52.12%" headers="mcps1.1.4.1.3 "><p id="p25727981"><a name="p25727981"></a><a name="p25727981"></a>更新时间。</p>
    <p id="p15544215281"><a name="p15544215281"></a><a name="p15544215281"></a>时间格式为UTC时间。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "update_time":"2016-08-01T02:16:38Z",
        "push_policy":0,
        "create_time":"2016-08-01T02:16:38Z",
        "name":"test_create_topic_v2",
        "topic_urn":"urn:smn:regionId:8bad8a40e0f7462f8c1676e3f93a8183:test_create_topic_v2",
        "display_name":"test create topic v2",
        "request_id":"6837531fd3f54550927b930180a706bf"
    }
    ```


## 返回值<a name="section37726867"></a>

请参考[返回值](返回值.md)。

## 错误码<a name="section73211020122511"></a>

请参考[错误码说明](错误码说明.md)。

