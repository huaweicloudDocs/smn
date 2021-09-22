# 更新Application<a name="UpdateApplication"></a>

## 功能介绍<a name="section636316015213"></a>

更新应用平台。

## 调试<a name="section1056114122524"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=SMN&api=ListTopics)中调试该接口。

## URI<a name="section836619019216"></a>

PUT /v2/\{project\_id\}/notifications/applications/\{application\_urn\}

**表 1**  路径参数

<a name="table53695012113"></a>
<table><thead align="left"><tr id="row12368170142114"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p13709020218"><a name="p13709020218"></a><a name="p13709020218"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p8370160142111"><a name="p8370160142111"></a><a name="p8370160142111"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p1937115017211"><a name="p1937115017211"></a><a name="p1937115017211"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p437214012213"><a name="p437214012213"></a><a name="p437214012213"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row83682010213"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p6373190182111"><a name="p6373190182111"></a><a name="p6373190182111"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p13741703219"><a name="p13741703219"></a><a name="p13741703219"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p113754017214"><a name="p113754017214"></a><a name="p113754017214"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p183766011215"><a name="p183766011215"></a><a name="p183766011215"></a>项目ID。</p>
<p id="p123761605211"><a name="p123761605211"></a><a name="p123761605211"></a>获取项目ID请参考<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
<tr id="row1536810002111"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p193776016212"><a name="p193776016212"></a><a name="p193776016212"></a>application_urn</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p737816002118"><a name="p737816002118"></a><a name="p737816002118"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p14379120142117"><a name="p14379120142117"></a><a name="p14379120142117"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p41777062115"><a name="p41777062115"></a><a name="p41777062115"></a>Application的唯一资源标识，可通过<a href="查询Application.md">查询Application</a>获取该标识。</p>
</td>
</tr>
</tbody>
</table>

## 请求参数<a name="section183811402219"></a>

**表 2**  请求Header参数

<a name="HeaderParameter"></a>
<table><thead align="left"><tr id="row1238315012116"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p19384140142119"><a name="p19384140142119"></a><a name="p19384140142119"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p19385405216"><a name="p19385405216"></a><a name="p19385405216"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p1738511072111"><a name="p1738511072111"></a><a name="p1738511072111"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p1738617018219"><a name="p1738617018219"></a><a name="p1738617018219"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row33838015217"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p03871109211"><a name="p03871109211"></a><a name="p03871109211"></a>X-Auth-Token</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p173880072116"><a name="p173880072116"></a><a name="p173880072116"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1638920142116"><a name="p1638920142116"></a><a name="p1638920142116"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p173902072119"><a name="p173902072119"></a><a name="p173902072119"></a>用户Token。</p>
<p id="p339115014217"><a name="p339115014217"></a><a name="p339115014217"></a>通过调用IAM服务获取用户Token接口获取（响应消息头中X-Subject-Token的值）。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  请求Body参数

<a name="requestParameter"></a>
<table><thead align="left"><tr id="row6393605211"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p73958014218"><a name="p73958014218"></a><a name="p73958014218"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p43961020213"><a name="p43961020213"></a><a name="p43961020213"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p1839714012210"><a name="p1839714012210"></a><a name="p1839714012210"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p153983016215"><a name="p153983016215"></a><a name="p153983016215"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row0393180202115"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p4399150192116"><a name="p4399150192116"></a><a name="p4399150192116"></a>platform_principal</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p0399602214"><a name="p0399602214"></a><a name="p0399602214"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p940012082119"><a name="p940012082119"></a><a name="p940012082119"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p94021014215"><a name="p94021014215"></a><a name="p94021014215"></a>对于HMS平台是APP ID，只能包含英文字母和数字，最大20个字符。</p>
<p id="p1340211019212"><a name="p1340211019212"></a><a name="p1340211019212"></a>对于苹果APNS、APNS_SandBox平台是推送证书，大小不超过8K，且是Base64编码。</p>
</td>
</tr>
<tr id="row17393190102113"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p940318002113"><a name="p940318002113"></a><a name="p940318002113"></a>platform_credential</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p84042016218"><a name="p84042016218"></a><a name="p84042016218"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p64054092111"><a name="p64054092111"></a><a name="p64054092111"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1040611022118"><a name="p1040611022118"></a><a name="p1040611022118"></a>对于HMS平台是APP SECRET， 只能包含英文字母和数字，32到64个字符。</p>
<p id="p1740710142115"><a name="p1740710142115"></a><a name="p1740710142115"></a>对于苹果APNS、APNS_SandBox平台是推送证书的私钥（private key）， 大小不超过8K，且是Base64编码。</p>
</td>
</tr>
</tbody>
</table>

