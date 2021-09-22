# 查询Application的Endpoint属性<a name="ListApplicationEndpointAttributes"></a>

## 功能介绍<a name="section95353819210"></a>

获取endpoint的属性。

## 调试<a name="section1056114122524"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=SMN&api=ListTopics)中调试该接口。

## URI<a name="section653713819219"></a>

GET /v2/\{project\_id\}/notifications/endpoints/\{endpoint\_urn\}

**表 1**  路径参数

<a name="table853898132113"></a>
<table><thead align="left"><tr id="row1253868142110"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p165391184215"><a name="p165391184215"></a><a name="p165391184215"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p13539108112111"><a name="p13539108112111"></a><a name="p13539108112111"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p2540158162120"><a name="p2540158162120"></a><a name="p2540158162120"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p1454019892111"><a name="p1454019892111"></a><a name="p1454019892111"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row053878112110"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1354120813212"><a name="p1354120813212"></a><a name="p1354120813212"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p15541128102110"><a name="p15541128102110"></a><a name="p15541128102110"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1654216892118"><a name="p1654216892118"></a><a name="p1654216892118"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1754212822114"><a name="p1754212822114"></a><a name="p1754212822114"></a>项目ID。</p>
<p id="p4568812165217"><a name="p4568812165217"></a><a name="p4568812165217"></a>获取项目ID请参考<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
<tr id="row3538587217"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p2054316892111"><a name="p2054316892111"></a><a name="p2054316892111"></a>endpoint_urn</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p35431288215"><a name="p35431288215"></a><a name="p35431288215"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p35449814210"><a name="p35449814210"></a><a name="p35449814210"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p254438112113"><a name="p254438112113"></a><a name="p254438112113"></a>Endpoint的唯一资源标识，可通过<a href="查询Application的Endpoint列表.md">查询Application的Endpoint列表</a>获取该标识。</p>
</td>
</tr>
</tbody>
</table>

## 请求参数<a name="section185455818213"></a>

**表 2**  请求Header参数

<a name="HeaderParameter"></a>
<table><thead align="left"><tr id="row154568162111"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p454620818214"><a name="p454620818214"></a><a name="p454620818214"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p154778122117"><a name="p154778122117"></a><a name="p154778122117"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p1854748182118"><a name="p1854748182118"></a><a name="p1854748182118"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p1454710811215"><a name="p1454710811215"></a><a name="p1454710811215"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row13545148112118"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p5548208162115"><a name="p5548208162115"></a><a name="p5548208162115"></a>X-Auth-Token</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p16548128182113"><a name="p16548128182113"></a><a name="p16548128182113"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p95497817212"><a name="p95497817212"></a><a name="p95497817212"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p95491088211"><a name="p95491088211"></a><a name="p95491088211"></a>用户Token。</p>
<p id="p145502832113"><a name="p145502832113"></a><a name="p145502832113"></a>通过调用IAM服务获取用户Token接口获取（响应消息头中X-Subject-Token的值）。</p>
</td>
</tr>
</tbody>
</table>

## 响应参数<a name="section9550186217"></a>

**状态码： 200**

**表 3**  响应Body参数

<a name="responseParameter"></a>
<table><thead align="left"><tr id="row175512812117"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p755219819211"><a name="p755219819211"></a><a name="p755219819211"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p25531481218"><a name="p25531481218"></a><a name="p25531481218"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p3553198182113"><a name="p3553198182113"></a><a name="p3553198182113"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row15511842112"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p855428192116"><a name="p855428192116"></a><a name="p855428192116"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1955414862115"><a name="p1955414862115"></a><a name="p1955414862115"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p9554084215"><a name="p9554084215"></a><a name="p9554084215"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row155217852115"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1455598142115"><a name="p1455598142115"></a><a name="p1455598142115"></a>attributes</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p655513822110"><a name="p655513822110"></a><a name="p655513822110"></a><a href="#response_ApplicationEndpointAttribute">表4</a>object</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p755510816218"><a name="p755510816218"></a><a name="p755510816218"></a>属性的键值对。</p>
</td>
</tr>
</tbody>
</table>

