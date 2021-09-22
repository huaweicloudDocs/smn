# App消息发布<a name="PublishAppMessage"></a>

## 功能介绍<a name="section12307181692116"></a>

将消息直发给endpoint设备。

## 调试<a name="section1056114122524"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=SMN&api=ListTopics)中调试该接口。

## URI<a name="section1731051611217"></a>

POST /v2/\{project\_id\}/notifications/endpoints/\{endpoint\_urn\}/publish

**表 1**  路径参数

<a name="table10313151614218"></a>
<table><thead align="left"><tr id="row203121616132116"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p1831491612214"><a name="p1831491612214"></a><a name="p1831491612214"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p1531518162210"><a name="p1531518162210"></a><a name="p1531518162210"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p1031671652115"><a name="p1031671652115"></a><a name="p1031671652115"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p1331713169217"><a name="p1331713169217"></a><a name="p1331713169217"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row5312716112115"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p13318416102120"><a name="p13318416102120"></a><a name="p13318416102120"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p193185165215"><a name="p193185165215"></a><a name="p193185165215"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p153191516182113"><a name="p153191516182113"></a><a name="p153191516182113"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p163201165215"><a name="p163201165215"></a><a name="p163201165215"></a>项目ID。</p>
<p id="p4568812165217"><a name="p4568812165217"></a><a name="p4568812165217"></a>获取项目ID请参考<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
<tr id="row1831281692118"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p232218165218"><a name="p232218165218"></a><a name="p232218165218"></a>endpoint_urn</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p10323716112117"><a name="p10323716112117"></a><a name="p10323716112117"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p23231616162111"><a name="p23231616162111"></a><a name="p23231616162111"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1232451614219"><a name="p1232451614219"></a><a name="p1232451614219"></a>Endpoint的唯一资源标识，可通过<a href="查询Application的Endpoint列表.md">查询Application的Endpoint列表</a>获取该标识</p>
</td>
</tr>
</tbody>
</table>

## 请求参数<a name="section203251916172120"></a>

**表 2**  请求Header参数

<a name="HeaderParameter"></a>
<table><thead align="left"><tr id="row113264162211"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p1632714169214"><a name="p1632714169214"></a><a name="p1632714169214"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p432871622118"><a name="p432871622118"></a><a name="p432871622118"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p3329171620213"><a name="p3329171620213"></a><a name="p3329171620213"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p1133041619213"><a name="p1133041619213"></a><a name="p1133041619213"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row143260160216"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p83304161215"><a name="p83304161215"></a><a name="p83304161215"></a>X-Auth-Token</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1133171602114"><a name="p1133171602114"></a><a name="p1133171602114"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p173321316172120"><a name="p173321316172120"></a><a name="p173321316172120"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p143331516142110"><a name="p143331516142110"></a><a name="p143331516142110"></a>用户Token。</p>
<p id="p143331416122115"><a name="p143331416122115"></a><a name="p143331416122115"></a>通过调用IAM服务获取用户Token接口获取（响应消息头中X-Subject-Token的值）。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  请求Body参数

