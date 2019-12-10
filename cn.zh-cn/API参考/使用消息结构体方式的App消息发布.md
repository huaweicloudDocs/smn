# 使用消息结构体方式的App消息发布<a name="ZH-CN_TOPIC_0118712471"></a>

## 功能介绍<a name="zh-cn_topic_0118694333_section51657386"></a>

-   接口名称

    PublishAppStructureMessage

-   功能描述

    将消息按结构体方式直发给endpoint设备。


## URI<a name="zh-cn_topic_0118694333_section62263298"></a>

-   URI格式

    POST /v2/\{project\_id\}/notifications/endpoints/\{endpoint\_urn\}/publish

-   参数说明

    <a name="zh-cn_topic_0118694333_table28645947"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0118694333_row28364525"><th class="cellrowborder" valign="top" width="23.95%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0118694333_p15825197"><a name="zh-cn_topic_0118694333_p15825197"></a><a name="zh-cn_topic_0118694333_p15825197"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.53%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0118694333_p6772561"><a name="zh-cn_topic_0118694333_p6772561"></a><a name="zh-cn_topic_0118694333_p6772561"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.53%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0118694333_p11706562"><a name="zh-cn_topic_0118694333_p11706562"></a><a name="zh-cn_topic_0118694333_p11706562"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="30.990000000000002%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0118694333_p8707431"><a name="zh-cn_topic_0118694333_p8707431"></a><a name="zh-cn_topic_0118694333_p8707431"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0118694333_row19812975"><td class="cellrowborder" valign="top" width="23.95%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0118694333_p61347105"><a name="zh-cn_topic_0118694333_p61347105"></a><a name="zh-cn_topic_0118694333_p61347105"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.53%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0118694333_p3059624"><a name="zh-cn_topic_0118694333_p3059624"></a><a name="zh-cn_topic_0118694333_p3059624"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.53%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0118694333_p46503020"><a name="zh-cn_topic_0118694333_p46503020"></a><a name="zh-cn_topic_0118694333_p46503020"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.990000000000002%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0118694333_p8648276"><a name="zh-cn_topic_0118694333_p8648276"></a><a name="zh-cn_topic_0118694333_p8648276"></a>项目ID</p>
    <p id="zh-cn_topic_0118694333_p10725625"><a name="zh-cn_topic_0118694333_p10725625"></a><a name="zh-cn_topic_0118694333_p10725625"></a>获取项目ID请参考<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0118694333_row40742214"><td class="cellrowborder" valign="top" width="23.95%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0118694333_p11785017"><a name="zh-cn_topic_0118694333_p11785017"></a><a name="zh-cn_topic_0118694333_p11785017"></a>endpoint_urn</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.53%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0118694333_p15062292"><a name="zh-cn_topic_0118694333_p15062292"></a><a name="zh-cn_topic_0118694333_p15062292"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.53%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0118694333_p12086144"><a name="zh-cn_topic_0118694333_p12086144"></a><a name="zh-cn_topic_0118694333_p12086144"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.990000000000002%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0118694333_p39453604"><a name="zh-cn_topic_0118694333_p39453604"></a><a name="zh-cn_topic_0118694333_p39453604"></a>Endpoint的唯一资源标识，可通过<a href="查询Application的Endpoint列表.md">查询Application的Endpoint列表</a>获取该标识。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="zh-cn_topic_0118694333_section23498771"></a>

