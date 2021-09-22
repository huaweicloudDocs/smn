# 删除Application<a name="DeleteApplication"></a>

## 功能介绍<a name="section1557042182113"></a>

删除平台应用。

## 调试<a name="section1056114122524"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=SMN&api=ListTopics)中调试该接口。

## URI<a name="section2057482142115"></a>

DELETE /v2/\{project\_id\}/notifications/applications/\{application\_urn\}

**表 1**  路径参数

<a name="table9577023219"></a>
<table><thead align="left"><tr id="row2576721217"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p145783218216"><a name="p145783218216"></a><a name="p145783218216"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p957962182117"><a name="p957962182117"></a><a name="p957962182117"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p1658112214212"><a name="p1658112214212"></a><a name="p1658112214212"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p165821210219"><a name="p165821210219"></a><a name="p165821210219"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row857612122116"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p5583162152111"><a name="p5583162152111"></a><a name="p5583162152111"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p105841213211"><a name="p105841213211"></a><a name="p105841213211"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p125859216218"><a name="p125859216218"></a><a name="p125859216218"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p125861421216"><a name="p125861421216"></a><a name="p125861421216"></a>项目ID。</p>
<p id="p4568812165217"><a name="p4568812165217"></a><a name="p4568812165217"></a>获取项目ID请参考<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
<tr id="row1457612214215"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1058852202119"><a name="p1058852202119"></a><a name="p1058852202119"></a>application_urn</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p958919217217"><a name="p958919217217"></a><a name="p958919217217"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p958992162114"><a name="p958992162114"></a><a name="p958992162114"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p16591152142120"><a name="p16591152142120"></a><a name="p16591152142120"></a>Application的唯一资源标识，可通过<a href="查询Application.md">查询Application</a>获取该标识。</p>
</td>
</tr>
</tbody>
</table>

## 请求参数<a name="section659111282115"></a>

**表 2**  请求Header参数

<a name="HeaderParameter"></a>
<table><thead align="left"><tr id="row7593172112119"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p7594121212"><a name="p7594121212"></a><a name="p7594121212"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p75966232116"><a name="p75966232116"></a><a name="p75966232116"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p105971421211"><a name="p105971421211"></a><a name="p105971421211"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p15981210215"><a name="p15981210215"></a><a name="p15981210215"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row3593225215"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p95991021218"><a name="p95991021218"></a><a name="p95991021218"></a>X-Auth-Token</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p5600921212"><a name="p5600921212"></a><a name="p5600921212"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1760122182110"><a name="p1760122182110"></a><a name="p1760122182110"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p460219282114"><a name="p460219282114"></a><a name="p460219282114"></a>用户Token。</p>
<p id="p16603162142113"><a name="p16603162142113"></a><a name="p16603162142113"></a>通过调用IAM服务获取用户Token接口获取（响应消息头中X-Subject-Token的值）。</p>
</td>
</tr>
</tbody>
</table>

## 响应参数<a name="section9604126218"></a>

**状态码： 200**

**表 3**  响应Body参数

<a name="responseParameter"></a>
<table><thead align="left"><tr id="row8607328215"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p5609132162115"><a name="p5609132162115"></a><a name="p5609132162115"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p961013242119"><a name="p961013242119"></a><a name="p961013242119"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p86106202110"><a name="p86106202110"></a><a name="p86106202110"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row14607223219"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p661116217213"><a name="p661116217213"></a><a name="p661116217213"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p96124220216"><a name="p96124220216"></a><a name="p96124220216"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1161318211211"><a name="p1161318211211"></a><a name="p1161318211211"></a>请求的唯一标识ID。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 400**

**表 4**  响应Body参数

<a name="table19615202152117"></a>
<table><thead align="left"><tr id="row06157262115"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p1861832152112"><a name="p1861832152112"></a><a name="p1861832152112"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p8619528212"><a name="p8619528212"></a><a name="p8619528212"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p26205211214"><a name="p26205211214"></a><a name="p26205211214"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row19615112162114"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p862118262113"><a name="p862118262113"></a><a name="p862118262113"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p106221524217"><a name="p106221524217"></a><a name="p106221524217"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1262312212118"><a name="p1262312212118"></a><a name="p1262312212118"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row36166242110"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p11624162112115"><a name="p11624162112115"></a><a name="p11624162112115"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1962418211219"><a name="p1962418211219"></a><a name="p1962418211219"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1762572172117"><a name="p1762572172117"></a><a name="p1762572172117"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row1361614211212"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1162602102118"><a name="p1162602102118"></a><a name="p1162602102118"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p176279210213"><a name="p176279210213"></a><a name="p176279210213"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p176281024213"><a name="p176281024213"></a><a name="p176281024213"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 403**

**表 5**  响应Body参数