<a name="requestParameter"></a>
<table><thead align="left"><tr id="row183341716152119"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p233551619218"><a name="p233551619218"></a><a name="p233551619218"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p193361216112113"><a name="p193361216112113"></a><a name="p193361216112113"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p12337131619214"><a name="p12337131619214"></a><a name="p12337131619214"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p1333801612115"><a name="p1333801612115"></a><a name="p1333801612115"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row733481662111"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p63381616102112"><a name="p63381616102112"></a><a name="p63381616102112"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p113391716112116"><a name="p113391716112116"></a><a name="p113391716112116"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p18340616172111"><a name="p18340616172111"></a><a name="p18340616172111"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1234271612118"><a name="p1234271612118"></a><a name="p1234271612118"></a>message与message_structure二者选其一。</p>
<p id="p1934211613216"><a name="p1934211613216"></a><a name="p1934211613216"></a>message, App消息发布。</p>
<p id="p203439162211"><a name="p203439162211"></a><a name="p203439162211"></a>message_structure, 使用消息结构体方式的App消息发布。</p>
<p id="p10343171672117"><a name="p10343171672117"></a><a name="p10343171672117"></a>app推送的消息内容，当前支持的推送平台有HMS、APNS、APNS_SANDBOX。</p>
<p id="p334371617218"><a name="p334371617218"></a><a name="p334371617218"></a>HMS是为开发者提供的消息推送平台。</p>
<p id="p10344181632115"><a name="p10344181632115"></a><a name="p10344181632115"></a>APNS和APNS_SANDBOX是用于推送iOS消息的服务平台。</p>
<p id="p203450165218"><a name="p203450165218"></a><a name="p203450165218"></a>HMS平台指定的消息内容不超过2K。</p>
<p id="p8345171619217"><a name="p8345171619217"></a><a name="p8345171619217"></a>APNS和APNS_SANDBOX平台的消息内容不能超过4K。</p>
<p id="p6346151612211"><a name="p6346151612211"></a><a name="p6346151612211"></a>推送平台的消息内容格式要求详情见application消息体格式。</p>
<p id="p1347616142116"><a name="p1347616142116"></a><a name="p1347616142116"></a>华为透传消息</p>
<p id="p1934751682114"><a name="p1934751682114"></a><a name="p1934751682114"></a>{ "hps": { "msg": { "type": 1, "body": { "key": "value" } } } }</p>
<p id="p334811622116"><a name="p334811622116"></a><a name="p334811622116"></a>华为系统通知栏消息</p>
<p id="p123489162217"><a name="p123489162217"></a><a name="p123489162217"></a>{ "hps": { "msg": { "type": 3, "body": { "content": "Push message content", "title": "Push message content" }, "action": { "type": 1, "param": { "intent": "#Intent;compo=com.rvr/.Activity;S.W=U;end" } } }, "ext": { "biTag": "Trump", "icon": "http://upload.w.org/00/150pxsvg.png" } } }</p>
<p id="p1234931672113"><a name="p1234931672113"></a><a name="p1234931672113"></a>苹果平台消息格式 { "aps": { "alert": "hello world" } }</p>
</td>
</tr>
<tr id="row133461632112"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p435071622115"><a name="p435071622115"></a><a name="p435071622115"></a>message_structure</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p935131612115"><a name="p935131612115"></a><a name="p935131612115"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p183521516182114"><a name="p183521516182114"></a><a name="p183521516182114"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p5354016172112"><a name="p5354016172112"></a><a name="p5354016172112"></a>app推送的消息内容，当前支持的推送平台有HMS、APNS、APNS_SANDBOX。</p>
<p id="p18354161672117"><a name="p18354161672117"></a><a name="p18354161672117"></a>HMS是为开发者提供的消息推送平台。</p>
<p id="p535410164217"><a name="p535410164217"></a><a name="p535410164217"></a>APNS和APNS_SANDBOX是用于推送iOS消息的服务平台。</p>
<p id="p1355216152119"><a name="p1355216152119"></a><a name="p1355216152119"></a>HMS平台指定的消息内容不超过2K。</p>
<p id="p113561516122115"><a name="p113561516122115"></a><a name="p113561516122115"></a>APNS和APNS_SANDBOX平台的消息内容不能超过4K。</p>
<p id="p93561016162114"><a name="p93561016162114"></a><a name="p93561016162114"></a>推送平台的消息内容格式要求详情见application消息体格式。</p>
<p id="p13357121672111"><a name="p13357121672111"></a><a name="p13357121672111"></a>华为透传消息</p>
<p id="p1435791618210"><a name="p1435791618210"></a><a name="p1435791618210"></a>{ "HMS": { "hps": { "msg": { "type": 1, "body": { "key": "value" } } } } }</p>
<p id="p035813167211"><a name="p035813167211"></a><a name="p035813167211"></a>华为系统通知栏消息</p>
<p id="p335818167214"><a name="p335818167214"></a><a name="p335818167214"></a>{ "HMS": { "hps": { "msg": { "type": 3, "body": { "content": "Push message content", "title": "Push message content" }, "action": { "type": 1, "param": { "intent": "#Intent;compo=com.rvr/.Activity;S.W=U;end" } } }, "ext": { "biTag": "Trump", "icon": "http://upload.w.org/00/150pxsvg.png" } } } }</p>
<p id="p1735914167211"><a name="p1735914167211"></a><a name="p1735914167211"></a>苹果平台消息格式</p>
<p id="p2359141620215"><a name="p2359141620215"></a><a name="p2359141620215"></a>{ "APNS": { "aps": { "alert": "hello world" } } }</p>
</td>
</tr>
<tr id="row6334111672119"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p83601816122110"><a name="p83601816122110"></a><a name="p83601816122110"></a>time_to_live</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1236111162219"><a name="p1236111162219"></a><a name="p1236111162219"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p13621016172113"><a name="p13621016172113"></a><a name="p13621016172113"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p0363131692114"><a name="p0363131692114"></a><a name="p0363131692114"></a>消息发送的生存时间，是相对于发布时间的。</p>
<p id="p15363161622113"><a name="p15363161622113"></a><a name="p15363161622113"></a>SMN系统将移动推送消息转交给推送平台前，会计算该消息在系统消耗的时间。只有消耗的时间小于time_to_live时，SMN才会将消息转交给推送平台，并将time_to_live减去消耗的时间传递给推送平台，否则消息废弃。</p>
<p id="p203641816102120"><a name="p203641816102120"></a><a name="p203641816102120"></a>time _to_live的单位是s，变量默认值是3600s，即一小时。值为正整数且小于等于3600*24。</p>
<p id="p5365916112120"><a name="p5365916112120"></a><a name="p5365916112120"></a>缺省值：<strong id="b7365171692114"><a name="b7365171692114"></a><a name="b7365171692114"></a>3600</strong></p>
</td>
</tr>
</tbody>
</table>

