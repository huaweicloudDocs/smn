# 创建Application endpoint<a name="CreateApplicationEndpoint"></a>

## 功能介绍<a name="section191113612115"></a>

创建应用平台的endpoint终端。

## 调试<a name="section1056114122524"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=SMN&api=ListTopics)中调试该接口。

## URI<a name="section19121668215"></a>

POST /v2/\{project\_id\}/notifications/applications/\{application\_urn\}/endpoints

**表 1**  路径参数

<a name="table15914364211"></a>
<table><thead align="left"><tr id="row1691417611215"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p59151616219"><a name="p59151616219"></a><a name="p59151616219"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p091519613216"><a name="p091519613216"></a><a name="p091519613216"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p1591517642117"><a name="p1591517642117"></a><a name="p1591517642117"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p791646112115"><a name="p791646112115"></a><a name="p791646112115"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1091413610215"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p139162622119"><a name="p139162622119"></a><a name="p139162622119"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1891646102120"><a name="p1891646102120"></a><a name="p1891646102120"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p29160642117"><a name="p29160642117"></a><a name="p29160642117"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1917365215"><a name="p1917365215"></a><a name="p1917365215"></a>项目ID。</p>
<p id="p4568812165217"><a name="p4568812165217"></a><a name="p4568812165217"></a>获取项目ID请参考<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
<tr id="row1491417632116"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p149178610214"><a name="p149178610214"></a><a name="p149178610214"></a>application_urn</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p491886102112"><a name="p491886102112"></a><a name="p491886102112"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p16918667211"><a name="p16918667211"></a><a name="p16918667211"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p209185642117"><a name="p209185642117"></a><a name="p209185642117"></a>Application的唯一资源标识，可通过<a href="查询Application.md">查询Application</a>获取该标识。</p>
</td>
</tr>
</tbody>
</table>

## 请求参数<a name="section2918560217"></a>

**表 2**  请求Header参数

<a name="HeaderParameter"></a>
<table><thead align="left"><tr id="row13919769218"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p1092013682119"><a name="p1092013682119"></a><a name="p1092013682119"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p5920126172111"><a name="p5920126172111"></a><a name="p5920126172111"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p1992015617216"><a name="p1992015617216"></a><a name="p1992015617216"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p11921568213"><a name="p11921568213"></a><a name="p11921568213"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row139198602117"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1492117619211"><a name="p1492117619211"></a><a name="p1492117619211"></a>X-Auth-Token</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p192114612216"><a name="p192114612216"></a><a name="p192114612216"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p16922186192113"><a name="p16922186192113"></a><a name="p16922186192113"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p09221668215"><a name="p09221668215"></a><a name="p09221668215"></a>用户Token。</p>
<p id="p179226652115"><a name="p179226652115"></a><a name="p179226652115"></a>通过调用IAM服务获取用户Token接口获取（响应消息头中X-Subject-Token的值）。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  请求Body参数

<a name="requestParameter"></a>
<table><thead align="left"><tr id="row9923466215"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p13924106172116"><a name="p13924106172116"></a><a name="p13924106172116"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p1892412682118"><a name="p1892412682118"></a><a name="p1892412682118"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p89251167219"><a name="p89251167219"></a><a name="p89251167219"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p892576112120"><a name="p892576112120"></a><a name="p892576112120"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1192314615219"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p17926166192117"><a name="p17926166192117"></a><a name="p17926166192117"></a>token</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p199261661217"><a name="p199261661217"></a><a name="p199261661217"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p139275612119"><a name="p139275612119"></a><a name="p139275612119"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p109278619213"><a name="p109278619213"></a><a name="p109278619213"></a>移动应用设备token，最大长度512个字节。</p>
</td>
</tr>
<tr id="row1292346152110"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p20928206152110"><a name="p20928206152110"></a><a name="p20928206152110"></a>user_data</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p19286672112"><a name="p19286672112"></a><a name="p19286672112"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p79289622113"><a name="p79289622113"></a><a name="p79289622113"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p392819622117"><a name="p392819622117"></a><a name="p392819622117"></a>用户自定义数据，最大长度支持UTF-8编码后2048字节。</p>
</td>
</tr>
</tbody>
</table>

## 响应参数<a name="section5929560215"></a>

**状态码： 201**

**表 4**  响应Body参数

<a name="responseParameter"></a>
<table><thead align="left"><tr id="row6930166102118"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p2931156132116"><a name="p2931156132116"></a><a name="p2931156132116"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p169321612114"><a name="p169321612114"></a><a name="p169321612114"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p1093226182113"><a name="p1093226182113"></a><a name="p1093226182113"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row693014616218"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p179320692113"><a name="p179320692113"></a><a name="p179320692113"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p18933468218"><a name="p18933468218"></a><a name="p18933468218"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p15933126132116"><a name="p15933126132116"></a><a name="p15933126132116"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row1793014613210"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1393310617215"><a name="p1393310617215"></a><a name="p1393310617215"></a>endpoint_urn</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p99345612215"><a name="p99345612215"></a><a name="p99345612215"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p149342682118"><a name="p149342682118"></a><a name="p149342682118"></a>Endpoint的唯一资源标识。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 400**

**表 5**  响应Body参数

<a name="table109342610217"></a>
<table><thead align="left"><tr id="row139356622116"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p193512682114"><a name="p193512682114"></a><a name="p193512682114"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p4936265217"><a name="p4936265217"></a><a name="p4936265217"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p209361661216"><a name="p209361661216"></a><a name="p209361661216"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row99354610210"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p493696122118"><a name="p493696122118"></a><a name="p493696122118"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p11937186192113"><a name="p11937186192113"></a><a name="p11937186192113"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p59378602114"><a name="p59378602114"></a><a name="p59378602114"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row1935126172111"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p093719615212"><a name="p093719615212"></a><a name="p093719615212"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1093819682118"><a name="p1093819682118"></a><a name="p1093819682118"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p893816122112"><a name="p893816122112"></a><a name="p893816122112"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row1935364218"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p493810602114"><a name="p493810602114"></a><a name="p493810602114"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p2093915611219"><a name="p2093915611219"></a><a name="p2093915611219"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p129395692119"><a name="p129395692119"></a><a name="p129395692119"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 403**

