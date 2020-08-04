# App消息发布<a name="smn_api_59001"></a>

## 功能介绍<a name="zh-cn_topic_0118694332_section46354700"></a>

-   接口名称

    PublishAppMessage

-   功能描述

    将消息直发给endpoint设备。


## URI<a name="zh-cn_topic_0118694332_section14539121"></a>

-   URI格式

    POST /v2/\{project\_id\}/notifications/endpoints/\{endpoint\_urn\}/publish

-   参数说明

    <a name="zh-cn_topic_0118694332_table21681426"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0118694332_row11404934"><th class="cellrowborder" valign="top" width="23.95%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0118694332_p51384442"><a name="zh-cn_topic_0118694332_p51384442"></a><a name="zh-cn_topic_0118694332_p51384442"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.53%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0118694332_p1390267"><a name="zh-cn_topic_0118694332_p1390267"></a><a name="zh-cn_topic_0118694332_p1390267"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.53%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0118694332_p45502768"><a name="zh-cn_topic_0118694332_p45502768"></a><a name="zh-cn_topic_0118694332_p45502768"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="30.990000000000002%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0118694332_p61845569"><a name="zh-cn_topic_0118694332_p61845569"></a><a name="zh-cn_topic_0118694332_p61845569"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0118694332_row28592218"><td class="cellrowborder" valign="top" width="23.95%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0118694332_p34268337"><a name="zh-cn_topic_0118694332_p34268337"></a><a name="zh-cn_topic_0118694332_p34268337"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.53%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0118694332_p24271941"><a name="zh-cn_topic_0118694332_p24271941"></a><a name="zh-cn_topic_0118694332_p24271941"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.53%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0118694332_p19870205"><a name="zh-cn_topic_0118694332_p19870205"></a><a name="zh-cn_topic_0118694332_p19870205"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.990000000000002%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0118694332_p65982786"><a name="zh-cn_topic_0118694332_p65982786"></a><a name="zh-cn_topic_0118694332_p65982786"></a>项目ID</p>
    <p id="zh-cn_topic_0118694332_p56974164"><a name="zh-cn_topic_0118694332_p56974164"></a><a name="zh-cn_topic_0118694332_p56974164"></a>获取项目ID请参考<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0118694332_row11122970"><td class="cellrowborder" valign="top" width="23.95%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0118694332_p28545349"><a name="zh-cn_topic_0118694332_p28545349"></a><a name="zh-cn_topic_0118694332_p28545349"></a>endpoint_urn</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.53%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0118694332_p30471937"><a name="zh-cn_topic_0118694332_p30471937"></a><a name="zh-cn_topic_0118694332_p30471937"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.53%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0118694332_p52307829"><a name="zh-cn_topic_0118694332_p52307829"></a><a name="zh-cn_topic_0118694332_p52307829"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.990000000000002%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0118694332_p9075786"><a name="zh-cn_topic_0118694332_p9075786"></a><a name="zh-cn_topic_0118694332_p9075786"></a>Endpoint的唯一资源标识，可通过<a href="查询Application的Endpoint列表.md">查询Application的Endpoint列表</a>获取该标识。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="zh-cn_topic_0118694332_section63743225"></a>