## 响应参数<a name="section10366111612210"></a>

**状态码： 200**

**表 4**  响应Body参数

<a name="responseParameter"></a>
<table><thead align="left"><tr id="row18368216182117"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p17369151611218"><a name="p17369151611218"></a><a name="p17369151611218"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p17370716172116"><a name="p17370716172116"></a><a name="p17370716172116"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p203718163212"><a name="p203718163212"></a><a name="p203718163212"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row7368191612210"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1537111652117"><a name="p1537111652117"></a><a name="p1537111652117"></a>message_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p13721916172111"><a name="p13721916172111"></a><a name="p13721916172111"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p10373121619219"><a name="p10373121619219"></a><a name="p10373121619219"></a>唯一的消息ID。</p>
</td>
</tr>
<tr id="row136820162213"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p33733165216"><a name="p33733165216"></a><a name="p33733165216"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p03749169211"><a name="p03749169211"></a><a name="p03749169211"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p2375111622119"><a name="p2375111622119"></a><a name="p2375111622119"></a>请求的唯一标识ID。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 400**

**表 5**  响应Body参数

<a name="table937691652110"></a>
<table><thead align="left"><tr id="row13771016172116"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p1437941622113"><a name="p1437941622113"></a><a name="p1437941622113"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p183801716192112"><a name="p183801716192112"></a><a name="p183801716192112"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p4381151642118"><a name="p4381151642118"></a><a name="p4381151642118"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row11377121619218"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1738251662119"><a name="p1738251662119"></a><a name="p1738251662119"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p11383191611213"><a name="p11383191611213"></a><a name="p11383191611213"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1438461619216"><a name="p1438461619216"></a><a name="p1438461619216"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row193772169216"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p73852166217"><a name="p73852166217"></a><a name="p73852166217"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p19385416172113"><a name="p19385416172113"></a><a name="p19385416172113"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p163862016132115"><a name="p163862016132115"></a><a name="p163862016132115"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row12377151622115"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p4387151662118"><a name="p4387151662118"></a><a name="p4387151662118"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p173886165214"><a name="p173886165214"></a><a name="p173886165214"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p3388121632116"><a name="p3388121632116"></a><a name="p3388121632116"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 403**

**表 6**  响应Body参数

<a name="table183899164216"></a>
<table><thead align="left"><tr id="row139061613215"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p539212166216"><a name="p539212166216"></a><a name="p539212166216"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p739331612119"><a name="p739331612119"></a><a name="p739331612119"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p1539471617214"><a name="p1539471617214"></a><a name="p1539471617214"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row18390141652110"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p2394121672115"><a name="p2394121672115"></a><a name="p2394121672115"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p15396161642113"><a name="p15396161642113"></a><a name="p15396161642113"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1039720167215"><a name="p1039720167215"></a><a name="p1039720167215"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row53903160218"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p19398316132112"><a name="p19398316132112"></a><a name="p19398316132112"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1939912168212"><a name="p1939912168212"></a><a name="p1939912168212"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1340011618213"><a name="p1340011618213"></a><a name="p1340011618213"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row2039051612119"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p114011166211"><a name="p114011166211"></a><a name="p114011166211"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p84011160211"><a name="p84011160211"></a><a name="p84011160211"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p6402016152117"><a name="p6402016152117"></a><a name="p6402016152117"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 404**

**表 7**  响应Body参数

<a name="table540315163218"></a>
<table><thead align="left"><tr id="row124046163218"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p0406181620211"><a name="p0406181620211"></a><a name="p0406181620211"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p1640711642119"><a name="p1640711642119"></a><a name="p1640711642119"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p15408216142110"><a name="p15408216142110"></a><a name="p15408216142110"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row8404416152111"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p34095166211"><a name="p34095166211"></a><a name="p34095166211"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p940971642114"><a name="p940971642114"></a><a name="p940971642114"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p8410111611213"><a name="p8410111611213"></a><a name="p8410111611213"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row94041316152117"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1341131682120"><a name="p1341131682120"></a><a name="p1341131682120"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1341213163213"><a name="p1341213163213"></a><a name="p1341213163213"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1413121642114"><a name="p1413121642114"></a><a name="p1413121642114"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row1240441672112"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1541491615211"><a name="p1541491615211"></a><a name="p1541491615211"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p144144164218"><a name="p144144164218"></a><a name="p144144164218"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p18415716142110"><a name="p18415716142110"></a><a name="p18415716142110"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 500**

