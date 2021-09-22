# 查询Application的Endpoint列表<a name="ListApplicationEndpoints"></a>

## 功能介绍<a name="section475416662114"></a>

查询平台的endpoint列表。

## 调试<a name="section1056114122524"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=SMN&api=ListTopics)中调试该接口。

## URI<a name="section57564611213"></a>

GET /v2/\{project\_id\}/notifications/applications/\{application\_urn\}/endpoints

**表 1**  路径参数

<a name="table13758146182119"></a>
<table><thead align="left"><tr id="row147572060212"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p1175813652116"><a name="p1175813652116"></a><a name="p1175813652116"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p3758166214"><a name="p3758166214"></a><a name="p3758166214"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p97587612211"><a name="p97587612211"></a><a name="p97587612211"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p137598692119"><a name="p137598692119"></a><a name="p137598692119"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1075711622116"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p475976152119"><a name="p475976152119"></a><a name="p475976152119"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p775912612113"><a name="p775912612113"></a><a name="p775912612113"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1776086132118"><a name="p1776086132118"></a><a name="p1776086132118"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p17605612211"><a name="p17605612211"></a><a name="p17605612211"></a>项目ID。</p>
<p id="p4568812165217"><a name="p4568812165217"></a><a name="p4568812165217"></a>获取项目ID请参考<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
<tr id="row07571261214"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p197601265217"><a name="p197601265217"></a><a name="p197601265217"></a>application_urn</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p67612682110"><a name="p67612682110"></a><a name="p67612682110"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p147614615216"><a name="p147614615216"></a><a name="p147614615216"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1076176122119"><a name="p1076176122119"></a><a name="p1076176122119"></a>Application的唯一资源标识，可通过<a href="查询Application.md">查询Application</a>获取该标识。</p>
</td>
</tr>
</tbody>
</table>

**表 2**  Query参数

<a name="table2076312617218"></a>
<table><thead align="left"><tr id="row117621464218"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p976396142116"><a name="p976396142116"></a><a name="p976396142116"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p57630619213"><a name="p57630619213"></a><a name="p57630619213"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p9764463211"><a name="p9764463211"></a><a name="p9764463211"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p57647612216"><a name="p57647612216"></a><a name="p57647612216"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row27629611218"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p07641262212"><a name="p07641262212"></a><a name="p07641262212"></a>offset</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p5765186132113"><a name="p5765186132113"></a><a name="p5765186132113"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p15765666211"><a name="p15765666211"></a><a name="p15765666211"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1076506172115"><a name="p1076506172115"></a><a name="p1076506172115"></a>偏移量。</p>
<p id="p97668612113"><a name="p97668612113"></a><a name="p97668612113"></a>偏移量为一个大于0小于资源总个数的整数，表示查询该偏移量后面的所有的资源，默认值为0。</p>
<p id="p1276617614214"><a name="p1276617614214"></a><a name="p1276617614214"></a>缺省值：<strong id="b376696172115"><a name="b376696172115"></a><a name="b376696172115"></a>0</strong></p>
</td>
</tr>
<tr id="row12762862212"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p127669612219"><a name="p127669612219"></a><a name="p127669612219"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p976617612117"><a name="p976617612117"></a><a name="p976617612117"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p576714692114"><a name="p576714692114"></a><a name="p576714692114"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p176717672120"><a name="p176717672120"></a><a name="p176717672120"></a>查询的数量限制。</p>
<p id="p876717642116"><a name="p876717642116"></a><a name="p876717642116"></a>取值范围：1~100，取值一般为10，20，50。功能说明：每页返回的资源个数。默认值为100。</p>
<p id="p207671861218"><a name="p207671861218"></a><a name="p207671861218"></a>缺省值：<strong id="b1976820616218"><a name="b1976820616218"></a><a name="b1976820616218"></a>100</strong></p>
</td>
</tr>
<tr id="row9762196102120"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1876836172119"><a name="p1876836172119"></a><a name="p1876836172119"></a>enabled</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p4768196142110"><a name="p4768196142110"></a><a name="p4768196142110"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p197681966219"><a name="p197681966219"></a><a name="p197681966219"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p127692662111"><a name="p127692662111"></a><a name="p127692662111"></a>设备是否可用，值为true或false字符串。</p>
</td>
</tr>
<tr id="row5762116182115"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p776918612210"><a name="p776918612210"></a><a name="p776918612210"></a>token</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p2769561214"><a name="p2769561214"></a><a name="p2769561214"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p147701164219"><a name="p147701164219"></a><a name="p147701164219"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p157705652116"><a name="p157705652116"></a><a name="p157705652116"></a>设备token，最大长度512个字节。</p>
</td>
</tr>
<tr id="row5762196122116"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p17770136192110"><a name="p17770136192110"></a><a name="p17770136192110"></a>user_data</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p15770106172115"><a name="p15770106172115"></a><a name="p15770106172115"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p18771362219"><a name="p18771362219"></a><a name="p18771362219"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p67718615218"><a name="p67718615218"></a><a name="p67718615218"></a>用户数据，最大长度2048个字节。</p>
</td>
</tr>
</tbody>
</table>