**表 4**  ApplicationEndpointAttribute

<a name="response_ApplicationEndpointAttribute"></a>
<table><thead align="left"><tr id="row5422896392"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p17423592391"><a name="p17423592391"></a><a name="p17423592391"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p2423497396"><a name="p2423497396"></a><a name="p2423497396"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p542449173912"><a name="p542449173912"></a><a name="p542449173912"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row15422395395"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1442419917390"><a name="p1442419917390"></a><a name="p1442419917390"></a>enabled</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1142413913911"><a name="p1142413913911"></a><a name="p1142413913911"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p6424169183914"><a name="p6424169183914"></a><a name="p6424169183914"></a>设备是否可用。</p>
</td>
</tr>
<tr id="row1942219113918"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p14425396394"><a name="p14425396394"></a><a name="p14425396394"></a>token</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p942511915393"><a name="p942511915393"></a><a name="p942511915393"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p44250914397"><a name="p44250914397"></a><a name="p44250914397"></a>设备token。</p>
</td>
</tr>
<tr id="row442217983916"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p842549153916"><a name="p842549153916"></a><a name="p842549153916"></a>user_data</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p19426209153911"><a name="p19426209153911"></a><a name="p19426209153911"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p144268914394"><a name="p144268914394"></a><a name="p144268914394"></a>用户数据。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 400**

**表 5**  响应Body参数

<a name="table8556688210"></a>
<table><thead align="left"><tr id="row18556178182118"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p7558198202114"><a name="p7558198202114"></a><a name="p7558198202114"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p13558789217"><a name="p13558789217"></a><a name="p13558789217"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p20559158112111"><a name="p20559158112111"></a><a name="p20559158112111"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row95568862110"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p15598862117"><a name="p15598862117"></a><a name="p15598862117"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p45602817212"><a name="p45602817212"></a><a name="p45602817212"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p4560789210"><a name="p4560789210"></a><a name="p4560789210"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row35571582214"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p356111822113"><a name="p356111822113"></a><a name="p356111822113"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p256110818212"><a name="p256110818212"></a><a name="p256110818212"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p105628822110"><a name="p105628822110"></a><a name="p105628822110"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row25576819213"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p6562588212"><a name="p6562588212"></a><a name="p6562588212"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p12563589216"><a name="p12563589216"></a><a name="p12563589216"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p35638832110"><a name="p35638832110"></a><a name="p35638832110"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 403**

**表 6**  响应Body参数

<a name="table1856418812114"></a>
<table><thead align="left"><tr id="row156568102117"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p1256512842113"><a name="p1256512842113"></a><a name="p1256512842113"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p656618872114"><a name="p656618872114"></a><a name="p656618872114"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p556619802120"><a name="p556619802120"></a><a name="p556619802120"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row165659822111"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1656718812114"><a name="p1656718812114"></a><a name="p1656718812114"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p656713892118"><a name="p656713892118"></a><a name="p656713892118"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1656711811218"><a name="p1656711811218"></a><a name="p1656711811218"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row65653802116"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p145686814216"><a name="p145686814216"></a><a name="p145686814216"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p115681083212"><a name="p115681083212"></a><a name="p115681083212"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p35686810217"><a name="p35686810217"></a><a name="p35686810217"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row1156514817217"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p05696820215"><a name="p05696820215"></a><a name="p05696820215"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p7569158182118"><a name="p7569158182118"></a><a name="p7569158182118"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p115691881213"><a name="p115691881213"></a><a name="p115691881213"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 404**

**表 7**  响应Body参数