**表 8**  响应Body参数

<a name="table16416111672112"></a>
<table><thead align="left"><tr id="row041611614217"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p184186166214"><a name="p184186166214"></a><a name="p184186166214"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p94182016152111"><a name="p94182016152111"></a><a name="p94182016152111"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p1141920165213"><a name="p1141920165213"></a><a name="p1141920165213"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1941613164217"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p13420151613217"><a name="p13420151613217"></a><a name="p13420151613217"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p642161632110"><a name="p642161632110"></a><a name="p642161632110"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p17422181612216"><a name="p17422181612216"></a><a name="p17422181612216"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row1841771622113"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1942331612116"><a name="p1942331612116"></a><a name="p1942331612116"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p184241916172117"><a name="p184241916172117"></a><a name="p184241916172117"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p8425131682112"><a name="p8425131682112"></a><a name="p8425131682112"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row741719169215"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p11426171672119"><a name="p11426171672119"></a><a name="p11426171672119"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p2426181611211"><a name="p2426181611211"></a><a name="p2426181611211"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p5427131692117"><a name="p5427131692117"></a><a name="p5427131692117"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

## 请求示例<a name="section0428141616216"></a>

-   App消息发布

    ```
    POST https://{SMN_Endpoint}/v2/{project_id}/notifications/endpoints/{endpoint_urn}/publish
    
    {
      "message" : {
        "hps" : {
          "msg" : {
            "action" : {
              "param" : {
                "intent" : "#Intent;compo=com.HC.SmnAppPush.defaultAction/.Activity;S.W=U;end"
              },
              "type" : 1
            },
            "body" : {
              "title" : "hello world",
              "content" : "hello world"
            },
            "type" : 3
          }
        }
      },
      "time_to_live" : 3600
    }
    ```

-   使用消息结构体方式的App消息发布

    ```
    POST https://{SMN_Endpoint}/v2/{project_id}/notifications/endpoints/{endpoint_urn}/publish
    
    {
      "message" : {
        "HMS" : {
          "hps" : {
            "msg" : {
              "action" : {
                "param" : {
                  "intent" : "#Intent;compo=com.HC.SmnAppPush.defaultAction/.Activity;S.W=U;end"
                },
                "type" : 1
              },
              "body" : {
                "title" : "hello world",
                "content" : "hello world"
              },
              "type" : 3
            }
          }
        }
      },
      "time_to_live" : 3600
    }
    ```


## 响应示例<a name="section1567216162113"></a>

无

## 状态码<a name="section556814161219"></a>

<a name="status_code"></a>
<table><thead align="left"><tr id="row13464111672119"><th class="cellrowborder" valign="top" width="15%" id="mcps1.1.3.1.1"><p id="p2056851652113"><a name="p2056851652113"></a><a name="p2056851652113"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="85%" id="mcps1.1.3.1.2"><p id="p1256821610217"><a name="p1256821610217"></a><a name="p1256821610217"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row04646165215"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p4569131612216"><a name="p4569131612216"></a><a name="p4569131612216"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p20569816152119"><a name="p20569816152119"></a><a name="p20569816152119"></a>OK</p>
</td>
</tr>
<tr id="row1646501632115"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p456991632110"><a name="p456991632110"></a><a name="p456991632110"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p2569101614218"><a name="p2569101614218"></a><a name="p2569101614218"></a>Bad Request</p>
</td>
</tr>
<tr id="row04652016102115"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p1056915165218"><a name="p1056915165218"></a><a name="p1056915165218"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p19570816192116"><a name="p19570816192116"></a><a name="p19570816192116"></a>Unauthorized</p>
</td>
</tr>
<tr id="row946541682119"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p1457031612113"><a name="p1457031612113"></a><a name="p1457031612113"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p45707165218"><a name="p45707165218"></a><a name="p45707165218"></a>Not Found</p>
</td>
</tr>
<tr id="row9465201617218"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p857010163212"><a name="p857010163212"></a><a name="p857010163212"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p1857151612213"><a name="p1857151612213"></a><a name="p1857151612213"></a>Internal Server Error</p>
</td>
</tr>
</tbody>
</table>

## 错误码<a name="section8571816152110"></a>

请参见[错误码](错误码.md)。