<a name="table1162919211215"></a>
<table><thead align="left"><tr id="row36301222112"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p106331228218"><a name="p106331228218"></a><a name="p106331228218"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p15634202112112"><a name="p15634202112112"></a><a name="p15634202112112"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p1963514210213"><a name="p1963514210213"></a><a name="p1963514210213"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row186302210218"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p186361124211"><a name="p186361124211"></a><a name="p186361124211"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p56371929212"><a name="p56371929212"></a><a name="p56371929212"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p0638192152111"><a name="p0638192152111"></a><a name="p0638192152111"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row176306212110"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p163913214215"><a name="p163913214215"></a><a name="p163913214215"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p156401524215"><a name="p156401524215"></a><a name="p156401524215"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p126424216213"><a name="p126424216213"></a><a name="p126424216213"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row1630142202118"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p146438217219"><a name="p146438217219"></a><a name="p146438217219"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p146431823218"><a name="p146431823218"></a><a name="p146431823218"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p10645125218"><a name="p10645125218"></a><a name="p10645125218"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 404**

**表 6**  响应Body参数

<a name="table14646162122114"></a>
<table><thead align="left"><tr id="row96471727218"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p196497210216"><a name="p196497210216"></a><a name="p196497210216"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p176501029218"><a name="p176501029218"></a><a name="p176501029218"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p20651152122111"><a name="p20651152122111"></a><a name="p20651152122111"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row264712282117"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p165213272112"><a name="p165213272112"></a><a name="p165213272112"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p86549242110"><a name="p86549242110"></a><a name="p86549242110"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p176551822217"><a name="p176551822217"></a><a name="p176551822217"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row196473212216"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p17656724215"><a name="p17656724215"></a><a name="p17656724215"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p26571126214"><a name="p26571126214"></a><a name="p26571126214"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p06587218213"><a name="p06587218213"></a><a name="p06587218213"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row1647142202111"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p136583215217"><a name="p136583215217"></a><a name="p136583215217"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p965910242119"><a name="p965910242119"></a><a name="p965910242119"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p36601222116"><a name="p36601222116"></a><a name="p36601222116"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 500**

**表 7**  响应Body参数

<a name="table16662924214"></a>
<table><thead align="left"><tr id="row26631211215"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p066412232117"><a name="p066412232117"></a><a name="p066412232117"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p186651924218"><a name="p186651924218"></a><a name="p186651924218"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p7666182102112"><a name="p7666182102112"></a><a name="p7666182102112"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row9663162172110"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1766772112119"><a name="p1766772112119"></a><a name="p1766772112119"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p866812232115"><a name="p866812232115"></a><a name="p866812232115"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1669142202111"><a name="p1669142202111"></a><a name="p1669142202111"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row12663429213"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p126701222211"><a name="p126701222211"></a><a name="p126701222211"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p176710218212"><a name="p176710218212"></a><a name="p176710218212"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p467113218214"><a name="p467113218214"></a><a name="p467113218214"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row866382102112"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p067210212116"><a name="p067210212116"></a><a name="p067210212116"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p16731225219"><a name="p16731225219"></a><a name="p16731225219"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p46741232111"><a name="p46741232111"></a><a name="p46741232111"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

## 请求示例<a name="section867515262110"></a>

删除平台应用

```
DELETE https://{SMN_Endpoint}/v2/{project_id}/notifications/applications/{application_urn}

{
  "platform_principal" : "appId",
  "platform_credential" : "appSecret"
}
```

## 响应示例<a name="section1868215213213"></a>

无

## 状态码<a name="section86831623218"></a>

<a name="status_code"></a>
<table><thead align="left"><tr id="row1968514212118"><th class="cellrowborder" valign="top" width="15%" id="mcps1.1.3.1.1"><p id="p1568610215214"><a name="p1568610215214"></a><a name="p1568610215214"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="85%" id="mcps1.1.3.1.2"><p id="p36871528218"><a name="p36871528218"></a><a name="p36871528218"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row146850217210"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p1468914292110"><a name="p1468914292110"></a><a name="p1468914292110"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p269018292114"><a name="p269018292114"></a><a name="p269018292114"></a>OK</p>
</td>
</tr>
<tr id="row11685927210"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p1169111215215"><a name="p1169111215215"></a><a name="p1169111215215"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p17693923218"><a name="p17693923218"></a><a name="p17693923218"></a>Bad Request</p>
</td>
</tr>
<tr id="row186859219215"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p169412213216"><a name="p169412213216"></a><a name="p169412213216"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p66952211211"><a name="p66952211211"></a><a name="p66952211211"></a>Unauthorized</p>
</td>
</tr>
<tr id="row166859222111"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p106966262110"><a name="p106966262110"></a><a name="p106966262110"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p156971527211"><a name="p156971527211"></a><a name="p156971527211"></a>Not Found</p>
</td>
</tr>
<tr id="row4685725217"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p1369811282115"><a name="p1369811282115"></a><a name="p1369811282115"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p2699102192118"><a name="p2699102192118"></a><a name="p2699102192118"></a>Internal Server Error</p>
</td>
</tr>
</tbody>
</table>

## 错误码<a name="section77006232117"></a>

请参见[错误码](错误码.md)。

