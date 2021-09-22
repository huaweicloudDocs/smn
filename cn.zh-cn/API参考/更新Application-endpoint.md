# 更新Application endpoint<a name="UpdateApplicationEndpoint"></a>

## 功能介绍<a name="section66781815215"></a>

更新设备属性。

## 调试<a name="section1056114122524"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=SMN&api=ListTopics)中调试该接口。

## URI<a name="section66804818215"></a>

PUT /v2/\{project\_id\}/notifications/endpoints/\{endpoint\_urn\}

**表 1**  路径参数

<a name="table1268216812215"></a>
<table><thead align="left"><tr id="row1168298142110"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p668316817218"><a name="p668316817218"></a><a name="p668316817218"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p126839802111"><a name="p126839802111"></a><a name="p126839802111"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p56836816219"><a name="p56836816219"></a><a name="p56836816219"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p1068416818211"><a name="p1068416818211"></a><a name="p1068416818211"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row76821187215"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p15684158182119"><a name="p15684158182119"></a><a name="p15684158182119"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p36851881218"><a name="p36851881218"></a><a name="p36851881218"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1668688112114"><a name="p1668688112114"></a><a name="p1668688112114"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p11686168102117"><a name="p11686168102117"></a><a name="p11686168102117"></a>项目ID。</p>
<p id="p4568812165217"><a name="p4568812165217"></a><a name="p4568812165217"></a>获取项目ID请参考<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
<tr id="row2068211852118"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p6687586216"><a name="p6687586216"></a><a name="p6687586216"></a>endpoint_urn</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p19688168162114"><a name="p19688168162114"></a><a name="p19688168162114"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p136881789211"><a name="p136881789211"></a><a name="p136881789211"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1368938162114"><a name="p1368938162114"></a><a name="p1368938162114"></a>Endpoint的唯一资源标识，可通过<a href="查询Application的Endpoint列表.md">查询Application的Endpoint列表</a>获取该标识。</p>
</td>
</tr>
</tbody>
</table>

## 请求参数<a name="section1469017822116"></a>

**表 2**  请求Header参数

<a name="HeaderParameter"></a>
<table><thead align="left"><tr id="row66918814214"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p26921689211"><a name="p26921689211"></a><a name="p26921689211"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p96939862112"><a name="p96939862112"></a><a name="p96939862112"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p5693198172119"><a name="p5693198172119"></a><a name="p5693198172119"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p6694982213"><a name="p6694982213"></a><a name="p6694982213"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row669111832120"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p16941842118"><a name="p16941842118"></a><a name="p16941842118"></a>X-Auth-Token</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p15695485219"><a name="p15695485219"></a><a name="p15695485219"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p20695128152112"><a name="p20695128152112"></a><a name="p20695128152112"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p16696138182119"><a name="p16696138182119"></a><a name="p16696138182119"></a>用户Token。</p>
<p id="p969648142117"><a name="p969648142117"></a><a name="p969648142117"></a>通过调用IAM服务获取用户Token接口获取（响应消息头中X-Subject-Token的值）。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  请求Body参数

<a name="requestParameter"></a>
<table><thead align="left"><tr id="row66972813219"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p6698986214"><a name="p6698986214"></a><a name="p6698986214"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p869917852116"><a name="p869917852116"></a><a name="p869917852116"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p2699158162115"><a name="p2699158162115"></a><a name="p2699158162115"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p117001882119"><a name="p117001882119"></a><a name="p117001882119"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row15697128122119"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1670016842114"><a name="p1670016842114"></a><a name="p1670016842114"></a>enabled</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p770118811211"><a name="p770118811211"></a><a name="p770118811211"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p137021812110"><a name="p137021812110"></a><a name="p137021812110"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1270210832118"><a name="p1270210832118"></a><a name="p1270210832118"></a>设备是否可用，值为true或false字符串。</p>
</td>
</tr>
<tr id="row1669708132113"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p157031186217"><a name="p157031186217"></a><a name="p157031186217"></a>user_data</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p570414832112"><a name="p570414832112"></a><a name="p570414832112"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p670416822117"><a name="p670416822117"></a><a name="p670416822117"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p157052081216"><a name="p157052081216"></a><a name="p157052081216"></a>用户自定义数据，最大长度支持UTF-8编码后2048字节。</p>
</td>
</tr>
</tbody>
</table>

## 响应参数<a name="section07064892119"></a>

**状态码： 200**

**表 4**  响应Body参数

<a name="responseParameter"></a>
<table><thead align="left"><tr id="row137074832113"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p1070838182112"><a name="p1070838182112"></a><a name="p1070838182112"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p207095822116"><a name="p207095822116"></a><a name="p207095822116"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p137097852113"><a name="p137097852113"></a><a name="p137097852113"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1070712814214"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p17710178132119"><a name="p17710178132119"></a><a name="p17710178132119"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p371010812218"><a name="p371010812218"></a><a name="p371010812218"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p167112089215"><a name="p167112089215"></a><a name="p167112089215"></a>请求的唯一标识ID。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 400**

**表 5**  响应Body参数

<a name="table11711148152116"></a>
<table><thead align="left"><tr id="row1971219815214"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p971513810216"><a name="p971513810216"></a><a name="p971513810216"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p6715108142114"><a name="p6715108142114"></a><a name="p6715108142114"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p197168817210"><a name="p197168817210"></a><a name="p197168817210"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row57128892115"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p07161184210"><a name="p07161184210"></a><a name="p07161184210"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p4717128162115"><a name="p4717128162115"></a><a name="p4717128162115"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p127171892111"><a name="p127171892111"></a><a name="p127171892111"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row0712158182112"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p77185818218"><a name="p77185818218"></a><a name="p77185818218"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p17181382215"><a name="p17181382215"></a><a name="p17181382215"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p5719198152112"><a name="p5719198152112"></a><a name="p5719198152112"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row571216842110"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1071938102120"><a name="p1071938102120"></a><a name="p1071938102120"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p2720138122115"><a name="p2720138122115"></a><a name="p2720138122115"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p5721108172111"><a name="p5721108172111"></a><a name="p5721108172111"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 403**