## 响应参数<a name="section154091022117"></a>

**状态码： 200**

**表 4**  响应Body参数

<a name="responseParameter"></a>
<table><thead align="left"><tr id="row84118072113"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p11412110102119"><a name="p11412110102119"></a><a name="p11412110102119"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p174137020218"><a name="p174137020218"></a><a name="p174137020218"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p8414907217"><a name="p8414907217"></a><a name="p8414907217"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row84114013215"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p144158032119"><a name="p144158032119"></a><a name="p144158032119"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1641519014215"><a name="p1641519014215"></a><a name="p1641519014215"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p164164012211"><a name="p164164012211"></a><a name="p164164012211"></a>请求的唯一标识ID。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 400**

**表 5**  响应Body参数

<a name="table1841760202117"></a>
<table><thead align="left"><tr id="row84185032112"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p0419180152110"><a name="p0419180152110"></a><a name="p0419180152110"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p13421170122110"><a name="p13421170122110"></a><a name="p13421170122110"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p64222007212"><a name="p64222007212"></a><a name="p64222007212"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row9418180202113"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1423601210"><a name="p1423601210"></a><a name="p1423601210"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1442413014219"><a name="p1442413014219"></a><a name="p1442413014219"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p642550182111"><a name="p642550182111"></a><a name="p642550182111"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row7418110152114"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1542660162115"><a name="p1542660162115"></a><a name="p1542660162115"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p154277017215"><a name="p154277017215"></a><a name="p154277017215"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p124281207212"><a name="p124281207212"></a><a name="p124281207212"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row541820015216"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p9429203211"><a name="p9429203211"></a><a name="p9429203211"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p164308014213"><a name="p164308014213"></a><a name="p164308014213"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p84317012213"><a name="p84317012213"></a><a name="p84317012213"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 403**

**表 6**  响应Body参数

<a name="table1043220011212"></a>
<table><thead align="left"><tr id="row13433110102111"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p1643518022110"><a name="p1643518022110"></a><a name="p1643518022110"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p443614011218"><a name="p443614011218"></a><a name="p443614011218"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p543815042113"><a name="p543815042113"></a><a name="p543815042113"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row543310018218"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1043916019211"><a name="p1043916019211"></a><a name="p1043916019211"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p04402012214"><a name="p04402012214"></a><a name="p04402012214"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p124411704218"><a name="p124411704218"></a><a name="p124411704218"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row043350162112"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p134421908216"><a name="p134421908216"></a><a name="p134421908216"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1844320082111"><a name="p1844320082111"></a><a name="p1844320082111"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1644417052115"><a name="p1644417052115"></a><a name="p1644417052115"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row543312012119"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1144510015213"><a name="p1144510015213"></a><a name="p1144510015213"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p13446601219"><a name="p13446601219"></a><a name="p13446601219"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p15447150112117"><a name="p15447150112117"></a><a name="p15447150112117"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 404**

**表 7**  响应Body参数