**表 6**  响应Body参数

<a name="table894012642114"></a>
<table><thead align="left"><tr id="row149404610216"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p15941061212"><a name="p15941061212"></a><a name="p15941061212"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p89421665218"><a name="p89421665218"></a><a name="p89421665218"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p5942767218"><a name="p5942767218"></a><a name="p5942767218"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row89401462218"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p59439622119"><a name="p59439622119"></a><a name="p59439622119"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p49431263217"><a name="p49431263217"></a><a name="p49431263217"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p89431964213"><a name="p89431964213"></a><a name="p89431964213"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row1294010692115"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p594446172117"><a name="p594446172117"></a><a name="p594446172117"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p694436132115"><a name="p694436132115"></a><a name="p694436132115"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p5945186182115"><a name="p5945186182115"></a><a name="p5945186182115"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row394015642111"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p169452610213"><a name="p169452610213"></a><a name="p169452610213"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p79451620214"><a name="p79451620214"></a><a name="p79451620214"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p20945764216"><a name="p20945764216"></a><a name="p20945764216"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 404**

**表 7**  响应Body参数

<a name="table69463611213"></a>
<table><thead align="left"><tr id="row59461363219"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p169477616212"><a name="p169477616212"></a><a name="p169477616212"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p594814610214"><a name="p594814610214"></a><a name="p594814610214"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p294814610213"><a name="p294814610213"></a><a name="p294814610213"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row894614642115"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p99481964219"><a name="p99481964219"></a><a name="p99481964219"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1194819682110"><a name="p1194819682110"></a><a name="p1194819682110"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p29491061213"><a name="p29491061213"></a><a name="p29491061213"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row594615618216"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p594911617214"><a name="p594911617214"></a><a name="p594911617214"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p6949163218"><a name="p6949163218"></a><a name="p6949163218"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1194917616218"><a name="p1194917616218"></a><a name="p1194917616218"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row9947960215"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p7950968215"><a name="p7950968215"></a><a name="p7950968215"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p39508619211"><a name="p39508619211"></a><a name="p39508619211"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1395012682113"><a name="p1395012682113"></a><a name="p1395012682113"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 500**

**表 8**  响应Body参数

<a name="table14951166152113"></a>
<table><thead align="left"><tr id="row79518618213"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p595217619212"><a name="p595217619212"></a><a name="p595217619212"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p79535619218"><a name="p79535619218"></a><a name="p79535619218"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p119541692118"><a name="p119541692118"></a><a name="p119541692118"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row3951664217"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p11954176162110"><a name="p11954176162110"></a><a name="p11954176162110"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p159551367215"><a name="p159551367215"></a><a name="p159551367215"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p159551468211"><a name="p159551468211"></a><a name="p159551468211"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row11951196102114"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p895611672117"><a name="p895611672117"></a><a name="p895611672117"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1695696122114"><a name="p1695696122114"></a><a name="p1695696122114"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p209567614218"><a name="p209567614218"></a><a name="p209567614218"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row1295114616215"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p9956106192112"><a name="p9956106192112"></a><a name="p9956106192112"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p9957864211"><a name="p9957864211"></a><a name="p9957864211"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p395786162117"><a name="p395786162117"></a><a name="p395786162117"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

## 请求示例<a name="section119571569214"></a>

创建Application endpoint

```
POST https://{SMN_Endpoint}/v2/{project_id}/notifications/applications/{application_urn}/endpoints

{
  "token" : "3708232124742383445",
  "user_data" : "This is token for user001"
}
```

## 响应示例<a name="section595919632113"></a>

无

## 状态码<a name="section7959867216"></a>

<a name="status_code"></a>
<table><thead align="left"><tr id="row17960863214"><th class="cellrowborder" valign="top" width="15%" id="mcps1.1.3.1.1"><p id="p18961667217"><a name="p18961667217"></a><a name="p18961667217"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="85%" id="mcps1.1.3.1.2"><p id="p796116612112"><a name="p796116612112"></a><a name="p796116612112"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1396014622111"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p1496215619218"><a name="p1496215619218"></a><a name="p1496215619218"></a>201</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p139625632114"><a name="p139625632114"></a><a name="p139625632114"></a>OK</p>
</td>
</tr>
<tr id="row296014612210"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p1696310610214"><a name="p1696310610214"></a><a name="p1696310610214"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p096320642116"><a name="p096320642116"></a><a name="p096320642116"></a>Bad Request</p>
</td>
</tr>
<tr id="row1196076202112"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p39631369216"><a name="p39631369216"></a><a name="p39631369216"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p169641862217"><a name="p169641862217"></a><a name="p169641862217"></a>Unauthorized</p>
</td>
</tr>
<tr id="row19961868213"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p2964186152110"><a name="p2964186152110"></a><a name="p2964186152110"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p1896418692114"><a name="p1896418692114"></a><a name="p1896418692114"></a>Not Found</p>
</td>
</tr>
<tr id="row19615614217"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p11965465218"><a name="p11965465218"></a><a name="p11965465218"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p49653619216"><a name="p49653619216"></a><a name="p49653619216"></a>Internal Server Error</p>
</td>
</tr>
</tbody>
</table>

## 错误码<a name="section1396515612216"></a>

请参见[错误码](错误码.md)。

