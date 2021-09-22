# 查询Application属性<a name="ListApplicationAttributes"></a>

## 功能介绍<a name="section015815022119"></a>

获取应用平台属性。

## 调试<a name="section1056114122524"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=SMN&api=ListTopics)中调试该接口。

## URI<a name="section21621606211"></a>

GET /v2/\{project\_id\}/notifications/applications/\{application\_urn\}

**表 1**  路径参数

<a name="table1516612011214"></a>
<table><thead align="left"><tr id="row181651304214"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p016680122116"><a name="p016680122116"></a><a name="p016680122116"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p81671802218"><a name="p81671802218"></a><a name="p81671802218"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p12168802217"><a name="p12168802217"></a><a name="p12168802217"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p1116970182117"><a name="p1116970182117"></a><a name="p1116970182117"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row416510012217"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p51705072112"><a name="p51705072112"></a><a name="p51705072112"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p017115014219"><a name="p017115014219"></a><a name="p017115014219"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p4172501214"><a name="p4172501214"></a><a name="p4172501214"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p171731301217"><a name="p171731301217"></a><a name="p171731301217"></a>项目ID。</p>
<p id="p4568812165217"><a name="p4568812165217"></a><a name="p4568812165217"></a>获取项目ID请参考<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
<tr id="row616512015212"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p4174504218"><a name="p4174504218"></a><a name="p4174504218"></a>application_urn</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1217516017219"><a name="p1217516017219"></a><a name="p1217516017219"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p217615002115"><a name="p217615002115"></a><a name="p217615002115"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p41777062115"><a name="p41777062115"></a><a name="p41777062115"></a>Application的唯一资源标识，可通过<a href="查询Application.md">查询Application</a>获取该标识。</p>
</td>
</tr>
</tbody>
</table>

## 请求参数<a name="section151780017216"></a>

**表 2**  请求Header参数

<a name="HeaderParameter"></a>
<table><thead align="left"><tr id="row01801407213"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p111827013218"><a name="p111827013218"></a><a name="p111827013218"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p1218350132113"><a name="p1218350132113"></a><a name="p1218350132113"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p418412092113"><a name="p418412092113"></a><a name="p418412092113"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p61851101218"><a name="p61851101218"></a><a name="p61851101218"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row818011011212"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p111857011212"><a name="p111857011212"></a><a name="p111857011212"></a>X-Auth-Token</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p31869018215"><a name="p31869018215"></a><a name="p31869018215"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p13187160102119"><a name="p13187160102119"></a><a name="p13187160102119"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p191881016214"><a name="p191881016214"></a><a name="p191881016214"></a>用户Token。</p>
<p id="p91883042114"><a name="p91883042114"></a><a name="p91883042114"></a>通过调用IAM服务获取用户Token接口获取（响应消息头中X-Subject-Token的值）。</p>
</td>
</tr>
</tbody>
</table>

## 响应参数<a name="section161917012214"></a>

**状态码： 200**

**表 3**  响应Body参数

<a name="responseParameter"></a>
<table><thead align="left"><tr id="row319370152115"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p81951014211"><a name="p81951014211"></a><a name="p81951014211"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p3196130132116"><a name="p3196130132116"></a><a name="p3196130132116"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p71971008218"><a name="p71971008218"></a><a name="p71971008218"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1193110122111"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p111975010219"><a name="p111975010219"></a><a name="p111975010219"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1719810019216"><a name="p1719810019216"></a><a name="p1719810019216"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1519915042115"><a name="p1519915042115"></a><a name="p1519915042115"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row819350182118"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p62006082115"><a name="p62006082115"></a><a name="p62006082115"></a>application_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p122013092117"><a name="p122013092117"></a><a name="p122013092117"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p42021605214"><a name="p42021605214"></a><a name="p42021605214"></a>Application的唯一标识ID。</p>
</td>
</tr>
<tr id="row8193000215"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p120390102116"><a name="p120390102116"></a><a name="p120390102116"></a>attributes</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p72040012214"><a name="p72040012214"></a><a name="p72040012214"></a><a href="#response_ApplicationAttribute">表4</a> object</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p8205170132112"><a name="p8205170132112"></a><a name="p8205170132112"></a>-</p>
</td>
</tr>
</tbody>
</table>

