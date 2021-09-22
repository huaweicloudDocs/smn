# 查询SMN API V2版本信息<a name="ListVersion"></a>

## 功能介绍<a name="section29182142113"></a>

查询SMN API V2版本信息。

## 调试<a name="section1056114122524"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=SMN&api=ListTopics)中调试该接口。

## URI<a name="section913721102118"></a>

GET /\{api\_version\}

**表 1**  路径参数

<a name="table101742112212"></a>
<table><thead align="left"><tr id="row141612114218"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p20184213216"><a name="p20184213216"></a><a name="p20184213216"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p171919219216"><a name="p171919219216"></a><a name="p171919219216"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p32012132116"><a name="p32012132116"></a><a name="p32012132116"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p2215211214"><a name="p2215211214"></a><a name="p2215211214"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1517172162117"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p02211214217"><a name="p02211214217"></a><a name="p02211214217"></a>api_version</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p62202132115"><a name="p62202132115"></a><a name="p62202132115"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p92372111211"><a name="p92372111211"></a><a name="p92372111211"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1124192119216"><a name="p1124192119216"></a><a name="p1124192119216"></a>待查询版本号。当前仅支持v2。</p>
</td>
</tr>
</tbody>
</table>

## 请求参数<a name="section1625521182115"></a>

**表 2**  请求Header参数

<a name="HeaderParameter"></a>
<table><thead align="left"><tr id="row112692122114"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p3288219215"><a name="p3288219215"></a><a name="p3288219215"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p1929142118213"><a name="p1929142118213"></a><a name="p1929142118213"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p130821102113"><a name="p130821102113"></a><a name="p130821102113"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p163182132110"><a name="p163182132110"></a><a name="p163182132110"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row2261721112117"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p63392112114"><a name="p63392112114"></a><a name="p63392112114"></a>X-Auth-Token</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p123417215218"><a name="p123417215218"></a><a name="p123417215218"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p12368212215"><a name="p12368212215"></a><a name="p12368212215"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1137121142111"><a name="p1137121142111"></a><a name="p1137121142111"></a>用户Token。</p>
<p id="p73716213219"><a name="p73716213219"></a><a name="p73716213219"></a>通过调用IAM服务获取用户Token接口获取（响应消息头中X-Subject-Token的值）。</p>
</td>
</tr>
</tbody>
</table>

## 响应参数<a name="section14401521192112"></a>

**状态码： 200**

**表 3**  响应Body参数

<a name="responseParameter"></a>
<table><thead align="left"><tr id="row1241102122115"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p543721182114"><a name="p543721182114"></a><a name="p543721182114"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p1444202116219"><a name="p1444202116219"></a><a name="p1444202116219"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p1746112110211"><a name="p1746112110211"></a><a name="p1746112110211"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row841821102110"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p84742142110"><a name="p84742142110"></a><a name="p84742142110"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p648921192112"><a name="p648921192112"></a><a name="p648921192112"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p09481736355"><a name="p09481736355"></a><a name="p09481736355"></a>描述version相关对象的列表。</p>
</td>
</tr>
</tbody>
</table>

**表 4**  VersionItem