## 请求参数<a name="section8771136152112"></a>

**表 3**  请求Header参数

<a name="HeaderParameter"></a>
<table><thead align="left"><tr id="row4772176202120"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p877396122118"><a name="p877396122118"></a><a name="p877396122118"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p1977316672114"><a name="p1977316672114"></a><a name="p1977316672114"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p4774186132111"><a name="p4774186132111"></a><a name="p4774186132111"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p67749618217"><a name="p67749618217"></a><a name="p67749618217"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row117723618218"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p37747692116"><a name="p37747692116"></a><a name="p37747692116"></a>X-Auth-Token</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1977411613211"><a name="p1977411613211"></a><a name="p1977411613211"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p127756619214"><a name="p127756619214"></a><a name="p127756619214"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p15775126132115"><a name="p15775126132115"></a><a name="p15775126132115"></a>用户Token。</p>
<p id="p87751769213"><a name="p87751769213"></a><a name="p87751769213"></a>通过调用IAM服务获取用户Token接口获取（响应消息头中X-Subject-Token的值）。</p>
</td>
</tr>
</tbody>
</table>

## 响应参数<a name="section777514618213"></a>

**状态码： 200**

**表 4**  响应Body参数

<a name="responseParameter"></a>
<table><thead align="left"><tr id="row2776661216"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p1677719642120"><a name="p1677719642120"></a><a name="p1677719642120"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p477717619214"><a name="p477717619214"></a><a name="p477717619214"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p77771067210"><a name="p77771067210"></a><a name="p77771067210"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row2776160219"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p97771264219"><a name="p97771264219"></a><a name="p97771264219"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1277811672117"><a name="p1277811672117"></a><a name="p1277811672117"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p167781563214"><a name="p167781563214"></a><a name="p167781563214"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row97764613211"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1877815610217"><a name="p1877815610217"></a><a name="p1877815610217"></a>next_page_flag</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p477812613213"><a name="p477812613213"></a><a name="p477812613213"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p117791060211"><a name="p117791060211"></a><a name="p117791060211"></a>是否有下一页标识。</p>
</td>
</tr>
<tr id="row11776261216"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p577910610216"><a name="p577910610216"></a><a name="p577910610216"></a>endpoints</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1577912612213"><a name="p1577912612213"></a><a name="p1577912612213"></a>Array of <a href="#response_ApplicationEndpoint">ApplicationEndpoint</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p677920642115"><a name="p677920642115"></a><a name="p677920642115"></a>Application_endpoint结构体数。</p>
</td>
</tr>
</tbody>
</table>

**表 5**  ApplicationEndpoint

