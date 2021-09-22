# 查询SMN支持的API版本号信息<a name="ListVersions"></a>

## 功能介绍<a name="section2756132012115"></a>

查询SMN开放API支持的版本号。

## 调试<a name="section1056114122524"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=SMN&api=ListTopics)中调试该接口。

## URI<a name="section476017207218"></a>

GET /

## 请求参数<a name="section1762122052119"></a>

**表 1**  请求Header参数

<a name="HeaderParameter"></a>
<table><thead align="left"><tr id="row16763162042113"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p18765420102115"><a name="p18765420102115"></a><a name="p18765420102115"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p276632082117"><a name="p276632082117"></a><a name="p276632082117"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p1076772013217"><a name="p1076772013217"></a><a name="p1076772013217"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p127687204219"><a name="p127687204219"></a><a name="p127687204219"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row14763120122118"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p15768172042110"><a name="p15768172042110"></a><a name="p15768172042110"></a>X-Auth-Token</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1876911209216"><a name="p1876911209216"></a><a name="p1876911209216"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p6770620162119"><a name="p6770620162119"></a><a name="p6770620162119"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p197711220172115"><a name="p197711220172115"></a><a name="p197711220172115"></a>用户Token。</p>
<p id="p137721720162110"><a name="p137721720162110"></a><a name="p137721720162110"></a>通过调用IAM服务获取用户Token接口获取（响应消息头中X-Subject-Token的值）。</p>
</td>
</tr>
</tbody>
</table>

## 响应参数<a name="section3774720132114"></a>

**状态码： 200**

**表 2**  响应Body参数

<a name="responseParameter"></a>
<table><thead align="left"><tr id="row19776820152117"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p177862052119"><a name="p177862052119"></a><a name="p177862052119"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p1777902032118"><a name="p1777902032118"></a><a name="p1777902032118"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p2780520172119"><a name="p2780520172119"></a><a name="p2780520172119"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1877662013210"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p078119201216"><a name="p078119201216"></a><a name="p078119201216"></a>versions</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p9782152014213"><a name="p9782152014213"></a><a name="p9782152014213"></a>Array of <a href="#response_VersionItem">VersionItem</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1078312209217"><a name="p1078312209217"></a><a name="p1078312209217"></a>描述version相关对象的列表。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  VersionItem

<a name="response_VersionItem"></a>
<table><thead align="left"><tr id="row1078414202212"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p478662082119"><a name="p478662082119"></a><a name="p478662082119"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p57874206210"><a name="p57874206210"></a><a name="p57874206210"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p2788102019213"><a name="p2788102019213"></a><a name="p2788102019213"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row19784162020212"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p578972011213"><a name="p578972011213"></a><a name="p578972011213"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p13790820142119"><a name="p13790820142119"></a><a name="p13790820142119"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p16791172019211"><a name="p16791172019211"></a><a name="p16791172019211"></a>版本ID（版本号），如v2。</p>
</td>
</tr>
<tr id="row57849202218"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p679262062117"><a name="p679262062117"></a><a name="p679262062117"></a>min_version</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p57931920142112"><a name="p57931920142112"></a><a name="p57931920142112"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1979417205217"><a name="p1979417205217"></a><a name="p1979417205217"></a>若该版本API支持微版本，则返回支持的最小微版本号；若不支持微版本，则返回空。</p>
</td>
</tr>
<tr id="row678482013215"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p47946204213"><a name="p47946204213"></a><a name="p47946204213"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1795920122110"><a name="p1795920122110"></a><a name="p1795920122110"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p12797162012117"><a name="p12797162012117"></a><a name="p12797162012117"></a>版本状态，为如下3种：</p>
<p id="p19798102062118"><a name="p19798102062118"></a><a name="p19798102062118"></a>CURRENT：表示该版本为主推版本。</p>
<p id="p1579882062117"><a name="p1579882062117"></a><a name="p1579882062117"></a>SUPPORTED：表示为老版本，但是现在还继续支持。</p>
<p id="p15799920152115"><a name="p15799920152115"></a><a name="p15799920152115"></a>DEPRECATED：表示为废弃版本，存在后续删除的可能。</p>
</td>
</tr>
<tr id="row127844203214"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1580052012112"><a name="p1580052012112"></a><a name="p1580052012112"></a>updated</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p198011207213"><a name="p198011207213"></a><a name="p198011207213"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p15802112013217"><a name="p15802112013217"></a><a name="p15802112013217"></a>版本发布时间，要求用UTC时间格式表示。如v2发布的时间2014-06-28T12:20:21Z。</p>
</td>
</tr>
<tr id="row1978432014213"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p108031205217"><a name="p108031205217"></a><a name="p108031205217"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1580411201219"><a name="p1580411201219"></a><a name="p1580411201219"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1680542018217"><a name="p1680542018217"></a><a name="p1680542018217"></a>若该版本API支持微版本，则返回支持的最大微版本号；若不支持微版本，则返回空。</p>
</td>
</tr>
<tr id="row1878462011218"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p9807202042116"><a name="p9807202042116"></a><a name="p9807202042116"></a>links</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p58083206216"><a name="p58083206216"></a><a name="p58083206216"></a>Array of <a href="#response_LinksItem">LinksItem</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1680918208219"><a name="p1680918208219"></a><a name="p1680918208219"></a>API的URL地址。</p>
</td>
</tr>
</tbody>
</table>