<a name="table357020815218"></a>
<table><thead align="left"><tr id="row4570389212"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p257113822111"><a name="p257113822111"></a><a name="p257113822111"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p957298192113"><a name="p957298192113"></a><a name="p957298192113"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p175727819218"><a name="p175727819218"></a><a name="p175727819218"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row35706814212"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1357320852113"><a name="p1357320852113"></a><a name="p1357320852113"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p15731185216"><a name="p15731185216"></a><a name="p15731185216"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p457320812113"><a name="p457320812113"></a><a name="p457320812113"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row257017814219"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1657420802114"><a name="p1657420802114"></a><a name="p1657420802114"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p19574178142111"><a name="p19574178142111"></a><a name="p19574178142111"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p185742813217"><a name="p185742813217"></a><a name="p185742813217"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row557018192116"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1957517816214"><a name="p1957517816214"></a><a name="p1957517816214"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1257714815214"><a name="p1257714815214"></a><a name="p1257714815214"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1057768182116"><a name="p1057768182116"></a><a name="p1057768182116"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 500**

**表 8**  响应Body参数

<a name="table557878122118"></a>
<table><thead align="left"><tr id="row857917832115"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p958120819219"><a name="p958120819219"></a><a name="p958120819219"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p758113818213"><a name="p758113818213"></a><a name="p758113818213"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p85821785217"><a name="p85821785217"></a><a name="p85821785217"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row115790817215"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p35831487211"><a name="p35831487211"></a><a name="p35831487211"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p14583118162115"><a name="p14583118162115"></a><a name="p14583118162115"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p7583108142113"><a name="p7583108142113"></a><a name="p7583108142113"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row1657917832118"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p175842084213"><a name="p175842084213"></a><a name="p175842084213"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1058511814219"><a name="p1058511814219"></a><a name="p1058511814219"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p358518142119"><a name="p358518142119"></a><a name="p358518142119"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row1157958192110"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p25861683210"><a name="p25861683210"></a><a name="p25861683210"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p125866832120"><a name="p125866832120"></a><a name="p125866832120"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p10587118102112"><a name="p10587118102112"></a><a name="p10587118102112"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

## 请求示例<a name="section195872810210"></a>

```
GET https://{SMN_Endpoint}/v2/{project_id}/notifications/endpoints/{endpoint_urn}

null
```

## 响应示例<a name="section3588178192115"></a>

**状态码： 200**

OK

```
{
  "request_id" : "c90d871f77f7425cae0a8b772a563d17",
  "attributes" : {
    "enabled" : "true",
    "token" : "3708232124742383445",
    "user_data" : "abc"
  }
}
```

## 状态码<a name="section1059238172110"></a>

<a name="status_code"></a>
<table><thead align="left"><tr id="row8593108182115"><th class="cellrowborder" valign="top" width="15%" id="mcps1.1.3.1.1"><p id="p12594288214"><a name="p12594288214"></a><a name="p12594288214"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="85%" id="mcps1.1.3.1.2"><p id="p55941386219"><a name="p55941386219"></a><a name="p55941386219"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row14593158132110"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p859518812215"><a name="p859518812215"></a><a name="p859518812215"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p1059518842112"><a name="p1059518842112"></a><a name="p1059518842112"></a>OK</p>
</td>
</tr>
<tr id="row0593688213"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p18595389212"><a name="p18595389212"></a><a name="p18595389212"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p759620862115"><a name="p759620862115"></a><a name="p759620862115"></a>Bad Request</p>
</td>
</tr>
<tr id="row759312812112"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p4596198182115"><a name="p4596198182115"></a><a name="p4596198182115"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p259717815217"><a name="p259717815217"></a><a name="p259717815217"></a>Unauthorized</p>
</td>
</tr>
<tr id="row45931882113"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p11597684215"><a name="p11597684215"></a><a name="p11597684215"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p135971820216"><a name="p135971820216"></a><a name="p135971820216"></a>Not Found</p>
</td>
</tr>
<tr id="row45931088216"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p175981813217"><a name="p175981813217"></a><a name="p175981813217"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p9598986219"><a name="p9598986219"></a><a name="p9598986219"></a>Internal Server Error</p>
</td>
</tr>
</tbody>
</table>

## 错误码<a name="section1959868102118"></a>

请参见[错误码](错误码.md)。