<a name="response_ApplicationEndpoint"></a>
<table><thead align="left"><tr id="row2780667213"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p1478112652113"><a name="p1478112652113"></a><a name="p1478112652113"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p11781206102114"><a name="p11781206102114"></a><a name="p11781206102114"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p1578215642112"><a name="p1578215642112"></a><a name="p1578215642112"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row197805616216"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1078226122115"><a name="p1078226122115"></a><a name="p1078226122115"></a>create_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p17782146142120"><a name="p17782146142120"></a><a name="p17782146142120"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p12782261217"><a name="p12782261217"></a><a name="p12782261217"></a>创建application的时间。时间格式为UTC时间，YYYY-MM-DDTHH:MM:SSZ。</p>
</td>
</tr>
<tr id="row0780176172118"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p19783126152116"><a name="p19783126152116"></a><a name="p19783126152116"></a>endpoint_urn</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1578316615213"><a name="p1578316615213"></a><a name="p1578316615213"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p12783136132114"><a name="p12783136132114"></a><a name="p12783136132114"></a>Application endpoint的唯一资源标识。</p>
</td>
</tr>
<tr id="row578026112119"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1784766218"><a name="p1784766218"></a><a name="p1784766218"></a>user_data</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p57841615211"><a name="p57841615211"></a><a name="p57841615211"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p117844682117"><a name="p117844682117"></a><a name="p117844682117"></a>用户自定义数据。最大长度支持UTF-8编码后2048字节。</p>
</td>
</tr>
<tr id="row678010632116"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p87859602111"><a name="p87859602111"></a><a name="p87859602111"></a>enabled</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p107851669213"><a name="p107851669213"></a><a name="p107851669213"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p978619682118"><a name="p978619682118"></a><a name="p978619682118"></a>endpoint启用开关。true或false字符串。</p>
</td>
</tr>
<tr id="row1780366213"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p578611614211"><a name="p578611614211"></a><a name="p578611614211"></a>token</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p177861565219"><a name="p177861565219"></a><a name="p177861565219"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p2078776142119"><a name="p2078776142119"></a><a name="p2078776142119"></a>设备token。最大长度512个字节。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 400**

**表 6**  响应Body参数

<a name="table197879672112"></a>
<table><thead align="left"><tr id="row1078813612119"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p17891864213"><a name="p17891864213"></a><a name="p17891864213"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p1679015618215"><a name="p1679015618215"></a><a name="p1679015618215"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p579096102112"><a name="p579096102112"></a><a name="p579096102112"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row167880611217"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p879011622110"><a name="p879011622110"></a><a name="p879011622110"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p47911063218"><a name="p47911063218"></a><a name="p47911063218"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p079114610217"><a name="p079114610217"></a><a name="p079114610217"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row16788666212"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p379246102115"><a name="p379246102115"></a><a name="p379246102115"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p3792176192116"><a name="p3792176192116"></a><a name="p3792176192116"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1779326102118"><a name="p1779326102118"></a><a name="p1779326102118"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row9788146112110"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p177931365216"><a name="p177931365216"></a><a name="p177931365216"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p879313622120"><a name="p879313622120"></a><a name="p879313622120"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p6793663218"><a name="p6793663218"></a><a name="p6793663218"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 403**

**表 7**  响应Body参数

<a name="table87941642117"></a>
<table><thead align="left"><tr id="row117945632116"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p6796116152113"><a name="p6796116152113"></a><a name="p6796116152113"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p1179646122115"><a name="p1179646122115"></a><a name="p1179646122115"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p14796466219"><a name="p14796466219"></a><a name="p14796466219"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row47943620215"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p15797061213"><a name="p15797061213"></a><a name="p15797061213"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p20797567214"><a name="p20797567214"></a><a name="p20797567214"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p117979618215"><a name="p117979618215"></a><a name="p117979618215"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row1179520682112"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p57984611219"><a name="p57984611219"></a><a name="p57984611219"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p67985619218"><a name="p67985619218"></a><a name="p67985619218"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p179811615215"><a name="p179811615215"></a><a name="p179811615215"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row1179514682116"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p147992682112"><a name="p147992682112"></a><a name="p147992682112"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p207996611214"><a name="p207996611214"></a><a name="p207996611214"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p198001612116"><a name="p198001612116"></a><a name="p198001612116"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 404**

**表 8**  响应Body参数

<a name="table128001368215"></a>
<table><thead align="left"><tr id="row1680266132113"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p1180466102112"><a name="p1180466102112"></a><a name="p1180466102112"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p13804156132118"><a name="p13804156132118"></a><a name="p13804156132118"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p8804263217"><a name="p8804263217"></a><a name="p8804263217"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row12802176102114"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p188051865218"><a name="p188051865218"></a><a name="p188051865218"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p12806146172115"><a name="p12806146172115"></a><a name="p12806146172115"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p88062652110"><a name="p88062652110"></a><a name="p88062652110"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row1380218612111"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p3806116122119"><a name="p3806116122119"></a><a name="p3806116122119"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p11807067218"><a name="p11807067218"></a><a name="p11807067218"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p980719613215"><a name="p980719613215"></a><a name="p980719613215"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row1280212611215"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p11807116162111"><a name="p11807116162111"></a><a name="p11807116162111"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p178081261217"><a name="p178081261217"></a><a name="p178081261217"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p8808862218"><a name="p8808862218"></a><a name="p8808862218"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 500**