**表 6**  响应Body参数

<a name="table177218817216"></a>
<table><thead align="left"><tr id="row572268112116"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p9723178142110"><a name="p9723178142110"></a><a name="p9723178142110"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p1972419813213"><a name="p1972419813213"></a><a name="p1972419813213"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p6725682215"><a name="p6725682215"></a><a name="p6725682215"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row2722782216"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p15726985213"><a name="p15726985213"></a><a name="p15726985213"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p127262822119"><a name="p127262822119"></a><a name="p127262822119"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1172738192111"><a name="p1172738192111"></a><a name="p1172738192111"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row77223862111"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p10727384217"><a name="p10727384217"></a><a name="p10727384217"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p12728389214"><a name="p12728389214"></a><a name="p12728389214"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p137289820210"><a name="p137289820210"></a><a name="p137289820210"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row4722387211"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p147292819213"><a name="p147292819213"></a><a name="p147292819213"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p07300813211"><a name="p07300813211"></a><a name="p07300813211"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p77300817212"><a name="p77300817212"></a><a name="p77300817212"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 404**

**表 7**  响应Body参数

<a name="table5730881217"></a>
<table><thead align="left"><tr id="row157318819217"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p773215812117"><a name="p773215812117"></a><a name="p773215812117"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p3733481218"><a name="p3733481218"></a><a name="p3733481218"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p127331681215"><a name="p127331681215"></a><a name="p127331681215"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1073117819218"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p197341888214"><a name="p197341888214"></a><a name="p197341888214"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p37355811215"><a name="p37355811215"></a><a name="p37355811215"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1773519832118"><a name="p1773519832118"></a><a name="p1773519832118"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row1673114862111"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p27361283214"><a name="p27361283214"></a><a name="p27361283214"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p97366820212"><a name="p97366820212"></a><a name="p97366820212"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p2073719813219"><a name="p2073719813219"></a><a name="p2073719813219"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row473119842117"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1773712819214"><a name="p1773712819214"></a><a name="p1773712819214"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p67382852110"><a name="p67382852110"></a><a name="p67382852110"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p273978152120"><a name="p273978152120"></a><a name="p273978152120"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 500**

**表 8**  响应Body参数

<a name="table1473920852119"></a>
<table><thead align="left"><tr id="row207405810218"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p107416892116"><a name="p107416892116"></a><a name="p107416892116"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p574217812116"><a name="p574217812116"></a><a name="p574217812116"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p674220812219"><a name="p674220812219"></a><a name="p674220812219"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row474048142117"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p18743785211"><a name="p18743785211"></a><a name="p18743785211"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p174310817219"><a name="p174310817219"></a><a name="p174310817219"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1974428192117"><a name="p1974428192117"></a><a name="p1974428192117"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row374016802120"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p117441582211"><a name="p117441582211"></a><a name="p117441582211"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p674514812112"><a name="p674514812112"></a><a name="p674514812112"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1474510812217"><a name="p1474510812217"></a><a name="p1474510812217"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row20740385214"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p174658152117"><a name="p174658152117"></a><a name="p174658152117"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p27468818214"><a name="p27468818214"></a><a name="p27468818214"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p274758102111"><a name="p274758102111"></a><a name="p274758102111"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

## 请求示例<a name="section47477811211"></a>

更新Application endpoint

```
POST https://{SMN_Endpoint}/v2/{project_id}/notifications/applications/{application_urn}/endpoints

{
  "enabled" : "false",
  "user_data" : "This is an APNS token for user001"
}
```

## 响应示例<a name="section1175115812115"></a>

无

## 状态码<a name="section187528882114"></a>

<a name="status_code"></a>
<table><thead align="left"><tr id="row1275348102115"><th class="cellrowborder" valign="top" width="15%" id="mcps1.1.3.1.1"><p id="p18754148152119"><a name="p18754148152119"></a><a name="p18754148152119"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="85%" id="mcps1.1.3.1.2"><p id="p175415812215"><a name="p175415812215"></a><a name="p175415812215"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row197531388219"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p1075517892120"><a name="p1075517892120"></a><a name="p1075517892120"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p167551689210"><a name="p167551689210"></a><a name="p167551689210"></a>OK</p>
</td>
</tr>
<tr id="row775314814218"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p1275616814219"><a name="p1275616814219"></a><a name="p1275616814219"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p167569810212"><a name="p167569810212"></a><a name="p167569810212"></a>Bad Request</p>
</td>
</tr>
<tr id="row97539892110"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p15757586211"><a name="p15757586211"></a><a name="p15757586211"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p67581886219"><a name="p67581886219"></a><a name="p67581886219"></a>Unauthorized</p>
</td>
</tr>
<tr id="row3753108152119"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p14758183215"><a name="p14758183215"></a><a name="p14758183215"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p11759884211"><a name="p11759884211"></a><a name="p11759884211"></a>Not Found</p>
</td>
</tr>
<tr id="row37530862116"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p275988182113"><a name="p275988182113"></a><a name="p275988182113"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p87601842111"><a name="p87601842111"></a><a name="p87601842111"></a>Internal Server Error</p>
</td>
</tr>
</tbody>
</table>

## 错误码<a name="section3760487213"></a>

请参见[错误码](错误码.md)。

