# 删除Application endpoint<a name="DeleteApplicationEndpoint"></a>

## 功能介绍<a name="section141413117216"></a>

删除设备。

## 调试<a name="section1056114122524"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=SMN&api=ListTopics)中调试该接口。

## URI<a name="section941719118213"></a>

DELETE /v2/\{project\_id\}/notifications/endpoints/\{endpoint\_urn\}

**表 1**  路径参数

<a name="table13420711162114"></a>
<table><thead align="left"><tr id="row441914112210"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p13421181192111"><a name="p13421181192111"></a><a name="p13421181192111"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p134211811102114"><a name="p134211811102114"></a><a name="p134211811102114"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p13422131115219"><a name="p13422131115219"></a><a name="p13422131115219"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p1142381152120"><a name="p1142381152120"></a><a name="p1142381152120"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row15419151102116"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p13424131152115"><a name="p13424131152115"></a><a name="p13424131152115"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1425201152116"><a name="p1425201152116"></a><a name="p1425201152116"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1425311132113"><a name="p1425311132113"></a><a name="p1425311132113"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1442601162115"><a name="p1442601162115"></a><a name="p1442601162115"></a>项目ID。</p>
<p id="p4568812165217"><a name="p4568812165217"></a><a name="p4568812165217"></a>获取项目ID请参考<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
<tr id="row1419811152115"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p442881120210"><a name="p442881120210"></a><a name="p442881120210"></a>endpoint_urn</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p0429131113218"><a name="p0429131113218"></a><a name="p0429131113218"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p44291211122110"><a name="p44291211122110"></a><a name="p44291211122110"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p144302111218"><a name="p144302111218"></a><a name="p144302111218"></a>Endpoint的唯一资源标识，可通过<a href="查询Application的Endpoint列表.md">查询Application的Endpoint列表</a>获取该标识。</p>
</td>
</tr>
</tbody>
</table>

## 请求参数<a name="section15431121120218"></a>

**表 2**  请求Header参数

<a name="HeaderParameter"></a>
<table><thead align="left"><tr id="row19432311132117"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p1543313116215"><a name="p1543313116215"></a><a name="p1543313116215"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p13434131116219"><a name="p13434131116219"></a><a name="p13434131116219"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p44351011122110"><a name="p44351011122110"></a><a name="p44351011122110"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p2435171115214"><a name="p2435171115214"></a><a name="p2435171115214"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1543221113213"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p543618115218"><a name="p543618115218"></a><a name="p543618115218"></a>X-Auth-Token</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p6437151132117"><a name="p6437151132117"></a><a name="p6437151132117"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p154381011112119"><a name="p154381011112119"></a><a name="p154381011112119"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p17439111112114"><a name="p17439111112114"></a><a name="p17439111112114"></a>用户Token。</p>
<p id="p643971132118"><a name="p643971132118"></a><a name="p643971132118"></a>通过调用IAM服务获取用户Token接口获取（响应消息头中X-Subject-Token的值）。</p>
</td>
</tr>
</tbody>
</table>

## 响应参数<a name="section16440101122111"></a>

**状态码： 200**

**表 3**  响应Body参数

<a name="responseParameter"></a>
<table><thead align="left"><tr id="row244201119217"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p14443121192115"><a name="p14443121192115"></a><a name="p14443121192115"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p144451142110"><a name="p144451142110"></a><a name="p144451142110"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p19445211142112"><a name="p19445211142112"></a><a name="p19445211142112"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row4442511172117"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p144465117219"><a name="p144465117219"></a><a name="p144465117219"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p14446181116213"><a name="p14446181116213"></a><a name="p14446181116213"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1144771114218"><a name="p1144771114218"></a><a name="p1144771114218"></a>请求的唯一标识ID。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 400**

**表 4**  响应Body参数

<a name="table15448111182114"></a>
<table><thead align="left"><tr id="row1744815111214"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p5450611122112"><a name="p5450611122112"></a><a name="p5450611122112"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p0450131162118"><a name="p0450131162118"></a><a name="p0450131162118"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p1045116115216"><a name="p1045116115216"></a><a name="p1045116115216"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row244801192115"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p245231118213"><a name="p245231118213"></a><a name="p245231118213"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p84521311142119"><a name="p84521311142119"></a><a name="p84521311142119"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1245317111214"><a name="p1245317111214"></a><a name="p1245317111214"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row544961172117"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1454181102113"><a name="p1454181102113"></a><a name="p1454181102113"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1045513112213"><a name="p1045513112213"></a><a name="p1045513112213"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1845581122114"><a name="p1845581122114"></a><a name="p1845581122114"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row2449191113215"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p24561011162115"><a name="p24561011162115"></a><a name="p24561011162115"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p44576116214"><a name="p44576116214"></a><a name="p44576116214"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p154581211142117"><a name="p154581211142117"></a><a name="p154581211142117"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 403**

**表 5**  响应Body参数