-   参数说明

    <a name="zh-cn_topic_0118694333_table38188405"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0118694333_row39710449"><th class="cellrowborder" valign="top" width="24.64%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0118694333_p62429818"><a name="zh-cn_topic_0118694333_p62429818"></a><a name="zh-cn_topic_0118694333_p62429818"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="14.49%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0118694333_p23650467"><a name="zh-cn_topic_0118694333_p23650467"></a><a name="zh-cn_topic_0118694333_p23650467"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.39%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0118694333_p36639636"><a name="zh-cn_topic_0118694333_p36639636"></a><a name="zh-cn_topic_0118694333_p36639636"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="43.480000000000004%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0118694333_p15020534"><a name="zh-cn_topic_0118694333_p15020534"></a><a name="zh-cn_topic_0118694333_p15020534"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0118694333_row33913387"><td class="cellrowborder" valign="top" width="24.64%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0118694333_p62629839"><a name="zh-cn_topic_0118694333_p62629839"></a><a name="zh-cn_topic_0118694333_p62629839"></a>message_structure</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.49%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0118694333_p39852162"><a name="zh-cn_topic_0118694333_p39852162"></a><a name="zh-cn_topic_0118694333_p39852162"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.39%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0118694333_p6799727"><a name="zh-cn_topic_0118694333_p6799727"></a><a name="zh-cn_topic_0118694333_p6799727"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="43.480000000000004%" headers="mcps1.1.5.1.4 "><p id="p350111202418"><a name="p350111202418"></a><a name="p350111202418"></a>app推送的消息内容，当前支持的推送平台有HMS、APNS、APNS_SANDBOX。</p>
    <a name="ul87989201445"></a><a name="ul87989201445"></a><ul id="ul87989201445"><li><span>HMS是为开发者提供的消息推送平台</span>。</li><li>APNS和APNS_SANDBOX<span>是用于推送iOS消息的服务平台。</span></li><li>HMS平台指定的消息内容不超过2K</li><li>APNS和APNS_SANDBOX平台的消息内容不能超过4K</li></ul>
    <p id="p89342034424"><a name="p89342034424"></a><a name="p89342034424"></a>推送平台的消息内容格式要求详情见<a href="application消息体格式.md">application消息体格式</a>。</p>
    </td>
    </tr>
    <tr id="row198275315261"><td class="cellrowborder" valign="top" width="24.64%" headers="mcps1.1.5.1.1 "><p id="p1533811576156"><a name="p1533811576156"></a><a name="p1533811576156"></a>time _to_live</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.49%" headers="mcps1.1.5.1.2 "><p id="p5760202491614"><a name="p5760202491614"></a><a name="p5760202491614"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.39%" headers="mcps1.1.5.1.3 "><p id="p123388576157"><a name="p123388576157"></a><a name="p123388576157"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="43.480000000000004%" headers="mcps1.1.5.1.4 "><p id="p860697124615"><a name="p860697124615"></a><a name="p860697124615"></a>消息发送的生存时间，是<span>相对于发布时间的。</span></p>
    <p id="p4356925115613"><a name="p4356925115613"></a><a name="p4356925115613"></a><span>SMN</span><span>系统将移动推送消息转交给推送平台前，</span><span>会计算该消息在系统消耗的时间。</span><span>只有消耗的时间小于</span><span>time_to_live时</span><span>，</span><span>SMN</span><span>才会将消息转交给推送平台，并</span><span>将t</span><span>ime_to_live</span><span>减去消耗的时间传递给推送平台。</span></p>
    <p id="p0262452195420"><a name="p0262452195420"></a><a name="p0262452195420"></a>time _to_live的单位是s，变量默认值是3600s，即一小时。<span>值为正整</span><span>数</span>且小于等于3600*24*7。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例

    ```
    POST https://{SMN_Endpoint}/v2/{project_id}/notifications/endpoints/{endpoint_urn}/publish
    {
        "message_structure": "{
                "HMS":"{
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
                }"
        }"
    }
    ```


## 响应消息<a name="zh-cn_topic_0118694333_section10162352"></a>

-   要素说明

    <a name="zh-cn_topic_0118694333_table56051844"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0118694333_row27742239"><th class="cellrowborder" valign="top" width="29.73%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0118694333_p32528885"><a name="zh-cn_topic_0118694333_p32528885"></a><a name="zh-cn_topic_0118694333_p32528885"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="27.029999999999998%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0118694333_p17593999"><a name="zh-cn_topic_0118694333_p17593999"></a><a name="zh-cn_topic_0118694333_p17593999"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="43.24%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0118694333_p15827797"><a name="zh-cn_topic_0118694333_p15827797"></a><a name="zh-cn_topic_0118694333_p15827797"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0118694333_row28769672"><td class="cellrowborder" valign="top" width="29.73%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0118694333_p48642116"><a name="zh-cn_topic_0118694333_p48642116"></a><a name="zh-cn_topic_0118694333_p48642116"></a>request_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.029999999999998%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0118694333_p47697357"><a name="zh-cn_topic_0118694333_p47697357"></a><a name="zh-cn_topic_0118694333_p47697357"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="43.24%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0118694333_p38280714"><a name="zh-cn_topic_0118694333_p38280714"></a><a name="zh-cn_topic_0118694333_p38280714"></a>请求的唯一标识ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0118694333_row56462471"><td class="cellrowborder" valign="top" width="29.73%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0118694333_p10057430"><a name="zh-cn_topic_0118694333_p10057430"></a><a name="zh-cn_topic_0118694333_p10057430"></a>message_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.029999999999998%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0118694333_p9345526"><a name="zh-cn_topic_0118694333_p9345526"></a><a name="zh-cn_topic_0118694333_p9345526"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="43.24%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0118694333_p18790159"><a name="zh-cn_topic_0118694333_p18790159"></a><a name="zh-cn_topic_0118694333_p18790159"></a>唯一的消息ID。</p>
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


## 返回值<a name="section242171292113"></a>

请参考[返回值](返回值.md)。

## 错误码<a name="section73211020122511"></a>

请参考[错误码说明](错误码说明.md)。