-   参数说明

    <a name="zh-cn_topic_0118694332_table64031004"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0118694332_row62473419"><th class="cellrowborder" valign="top" width="21.31213121312131%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0118694332_p27182148"><a name="zh-cn_topic_0118694332_p27182148"></a><a name="zh-cn_topic_0118694332_p27182148"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.31213121312131%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0118694332_p54270341"><a name="zh-cn_topic_0118694332_p54270341"></a><a name="zh-cn_topic_0118694332_p54270341"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.031803180318033%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0118694332_p33821495"><a name="zh-cn_topic_0118694332_p33821495"></a><a name="zh-cn_topic_0118694332_p33821495"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="39.34393439343935%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0118694332_p55186561"><a name="zh-cn_topic_0118694332_p55186561"></a><a name="zh-cn_topic_0118694332_p55186561"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0118694332_row26710272"><td class="cellrowborder" valign="top" width="21.31213121312131%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0118694332_p16048387"><a name="zh-cn_topic_0118694332_p16048387"></a><a name="zh-cn_topic_0118694332_p16048387"></a>message</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.31213121312131%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0118694332_p24851008"><a name="zh-cn_topic_0118694332_p24851008"></a><a name="zh-cn_topic_0118694332_p24851008"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.031803180318033%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0118694332_p66774621"><a name="zh-cn_topic_0118694332_p66774621"></a><a name="zh-cn_topic_0118694332_p66774621"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="39.34393439343935%" headers="mcps1.1.5.1.4 "><p id="p1097434819313"><a name="p1097434819313"></a><a name="p1097434819313"></a>app推送的消息内容，当前支持的推送平台有HMS、APNS、APNS_SANDBOX。</p>
    <a name="ul10271204916315"></a><a name="ul10271204916315"></a><ul id="ul10271204916315"><li>HMS是为开发者提供的消息推送平台。</li><li>APNS和APNS_SANDBOX是用于推送iOS消息的服务平台。</li><li>HMS平台指定的消息内容不超过2K</li><li>APNS和APNS_SANDBOX平台的消息内容不能超过4K</li></ul>
    <p id="p89342034424"><a name="p89342034424"></a><a name="p89342034424"></a>推送平台的消息内容格式要求详情见<a href="application消息体格式.md">application消息体格式</a>。</p>
    </td>
    </tr>
    <tr id="row5338165717155"><td class="cellrowborder" valign="top" width="21.31213121312131%" headers="mcps1.1.5.1.1 "><p id="p1533811576156"><a name="p1533811576156"></a><a name="p1533811576156"></a>time _to_live</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.31213121312131%" headers="mcps1.1.5.1.2 "><p id="p5760202491614"><a name="p5760202491614"></a><a name="p5760202491614"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.031803180318033%" headers="mcps1.1.5.1.3 "><p id="p123388576157"><a name="p123388576157"></a><a name="p123388576157"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="39.34393439343935%" headers="mcps1.1.5.1.4 "><p id="p860697124615"><a name="p860697124615"></a><a name="p860697124615"></a>消息发送的生存时间，是相对于发布时间的。</p>
    <p id="p4356925115613"><a name="p4356925115613"></a><a name="p4356925115613"></a>SMN系统将移动推送消息转交给推送平台前，会计算该消息在系统消耗的时间。只有消耗的时间小于time_to_live时，SMN才会将消息转交给推送平台，并将time_to_live减去消耗的时间传递给推送平台，否则消息废弃。</p>
    <p id="p0262452195420"><a name="p0262452195420"></a><a name="p0262452195420"></a>time _to_live的单位是s，变量默认值是3600s，即一小时。值为正整数且小于等于3600*24*7。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例

    ```
    POST https://{SMN_Endpoint}/v2/{project_id}/notifications/endpoints/{endpoint_urn}/publish
    {
        "message":{
             "hps":{
                   "msg":{
                         "action":{ 
                               "param":{
                                    "intent":"#Intent;compo=com.HC.SmnAppPush.defaultAction/.Activity;S.W=U;end"
                               },
                               "type":1
                         },
                         "body":{
                               "title":"hello world",
                               "content":"hello world"
                         },
                         "type":3
                    }
             }
        }
    }
    ```


## 响应消息<a name="zh-cn_topic_0118694332_section36818119"></a>

-   要素说明

    <a name="zh-cn_topic_0118694332_table26328706"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0118694332_row6366124"><th class="cellrowborder" valign="top" width="29.73%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0118694332_p45894015"><a name="zh-cn_topic_0118694332_p45894015"></a><a name="zh-cn_topic_0118694332_p45894015"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="27.029999999999998%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0118694332_p26427706"><a name="zh-cn_topic_0118694332_p26427706"></a><a name="zh-cn_topic_0118694332_p26427706"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="43.24%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0118694332_p60269446"><a name="zh-cn_topic_0118694332_p60269446"></a><a name="zh-cn_topic_0118694332_p60269446"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0118694332_row22411503"><td class="cellrowborder" valign="top" width="29.73%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0118694332_p3392477"><a name="zh-cn_topic_0118694332_p3392477"></a><a name="zh-cn_topic_0118694332_p3392477"></a>request_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.029999999999998%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0118694332_p6355195"><a name="zh-cn_topic_0118694332_p6355195"></a><a name="zh-cn_topic_0118694332_p6355195"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="43.24%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0118694332_p45008753"><a name="zh-cn_topic_0118694332_p45008753"></a><a name="zh-cn_topic_0118694332_p45008753"></a>请求的唯一标识ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0118694332_row62255659"><td class="cellrowborder" valign="top" width="29.73%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0118694332_p9543622"><a name="zh-cn_topic_0118694332_p9543622"></a><a name="zh-cn_topic_0118694332_p9543622"></a>message_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.029999999999998%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0118694332_p34835893"><a name="zh-cn_topic_0118694332_p34835893"></a><a name="zh-cn_topic_0118694332_p34835893"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="43.24%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0118694332_p3135073"><a name="zh-cn_topic_0118694332_p3135073"></a><a name="zh-cn_topic_0118694332_p3135073"></a>唯一的消息ID。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    { 
        "message_id": "bf94b63a5dfb475994d3ac34664e24f2", 
        "request_id": "9974c07f6d554a6d827956acbeb4be5f" 
    }
    ```


## 返回值<a name="zh-cn_topic_0118694332_section62927619"></a>

请参考[返回值](返回值.md)。

## 错误码<a name="section73211020122511"></a>

请参考[错误码说明](错误码说明.md)。