**表 4**  LinksItem

<a name="response_LinksItem"></a>
<table><thead align="left"><tr id="row88101920162117"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p1812102052112"><a name="p1812102052112"></a><a name="p1812102052112"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p1781402018218"><a name="p1781402018218"></a><a name="p1781402018218"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p1814220172120"><a name="p1814220172120"></a><a name="p1814220172120"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row281112042119"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p17815120122117"><a name="p17815120122117"></a><a name="p17815120122117"></a>href</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p38171120182118"><a name="p38171120182118"></a><a name="p38171120182118"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p681811202215"><a name="p681811202215"></a><a name="p681811202215"></a>对应快捷链接。</p>
</td>
</tr>
<tr id="row17811172013215"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1281992062110"><a name="p1281992062110"></a><a name="p1281992062110"></a>rel</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p68201420122111"><a name="p68201420122111"></a><a name="p68201420122111"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p108211220162114"><a name="p108211220162114"></a><a name="p108211220162114"></a>快捷链接标记名称。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 400**

**表 5**  响应Body参数

<a name="table1822122022112"></a>
<table><thead align="left"><tr id="row5823120192117"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p782412042112"><a name="p782412042112"></a><a name="p782412042112"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p282632092117"><a name="p282632092117"></a><a name="p282632092117"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p1782710205216"><a name="p1782710205216"></a><a name="p1782710205216"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row16823120182116"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p88282020112114"><a name="p88282020112114"></a><a name="p88282020112114"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p2082952032110"><a name="p2082952032110"></a><a name="p2082952032110"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1283011205215"><a name="p1283011205215"></a><a name="p1283011205215"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row782316207216"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1183102012114"><a name="p1183102012114"></a><a name="p1183102012114"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p14831112062120"><a name="p14831112062120"></a><a name="p14831112062120"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p883252062114"><a name="p883252062114"></a><a name="p883252062114"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row148235200211"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1483382019212"><a name="p1483382019212"></a><a name="p1483382019212"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p883432011215"><a name="p883432011215"></a><a name="p883432011215"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p11835122010219"><a name="p11835122010219"></a><a name="p11835122010219"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 403**

**表 6**  响应Body参数

<a name="table4837102062114"></a>
<table><thead align="left"><tr id="row138371820202110"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p1839122017211"><a name="p1839122017211"></a><a name="p1839122017211"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p11840122072113"><a name="p11840122072113"></a><a name="p11840122072113"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p4841112015214"><a name="p4841112015214"></a><a name="p4841112015214"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row5837120202110"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p88421820192117"><a name="p88421820192117"></a><a name="p88421820192117"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p12843182072120"><a name="p12843182072120"></a><a name="p12843182072120"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1584402062111"><a name="p1584402062111"></a><a name="p1584402062111"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row1837192012112"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p684415204219"><a name="p684415204219"></a><a name="p684415204219"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1384502032117"><a name="p1384502032117"></a><a name="p1384502032117"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p484682092117"><a name="p484682092117"></a><a name="p484682092117"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row4837220112118"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p12847132082119"><a name="p12847132082119"></a><a name="p12847132082119"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1784882042110"><a name="p1784882042110"></a><a name="p1784882042110"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p2849202042114"><a name="p2849202042114"></a><a name="p2849202042114"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 404**