<a name="table124593119211"></a>
<table><thead align="left"><tr id="row2460181119214"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p15462181119219"><a name="p15462181119219"></a><a name="p15462181119219"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p346301120211"><a name="p346301120211"></a><a name="p346301120211"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p14463101114215"><a name="p14463101114215"></a><a name="p14463101114215"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row18460191114219"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p13464191112110"><a name="p13464191112110"></a><a name="p13464191112110"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p44656118219"><a name="p44656118219"></a><a name="p44656118219"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p346581162111"><a name="p346581162111"></a><a name="p346581162111"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row194601611142112"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p164661411132113"><a name="p164661411132113"></a><a name="p164661411132113"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1946631117212"><a name="p1946631117212"></a><a name="p1946631117212"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p64671911152118"><a name="p64671911152118"></a><a name="p64671911152118"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row44601711122116"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p74681711132118"><a name="p74681711132118"></a><a name="p74681711132118"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1746918118213"><a name="p1746918118213"></a><a name="p1746918118213"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p947018118213"><a name="p947018118213"></a><a name="p947018118213"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 404**

**表 6**  响应Body参数

<a name="table1247031110216"></a>
<table><thead align="left"><tr id="row16471171182117"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p347241122120"><a name="p347241122120"></a><a name="p347241122120"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p847311112216"><a name="p847311112216"></a><a name="p847311112216"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p74731311182111"><a name="p74731311182111"></a><a name="p74731311182111"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row24711111142111"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p747431152116"><a name="p747431152116"></a><a name="p747431152116"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p54749114213"><a name="p54749114213"></a><a name="p54749114213"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p17475201122110"><a name="p17475201122110"></a><a name="p17475201122110"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row17471161111214"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p7475211192114"><a name="p7475211192114"></a><a name="p7475211192114"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1476111152114"><a name="p1476111152114"></a><a name="p1476111152114"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p94779118212"><a name="p94779118212"></a><a name="p94779118212"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row13471711132116"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p6477101172110"><a name="p6477101172110"></a><a name="p6477101172110"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p44788112213"><a name="p44788112213"></a><a name="p44788112213"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1547961162116"><a name="p1547961162116"></a><a name="p1547961162116"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 500**

**表 7**  响应Body参数

<a name="table174800113214"></a>
<table><thead align="left"><tr id="row748017111217"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p1482121110214"><a name="p1482121110214"></a><a name="p1482121110214"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p34825113216"><a name="p34825113216"></a><a name="p34825113216"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p124836113212"><a name="p124836113212"></a><a name="p124836113212"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row154818116214"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1483171192112"><a name="p1483171192112"></a><a name="p1483171192112"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p10484711162116"><a name="p10484711162116"></a><a name="p10484711162116"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p18485181152116"><a name="p18485181152116"></a><a name="p18485181152116"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row194811111152114"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1648571132117"><a name="p1648571132117"></a><a name="p1648571132117"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p0486161192115"><a name="p0486161192115"></a><a name="p0486161192115"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1448751172113"><a name="p1448751172113"></a><a name="p1448751172113"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row84814113211"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1648731162110"><a name="p1648731162110"></a><a name="p1648731162110"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1948814118212"><a name="p1948814118212"></a><a name="p1948814118212"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p144886119212"><a name="p144886119212"></a><a name="p144886119212"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

## 请求示例<a name="section11489161112212"></a>

删除Application endpoint

```
DELETE https://{SMN_Endpoint}/v2/{project_id}/notifications/endpoints/{endpoint_urn}

null
```

## 响应示例<a name="section17493151192111"></a>

无

## 状态码<a name="section1049413115215"></a>

<a name="status_code"></a>
<table><thead align="left"><tr id="row94965114215"><th class="cellrowborder" valign="top" width="15%" id="mcps1.1.3.1.1"><p id="p949781114212"><a name="p949781114212"></a><a name="p949781114212"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="85%" id="mcps1.1.3.1.2"><p id="p15498181142116"><a name="p15498181142116"></a><a name="p15498181142116"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row249611113212"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p1249871112119"><a name="p1249871112119"></a><a name="p1249871112119"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p1449931116219"><a name="p1449931116219"></a><a name="p1449931116219"></a>OK</p>
</td>
</tr>
<tr id="row19496111116217"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p550041162110"><a name="p550041162110"></a><a name="p550041162110"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p105011119214"><a name="p105011119214"></a><a name="p105011119214"></a>Bad Request</p>
</td>
</tr>
<tr id="row134962114210"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p18502121113214"><a name="p18502121113214"></a><a name="p18502121113214"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p1150315116216"><a name="p1150315116216"></a><a name="p1150315116216"></a>Unauthorized</p>
</td>
</tr>
<tr id="row11496141112113"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p1504161112114"><a name="p1504161112114"></a><a name="p1504161112114"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p95041411142118"><a name="p95041411142118"></a><a name="p95041411142118"></a>Not Found</p>
</td>
</tr>
<tr id="row204965114216"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p1505311162120"><a name="p1505311162120"></a><a name="p1505311162120"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p35061111192120"><a name="p35061111192120"></a><a name="p35061111192120"></a>Internal Server Error</p>
</td>
</tr>
</tbody>
</table>

## 错误码<a name="section7506131120212"></a>

请参见[错误码](错误码.md)。