**表 9**  响应Body参数

<a name="table15808665218"></a>
<table><thead align="left"><tr id="row1809136122118"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p13810106112119"><a name="p13810106112119"></a><a name="p13810106112119"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p1681010616218"><a name="p1681010616218"></a><a name="p1681010616218"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p38109617214"><a name="p38109617214"></a><a name="p38109617214"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row168094616216"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p15811186162111"><a name="p15811186162111"></a><a name="p15811186162111"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p20811196202113"><a name="p20811196202113"></a><a name="p20811196202113"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1981176142116"><a name="p1981176142116"></a><a name="p1981176142116"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row7809136142117"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p118125632117"><a name="p118125632117"></a><a name="p118125632117"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p15812176122112"><a name="p15812176122112"></a><a name="p15812176122112"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1881246132114"><a name="p1881246132114"></a><a name="p1881246132114"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row1680917617212"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1881214682118"><a name="p1881214682118"></a><a name="p1881214682118"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p981317632111"><a name="p981317632111"></a><a name="p981317632111"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1881316617218"><a name="p1881316617218"></a><a name="p1881316617218"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

## 请求示例<a name="section1981366102115"></a>

```
GET https://{SMN_Endpoint}/v2/{project_id}/notifications/applications/{application_urn}/endpoints?offset=0&limit=10

null
```

## 响应示例<a name="section12814156202114"></a>

**状态码： 200**

OK

```
{
  "request_id" : "c90d871f77f7425cae0a8b772a563d17",
  "next_page_flag" : false,
  "endpoints" : [ {
    "create_time" : "2018-01-12T01:25:14Z",
    "endpoint_urn" : "urn:smn:regionId:429ffced18074da0938112f2c362b935:endpoint-APNS-application_name-62f0bafec61c45fbbb5d0fc6bd696a2d",
    "user_data" : "no user data",
    "enabled" : "true",
    "token" : "1f2fda4c1013c47ac4c59bd22379d88e14b07b0ebf47f2f79d1a6b06ed03390d"
  } ]
}
```

## 状态码<a name="section208176642111"></a>

<a name="status_code"></a>
<table><thead align="left"><tr id="row198181632113"><th class="cellrowborder" valign="top" width="15%" id="mcps1.1.3.1.1"><p id="p78195614217"><a name="p78195614217"></a><a name="p78195614217"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="85%" id="mcps1.1.3.1.2"><p id="p10819760217"><a name="p10819760217"></a><a name="p10819760217"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row48188642110"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p182011682110"><a name="p182011682110"></a><a name="p182011682110"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p158208610217"><a name="p158208610217"></a><a name="p158208610217"></a>OK</p>
</td>
</tr>
<tr id="row981866162117"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p168207602110"><a name="p168207602110"></a><a name="p168207602110"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p1782186132114"><a name="p1782186132114"></a><a name="p1782186132114"></a>Bad Request</p>
</td>
</tr>
<tr id="row1481819617218"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p148218617215"><a name="p148218617215"></a><a name="p148218617215"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p5821126172115"><a name="p5821126172115"></a><a name="p5821126172115"></a>Unauthorized</p>
</td>
</tr>
<tr id="row78181682118"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p78222618213"><a name="p78222618213"></a><a name="p78222618213"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p1682212613216"><a name="p1682212613216"></a><a name="p1682212613216"></a>Not Found</p>
</td>
</tr>
<tr id="row3818463211"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p28221160211"><a name="p28221160211"></a><a name="p28221160211"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p58226613217"><a name="p58226613217"></a><a name="p58226613217"></a>Internal Server Error</p>
</td>
</tr>
</tbody>
</table>

## 错误码<a name="section128221664211"></a>

请参见[错误码](错误码.md)。