<a name="response_VersionItem"></a>
<table><thead align="left"><tr id="row115162142118"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p14528214210"><a name="p14528214210"></a><a name="p14528214210"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p1354152192112"><a name="p1354152192112"></a><a name="p1354152192112"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p055102172115"><a name="p055102172115"></a><a name="p055102172115"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row95192117212"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p05642111212"><a name="p05642111212"></a><a name="p05642111212"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p35717216215"><a name="p35717216215"></a><a name="p35717216215"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1058421182114"><a name="p1058421182114"></a><a name="p1058421182114"></a>版本ID（版本号），如v2。</p>
</td>
</tr>
<tr id="row35112217215"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p05972152114"><a name="p05972152114"></a><a name="p05972152114"></a>min_version</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p2060102132117"><a name="p2060102132117"></a><a name="p2060102132117"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p26116218216"><a name="p26116218216"></a><a name="p26116218216"></a>若该版本API支持微版本，则返回支持的最小微版本号；若不支持微版本，则返回空。</p>
</td>
</tr>
<tr id="row15111211213"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1762172152116"><a name="p1762172152116"></a><a name="p1762172152116"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p36332116218"><a name="p36332116218"></a><a name="p36332116218"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p9641821102118"><a name="p9641821102118"></a><a name="p9641821102118"></a>版本状态，为如下3种：</p>
<p id="p365112119219"><a name="p365112119219"></a><a name="p365112119219"></a>CURRENT：表示该版本为主推版本。</p>
<p id="p66682110215"><a name="p66682110215"></a><a name="p66682110215"></a>SUPPORTED：表示为老版本，但是现在还继续支持。</p>
<p id="p186613211213"><a name="p186613211213"></a><a name="p186613211213"></a>DEPRECATED：表示为废弃版本，存在后续删除的可能。</p>
</td>
</tr>
<tr id="row1351202192119"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p96782192112"><a name="p96782192112"></a><a name="p96782192112"></a>updated</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1568921122114"><a name="p1568921122114"></a><a name="p1568921122114"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1069142111214"><a name="p1069142111214"></a><a name="p1069142111214"></a>版本发布时间，要求用UTC时间格式表示。如v2发布的时间2014-06-28T12:20:21Z。</p>
</td>
</tr>
<tr id="row3511221192113"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p10701521142116"><a name="p10701521142116"></a><a name="p10701521142116"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p117172142116"><a name="p117172142116"></a><a name="p117172142116"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1672321172117"><a name="p1672321172117"></a><a name="p1672321172117"></a>若该版本API支持微版本，则返回支持的最大微版本号；若不支持微版本，则返回空。</p>
</td>
</tr>
<tr id="row1851102111219"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p8741121122110"><a name="p8741121122110"></a><a name="p8741121122110"></a>links</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p87532122116"><a name="p87532122116"></a><a name="p87532122116"></a>Array of <a href="#response_LinksItem">LinksItem</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1276821122119"><a name="p1276821122119"></a><a name="p1276821122119"></a>API的URL地址。</p>
</td>
</tr>
</tbody>
</table>

**表 5**  LinksItem

<a name="response_LinksItem"></a>
<table><thead align="left"><tr id="row17786217212"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p77913214217"><a name="p77913214217"></a><a name="p77913214217"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p108052182111"><a name="p108052182111"></a><a name="p108052182111"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p168282111217"><a name="p168282111217"></a><a name="p168282111217"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row15786214211"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p118313212219"><a name="p118313212219"></a><a name="p118313212219"></a>href</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1084421152116"><a name="p1084421152116"></a><a name="p1084421152116"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p168716214217"><a name="p168716214217"></a><a name="p168716214217"></a>对应快捷链接。</p>
</td>
</tr>
<tr id="row57862122115"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1988821132112"><a name="p1988821132112"></a><a name="p1988821132112"></a>rel</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p589102118215"><a name="p589102118215"></a><a name="p589102118215"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p15911821122117"><a name="p15911821122117"></a><a name="p15911821122117"></a>快捷链接标记名称。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 400**

**表 6**  响应Body参数

<a name="table1892202112119"></a>
<table><thead align="left"><tr id="row393152110218"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p209532118216"><a name="p209532118216"></a><a name="p209532118216"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p11961521182111"><a name="p11961521182111"></a><a name="p11961521182111"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p1197221102113"><a name="p1197221102113"></a><a name="p1197221102113"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row13931721182113"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1698102142116"><a name="p1698102142116"></a><a name="p1698102142116"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p79916218211"><a name="p79916218211"></a><a name="p79916218211"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p16100152120214"><a name="p16100152120214"></a><a name="p16100152120214"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row09332118212"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p710162162113"><a name="p710162162113"></a><a name="p710162162113"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p71018213218"><a name="p71018213218"></a><a name="p71018213218"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p14103162162111"><a name="p14103162162111"></a><a name="p14103162162111"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row79352117216"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p201042216217"><a name="p201042216217"></a><a name="p201042216217"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p81041221142112"><a name="p81041221142112"></a><a name="p81041221142112"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1910642162116"><a name="p1910642162116"></a><a name="p1910642162116"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 403**

**表 7**  响应Body参数

<a name="table18107102119217"></a>
<table><thead align="left"><tr id="row1210792120214"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p410942115219"><a name="p410942115219"></a><a name="p410942115219"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p10110152132113"><a name="p10110152132113"></a><a name="p10110152132113"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p511102162112"><a name="p511102162112"></a><a name="p511102162112"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row19108102118212"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p10112182110212"><a name="p10112182110212"></a><a name="p10112182110212"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p18113321122117"><a name="p18113321122117"></a><a name="p18113321122117"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p5113112112214"><a name="p5113112112214"></a><a name="p5113112112214"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row1710810219214"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1111415214219"><a name="p1111415214219"></a><a name="p1111415214219"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1115192182117"><a name="p1115192182117"></a><a name="p1115192182117"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p13116122132119"><a name="p13116122132119"></a><a name="p13116122132119"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row17108221172120"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p12117121142114"><a name="p12117121142114"></a><a name="p12117121142114"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1111832117211"><a name="p1111832117211"></a><a name="p1111832117211"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p3119102112117"><a name="p3119102112117"></a><a name="p3119102112117"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 404**