**表 4**  ApplicationAttribute

<a name="response_ApplicationAttribute"></a>
<table><thead align="left"><tr id="row18175164203517"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p0176134113518"><a name="p0176134113518"></a><a name="p0176134113518"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p1317618417355"><a name="p1317618417355"></a><a name="p1317618417355"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p3177174103520"><a name="p3177174103520"></a><a name="p3177174103520"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1317511412350"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p141776453514"><a name="p141776453514"></a><a name="p141776453514"></a>enabled</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p017764193517"><a name="p017764193517"></a><a name="p017764193517"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p51788453517"><a name="p51788453517"></a><a name="p51788453517"></a>应用平台是否启用。</p>
</td>
</tr>
<tr id="row21751740356"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1917894173516"><a name="p1917894173516"></a><a name="p1917894173516"></a>apple_certificate_expiration_date</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p131788443516"><a name="p131788443516"></a><a name="p131788443516"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p161795414355"><a name="p161795414355"></a><a name="p161795414355"></a>苹果证书过期时间，APNS、APNS_SANDBOX平台特有属性。时间格式为UTC时间，YYYY-MM-DDTHH:MM:SSZ。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 400**

**表 5**  响应Body参数

<a name="table192068016213"></a>
<table><thead align="left"><tr id="row1520613012116"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p1620850122113"><a name="p1620850122113"></a><a name="p1620850122113"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p920918018214"><a name="p920918018214"></a><a name="p920918018214"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p52108052111"><a name="p52108052111"></a><a name="p52108052111"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row520616011213"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p10212150162118"><a name="p10212150162118"></a><a name="p10212150162118"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p321319052110"><a name="p321319052110"></a><a name="p321319052110"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p16215408211"><a name="p16215408211"></a><a name="p16215408211"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row112073092110"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1217406218"><a name="p1217406218"></a><a name="p1217406218"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p11218160132110"><a name="p11218160132110"></a><a name="p11218160132110"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p132181707212"><a name="p132181707212"></a><a name="p132181707212"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row6207202210"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1921918013215"><a name="p1921918013215"></a><a name="p1921918013215"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p422017082114"><a name="p422017082114"></a><a name="p422017082114"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1722118082119"><a name="p1722118082119"></a><a name="p1722118082119"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 403**

**表 6**  响应Body参数

<a name="table1422310018211"></a>
<table><thead align="left"><tr id="row152231903211"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p1522520112115"><a name="p1522520112115"></a><a name="p1522520112115"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p17226806211"><a name="p17226806211"></a><a name="p17226806211"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p122770102118"><a name="p122770102118"></a><a name="p122770102118"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row152240014217"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p522815014210"><a name="p522815014210"></a><a name="p522815014210"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1622919015218"><a name="p1622919015218"></a><a name="p1622919015218"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p62301009215"><a name="p62301009215"></a><a name="p62301009215"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row1622460182111"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p172303020211"><a name="p172303020211"></a><a name="p172303020211"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1223150112110"><a name="p1223150112110"></a><a name="p1223150112110"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p182321109215"><a name="p182321109215"></a><a name="p182321109215"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row14224190162111"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p102331209211"><a name="p102331209211"></a><a name="p102331209211"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p192344062117"><a name="p192344062117"></a><a name="p192344062117"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p123519017217"><a name="p123519017217"></a><a name="p123519017217"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 404**

**表 7**  响应Body参数