<a name="table244919002110"></a>
<table><thead align="left"><tr id="row4450200132118"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p11452140112119"><a name="p11452140112119"></a><a name="p11452140112119"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p545360122110"><a name="p545360122110"></a><a name="p545360122110"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p1945450152111"><a name="p1945450152111"></a><a name="p1945450152111"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row8450307216"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1045513082112"><a name="p1045513082112"></a><a name="p1045513082112"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1345612052114"><a name="p1345612052114"></a><a name="p1345612052114"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p445715092113"><a name="p445715092113"></a><a name="p445715092113"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row445060132110"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p545870192119"><a name="p545870192119"></a><a name="p545870192119"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1545813012116"><a name="p1545813012116"></a><a name="p1545813012116"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p645915072112"><a name="p645915072112"></a><a name="p645915072112"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row1045014012213"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p134601706213"><a name="p134601706213"></a><a name="p134601706213"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1246112042110"><a name="p1246112042110"></a><a name="p1246112042110"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p34629011219"><a name="p34629011219"></a><a name="p34629011219"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 500**

**表 8**  响应Body参数

<a name="table1346380142115"></a>
<table><thead align="left"><tr id="row124641100215"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p2046620018210"><a name="p2046620018210"></a><a name="p2046620018210"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p64671808216"><a name="p64671808216"></a><a name="p64671808216"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p84681307214"><a name="p84681307214"></a><a name="p84681307214"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1646411032120"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p247013012216"><a name="p247013012216"></a><a name="p247013012216"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p14711209218"><a name="p14711209218"></a><a name="p14711209218"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1547260112117"><a name="p1547260112117"></a><a name="p1547260112117"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row12464200132111"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p64731902219"><a name="p64731902219"></a><a name="p64731902219"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p14474505211"><a name="p14474505211"></a><a name="p14474505211"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p114750016215"><a name="p114750016215"></a><a name="p114750016215"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row146510182111"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p64766062117"><a name="p64766062117"></a><a name="p64766062117"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1047617082111"><a name="p1047617082111"></a><a name="p1047617082111"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p647716014219"><a name="p647716014219"></a><a name="p647716014219"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

## 请求示例<a name="section8478140122113"></a>

更新应用平台

```
PUT https://{SMN_Endpoint}/v2/{project_id}/notifications/applications/{application_urn}

{
  "platform_principal" : "appId",
  "platform_credential" : "appSecret"
}
```

## 响应示例<a name="section448419012113"></a>

无

## 状态码<a name="section6485502216"></a>

<a name="status_code"></a>
<table><thead align="left"><tr id="row10486504217"><th class="cellrowborder" valign="top" width="15%" id="mcps1.1.3.1.1"><p id="p1448715042110"><a name="p1448715042110"></a><a name="p1448715042110"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="85%" id="mcps1.1.3.1.2"><p id="p9488140192117"><a name="p9488140192117"></a><a name="p9488140192117"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row648610172118"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p748919010214"><a name="p748919010214"></a><a name="p748919010214"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p14490170182112"><a name="p14490170182112"></a><a name="p14490170182112"></a>OK</p>
</td>
</tr>
<tr id="row134868052113"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p34919012211"><a name="p34919012211"></a><a name="p34919012211"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p18492180172116"><a name="p18492180172116"></a><a name="p18492180172116"></a>Bad Request</p>
</td>
</tr>
<tr id="row144861007216"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p11493502211"><a name="p11493502211"></a><a name="p11493502211"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p1449414062119"><a name="p1449414062119"></a><a name="p1449414062119"></a>Unauthorized</p>
</td>
</tr>
<tr id="row248619092118"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p1649510015213"><a name="p1649510015213"></a><a name="p1649510015213"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p1049618022111"><a name="p1049618022111"></a><a name="p1049618022111"></a>Not Found</p>
</td>
</tr>
<tr id="row15486205217"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p2049612018213"><a name="p2049612018213"></a><a name="p2049612018213"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p144977082116"><a name="p144977082116"></a><a name="p144977082116"></a>Internal Server Error</p>
</td>
</tr>
</tbody>
</table>

## 错误码<a name="section74981015216"></a>

请参见[错误码](错误码.md)。