**表 8**  响应Body参数

<a name="table1112122114216"></a>
<table><thead align="left"><tr id="row41211421162110"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p14123421182116"><a name="p14123421182116"></a><a name="p14123421182116"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p6124132182114"><a name="p6124132182114"></a><a name="p6124132182114"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p71260210213"><a name="p71260210213"></a><a name="p71260210213"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row9121721142110"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p11127172111216"><a name="p11127172111216"></a><a name="p11127172111216"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p19128202162113"><a name="p19128202162113"></a><a name="p19128202162113"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p16129182192113"><a name="p16129182192113"></a><a name="p16129182192113"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row101211221132111"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p813102116217"><a name="p813102116217"></a><a name="p813102116217"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p313272182110"><a name="p313272182110"></a><a name="p313272182110"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p91341121132110"><a name="p91341121132110"></a><a name="p91341121132110"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row17121821102113"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p191351821122116"><a name="p191351821122116"></a><a name="p191351821122116"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1313632116215"><a name="p1313632116215"></a><a name="p1313632116215"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p15137921162119"><a name="p15137921162119"></a><a name="p15137921162119"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 500**

**表 9**  响应Body参数

<a name="table1713962114216"></a>
<table><thead align="left"><tr id="row1140821122119"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p171421821112111"><a name="p171421821112111"></a><a name="p171421821112111"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p1514342172117"><a name="p1514342172117"></a><a name="p1514342172117"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p314415211217"><a name="p314415211217"></a><a name="p314415211217"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row714052119219"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p111451821122111"><a name="p111451821122111"></a><a name="p111451821122111"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p171465215211"><a name="p171465215211"></a><a name="p171465215211"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p9147192117213"><a name="p9147192117213"></a><a name="p9147192117213"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row014092120217"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p71488210214"><a name="p71488210214"></a><a name="p71488210214"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p114910210216"><a name="p114910210216"></a><a name="p114910210216"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1715062117214"><a name="p1715062117214"></a><a name="p1715062117214"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row111406214216"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p121518213215"><a name="p121518213215"></a><a name="p121518213215"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p71521421132119"><a name="p71521421132119"></a><a name="p71521421132119"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p915312214216"><a name="p915312214216"></a><a name="p915312214216"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

## 请求示例<a name="section111541921112118"></a>

```
GET https://{SMN_Endpoint}/v2

null
```

## 响应示例<a name="section121581521162114"></a>

**状态码： 200**

OK

```
{
  "version" : {
    "id" : "v2",
    "links" : [ {
      "href" : "https://127.0.0.1/v2",
      "rel" : "self"
    } ],
    "min_version" : "",
    "status" : "CURRENT",
    "updated" : "2018-09-19T00:00:00Z",
    "version" : ""
  }
}
```

## 状态码<a name="section111731521162118"></a>

<a name="status_code"></a>
<table><thead align="left"><tr id="row617417219212"><th class="cellrowborder" valign="top" width="15%" id="mcps1.1.3.1.1"><p id="p1417519211210"><a name="p1417519211210"></a><a name="p1417519211210"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="85%" id="mcps1.1.3.1.2"><p id="p1717712110219"><a name="p1717712110219"></a><a name="p1717712110219"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row10174152114211"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p71781921132116"><a name="p71781921132116"></a><a name="p71781921132116"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p4179152113213"><a name="p4179152113213"></a><a name="p4179152113213"></a>OK</p>
</td>
</tr>
<tr id="row617411211215"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p1018019217210"><a name="p1018019217210"></a><a name="p1018019217210"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p518111214218"><a name="p518111214218"></a><a name="p518111214218"></a>Bad Request</p>
</td>
</tr>
<tr id="row1117418216217"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p1181132182116"><a name="p1181132182116"></a><a name="p1181132182116"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p11182132110219"><a name="p11182132110219"></a><a name="p11182132110219"></a>Unauthorized</p>
</td>
</tr>
<tr id="row191746216215"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p101838215211"><a name="p101838215211"></a><a name="p101838215211"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p191841721132112"><a name="p191841721132112"></a><a name="p191841721132112"></a>Not Found</p>
</td>
</tr>
<tr id="row18174162132112"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p191856218212"><a name="p191856218212"></a><a name="p191856218212"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p1018732112215"><a name="p1018732112215"></a><a name="p1018732112215"></a>Internal Server Error</p>
</td>
</tr>
</tbody>
</table>

## 错误码<a name="section7188172112114"></a>

请参见[错误码](错误码.md)。