**表 7**  响应Body参数

<a name="table585113202216"></a>
<table><thead align="left"><tr id="row4851122092113"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p1085392042117"><a name="p1085392042117"></a><a name="p1085392042117"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p9855182052110"><a name="p9855182052110"></a><a name="p9855182052110"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p2856142017219"><a name="p2856142017219"></a><a name="p2856142017219"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row20851192012211"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p12857142018218"><a name="p12857142018218"></a><a name="p12857142018218"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p108588202213"><a name="p108588202213"></a><a name="p108588202213"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p5859132082119"><a name="p5859132082119"></a><a name="p5859132082119"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row15851172002113"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1086014205218"><a name="p1086014205218"></a><a name="p1086014205218"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p98613202217"><a name="p98613202217"></a><a name="p98613202217"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p586222072113"><a name="p586222072113"></a><a name="p586222072113"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row128525206210"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p19863420112113"><a name="p19863420112113"></a><a name="p19863420112113"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p286413208218"><a name="p286413208218"></a><a name="p286413208218"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p886510204217"><a name="p886510204217"></a><a name="p886510204217"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 500**

**表 8**  响应Body参数

<a name="table108661620132119"></a>
<table><thead align="left"><tr id="row1786710204215"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p168691120182119"><a name="p168691120182119"></a><a name="p168691120182119"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p11870122052116"><a name="p11870122052116"></a><a name="p11870122052116"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p6871620182119"><a name="p6871620182119"></a><a name="p6871620182119"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1186772016214"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p118721920162120"><a name="p118721920162120"></a><a name="p118721920162120"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p087317203213"><a name="p087317203213"></a><a name="p087317203213"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p087417200212"><a name="p087417200212"></a><a name="p087417200212"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row1986722012219"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p148751220162112"><a name="p148751220162112"></a><a name="p148751220162112"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1887611208214"><a name="p1887611208214"></a><a name="p1887611208214"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p4877720172118"><a name="p4877720172118"></a><a name="p4877720172118"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row168671520152118"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1187872092116"><a name="p1187872092116"></a><a name="p1187872092116"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p12879102082110"><a name="p12879102082110"></a><a name="p12879102082110"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p188042019215"><a name="p188042019215"></a><a name="p188042019215"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

## 请求示例<a name="section1188116201210"></a>

```
GET https://{SMN_Endpoint}/

null
```

## 响应示例<a name="section16885192016211"></a>

**状态码： 200**

OK

```
{
  "versions" : {
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

## 状态码<a name="section2899820132114"></a>

<a name="status_code"></a>
<table><thead align="left"><tr id="row190192032119"><th class="cellrowborder" valign="top" width="15%" id="mcps1.1.3.1.1"><p id="p49021820112118"><a name="p49021820112118"></a><a name="p49021820112118"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="85%" id="mcps1.1.3.1.2"><p id="p690392018217"><a name="p690392018217"></a><a name="p690392018217"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row12901122032112"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p1905172011214"><a name="p1905172011214"></a><a name="p1905172011214"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p59061020162110"><a name="p59061020162110"></a><a name="p59061020162110"></a>OK</p>
</td>
</tr>
<tr id="row119011204212"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p14907172019214"><a name="p14907172019214"></a><a name="p14907172019214"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p179082203213"><a name="p179082203213"></a><a name="p179082203213"></a>Bad Request</p>
</td>
</tr>
<tr id="row1901620162118"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p29091920112117"><a name="p29091920112117"></a><a name="p29091920112117"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p1091015209219"><a name="p1091015209219"></a><a name="p1091015209219"></a>Unauthorized</p>
</td>
</tr>
<tr id="row4901102062117"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p4911122042110"><a name="p4911122042110"></a><a name="p4911122042110"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p1291332017219"><a name="p1291332017219"></a><a name="p1291332017219"></a>Not Found</p>
</td>
</tr>
<tr id="row13901142020212"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p89141420162111"><a name="p89141420162111"></a><a name="p89141420162111"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p591511208212"><a name="p591511208212"></a><a name="p591511208212"></a>Internal Server Error</p>
</td>
</tr>
</tbody>
</table>

## 错误码<a name="section091782010214"></a>

请参见[错误码](错误码.md)。