<a name="table2023615010210"></a>
<table><thead align="left"><tr id="row223618012118"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p1823812014212"><a name="p1823812014212"></a><a name="p1823812014212"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p172391102215"><a name="p172391102215"></a><a name="p172391102215"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p172400082110"><a name="p172400082110"></a><a name="p172400082110"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row02378012214"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p15241170102117"><a name="p15241170102117"></a><a name="p15241170102117"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p324211010214"><a name="p324211010214"></a><a name="p324211010214"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p14242130152117"><a name="p14242130152117"></a><a name="p14242130152117"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row22374062118"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p324313012115"><a name="p324313012115"></a><a name="p324313012115"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p72441805216"><a name="p72441805216"></a><a name="p72441805216"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p16245409217"><a name="p16245409217"></a><a name="p16245409217"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row523717022114"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p52450042118"><a name="p52450042118"></a><a name="p52450042118"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p152469022120"><a name="p152469022120"></a><a name="p152469022120"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1524710112114"><a name="p1524710112114"></a><a name="p1524710112114"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 500**

**表 8**  响应Body参数

<a name="table72485011210"></a>
<table><thead align="left"><tr id="row19248505219"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p825015016219"><a name="p825015016219"></a><a name="p825015016219"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p162519010217"><a name="p162519010217"></a><a name="p162519010217"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p925111018218"><a name="p925111018218"></a><a name="p925111018218"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row14248130132120"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p8252200192116"><a name="p8252200192116"></a><a name="p8252200192116"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p62535062116"><a name="p62535062116"></a><a name="p62535062116"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p142546002112"><a name="p142546002112"></a><a name="p142546002112"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row524818092118"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p17255205218"><a name="p17255205218"></a><a name="p17255205218"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1725660202110"><a name="p1725660202110"></a><a name="p1725660202110"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p425618011210"><a name="p425618011210"></a><a name="p425618011210"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row22488015217"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p112571011211"><a name="p112571011211"></a><a name="p112571011211"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p62582020218"><a name="p62582020218"></a><a name="p62582020218"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p122592052116"><a name="p122592052116"></a><a name="p122592052116"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

## 请求示例<a name="section82594011215"></a>

```
GET https://{SMN_Endpoint}/v2/{project_id}/notifications/applications/{application_urn}

null
```

## 响应示例<a name="section826312015211"></a>

**状态码： 200**

OK

```
{
  "request_id" : "6a63a18b8bab40ffb71ebd9cb80d0085",
  "application_id" : "b1b8643dc12b4g77ad6e35a16003119b",
  "attributes" : {
    "enabled" : "true",
    "apple_certificate_expiration_date" : "2018-03-09T12:21:40Z"
  }
}
```

## 状态码<a name="section4270130102117"></a>

<a name="status_code"></a>
<table><thead align="left"><tr id="row9272702211"><th class="cellrowborder" valign="top" width="15%" id="mcps1.1.3.1.1"><p id="p927313012219"><a name="p927313012219"></a><a name="p927313012219"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="85%" id="mcps1.1.3.1.2"><p id="p16274170152117"><a name="p16274170152117"></a><a name="p16274170152117"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row92721705210"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p11275309212"><a name="p11275309212"></a><a name="p11275309212"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p182765022111"><a name="p182765022111"></a><a name="p182765022111"></a>OK</p>
</td>
</tr>
<tr id="row227200182116"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p5277180132114"><a name="p5277180132114"></a><a name="p5277180132114"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p162771509214"><a name="p162771509214"></a><a name="p162771509214"></a>Bad Request</p>
</td>
</tr>
<tr id="row22725010218"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p1427812019216"><a name="p1427812019216"></a><a name="p1427812019216"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p13279130142115"><a name="p13279130142115"></a><a name="p13279130142115"></a>Unauthorized</p>
</td>
</tr>
<tr id="row1227219052115"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p11280200112111"><a name="p11280200112111"></a><a name="p11280200112111"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p1828170132120"><a name="p1828170132120"></a><a name="p1828170132120"></a>Not Found</p>
</td>
</tr>
<tr id="row172725017215"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p128218092113"><a name="p128218092113"></a><a name="p128218092113"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p528312022116"><a name="p528312022116"></a><a name="p528312022116"></a>Internal Server Error</p>
</td>
</tr>
</tbody>
</table>

## 错误码<a name="section102847020211"></a>

请参见[错误码](错误码.md)。

