# 查询Application<a name="ListApplications"></a>

## 功能介绍<a name="section03714560200"></a>

查询应用平台列表。

## 调试<a name="section1056114122524"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=SMN&api=ListTopics)中调试该接口。

## URI<a name="section839115612010"></a>

GET /v2/\{project\_id\}/notifications/applications

**表 1**  路径参数

<a name="table8421856112012"></a>
<table><thead align="left"><tr id="row204175622010"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p1042145616205"><a name="p1042145616205"></a><a name="p1042145616205"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p1543125617201"><a name="p1543125617201"></a><a name="p1543125617201"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p164413560209"><a name="p164413560209"></a><a name="p164413560209"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p94535672013"><a name="p94535672013"></a><a name="p94535672013"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row841135614205"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p64535682019"><a name="p64535682019"></a><a name="p64535682019"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p144645622017"><a name="p144645622017"></a><a name="p144645622017"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1246256162017"><a name="p1246256162017"></a><a name="p1246256162017"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1347195620204"><a name="p1347195620204"></a><a name="p1347195620204"></a>项目ID。</p>
<p id="p4568812165217"><a name="p4568812165217"></a><a name="p4568812165217"></a>获取项目ID请参考<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 2**  Query参数

<a name="table550156102018"></a>
<table><thead align="left"><tr id="row184910568205"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p2051105692014"><a name="p2051105692014"></a><a name="p2051105692014"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p1552155632011"><a name="p1552155632011"></a><a name="p1552155632011"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p452135615209"><a name="p452135615209"></a><a name="p452135615209"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p65317562207"><a name="p65317562207"></a><a name="p65317562207"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row649756162017"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p5545567205"><a name="p5545567205"></a><a name="p5545567205"></a>offset</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p12553565205"><a name="p12553565205"></a><a name="p12553565205"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p13557562206"><a name="p13557562206"></a><a name="p13557562206"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p105625662016"><a name="p105625662016"></a><a name="p105625662016"></a>偏移量。</p>
<p id="p55615567201"><a name="p55615567201"></a><a name="p55615567201"></a>偏移量为一个大于0小于资源总个数的整数，表示查询该偏移量后面的所有的资源，默认值为0。</p>
<p id="p1057175612016"><a name="p1057175612016"></a><a name="p1057175612016"></a>缺省值：<strong id="b145725682011"><a name="b145725682011"></a><a name="b145725682011"></a>0</strong></p>
</td>
</tr>
<tr id="row24925612201"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p857145632019"><a name="p857145632019"></a><a name="p857145632019"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1858556132010"><a name="p1858556132010"></a><a name="p1858556132010"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p145985618203"><a name="p145985618203"></a><a name="p145985618203"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1459135602016"><a name="p1459135602016"></a><a name="p1459135602016"></a>查询的数量限制。</p>
<p id="p660175632013"><a name="p660175632013"></a><a name="p660175632013"></a>取值范围：1~100，取值一般为10，20，50。功能说明：每页返回的资源个数。默认值为100。</p>
<p id="p176011567207"><a name="p176011567207"></a><a name="p176011567207"></a>缺省值：<strong id="b560956132013"><a name="b560956132013"></a><a name="b560956132013"></a>100</strong></p>
</td>
</tr>
<tr id="row134985612011"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p136117565203"><a name="p136117565203"></a><a name="p136117565203"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1662205611204"><a name="p1662205611204"></a><a name="p1662205611204"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p96255662018"><a name="p96255662018"></a><a name="p96255662018"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p76385613200"><a name="p76385613200"></a><a name="p76385613200"></a>检索应用名称。</p>
<p id="p66325616203"><a name="p66325616203"></a><a name="p66325616203"></a>支持后向模糊匹配，长度不得超过64个字符，只能包含英文字母、下划线和数字。</p>
</td>
</tr>
<tr id="row249145616207"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1564956162016"><a name="p1564956162016"></a><a name="p1564956162016"></a>platform</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p106555619204"><a name="p106555619204"></a><a name="p106555619204"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p76514566205"><a name="p76514566205"></a><a name="p76514566205"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p96665682013"><a name="p96665682013"></a><a name="p96665682013"></a>应用平台。</p>
<p id="p11675563200"><a name="p11675563200"></a><a name="p11675563200"></a>目前仅支持HMS、APNS、APNS_SANDBOX。</p>
<p id="p196745611201"><a name="p196745611201"></a><a name="p196745611201"></a>HMS是为开发者提供的消息推送平台。</p>
<p id="p167856192011"><a name="p167856192011"></a><a name="p167856192011"></a>APNS和APNS_SANDBOX是用于推送iOS消息的服务平台。</p>
</td>
</tr>
</tbody>
</table>

## 请求参数<a name="section5681563208"></a>

**表 3**  请求Header参数

<a name="HeaderParameter"></a>
<table><thead align="left"><tr id="row19698567205"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p1270165672011"><a name="p1270165672011"></a><a name="p1270165672011"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p771656142011"><a name="p771656142011"></a><a name="p771656142011"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p20728568206"><a name="p20728568206"></a><a name="p20728568206"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p177314566204"><a name="p177314566204"></a><a name="p177314566204"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row66975610208"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p167475662014"><a name="p167475662014"></a><a name="p167475662014"></a>X-Auth-Token</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p3741156132016"><a name="p3741156132016"></a><a name="p3741156132016"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p117575612202"><a name="p117575612202"></a><a name="p117575612202"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p18766567201"><a name="p18766567201"></a><a name="p18766567201"></a>用户Token。</p>
<p id="p167795613204"><a name="p167795613204"></a><a name="p167795613204"></a>通过调用IAM服务获取用户Token接口获取（响应消息头中X-Subject-Token的值）。</p>
</td>
</tr>
</tbody>
</table>

## 响应参数<a name="section157805620202"></a>

**状态码： 200**

**表 4**  响应Body参数

<a name="responseParameter"></a>
<table><thead align="left"><tr id="row280185613206"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p6811256172014"><a name="p6811256172014"></a><a name="p6811256172014"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p16821756202016"><a name="p16821756202016"></a><a name="p16821756202016"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p682656172019"><a name="p682656172019"></a><a name="p682656172019"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row38095672017"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p583556172020"><a name="p583556172020"></a><a name="p583556172020"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1884256112016"><a name="p1884256112016"></a><a name="p1884256112016"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p28485616204"><a name="p28485616204"></a><a name="p28485616204"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row198017563207"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p485155619206"><a name="p485155619206"></a><a name="p485155619206"></a>application_count</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p16862567206"><a name="p16862567206"></a><a name="p16862567206"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p48611567204"><a name="p48611567204"></a><a name="p48611567204"></a>返回的Application个数。该参数不受offset和limit影响，即返回的是您帐户下所有的Application个数。</p>
</td>
</tr>
<tr id="row148010569204"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p68765614202"><a name="p68765614202"></a><a name="p68765614202"></a>applications</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p148875615206"><a name="p148875615206"></a><a name="p148875615206"></a>Array of <a href="#response_ApplicationItem">ApplicationItem</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p9881562207"><a name="p9881562207"></a><a name="p9881562207"></a>详见<a href="#response_ApplicationItem">表5</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 5**  ApplicationItem

<a name="response_ApplicationItem"></a>
<table><thead align="left"><tr id="row1490145642017"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p5922056162013"><a name="p5922056162013"></a><a name="p5922056162013"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p1892256182013"><a name="p1892256182013"></a><a name="p1892256182013"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p149365692018"><a name="p149365692018"></a><a name="p149365692018"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row139085614205"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p199414566204"><a name="p199414566204"></a><a name="p199414566204"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p29411566201"><a name="p29411566201"></a><a name="p29411566201"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1495155619208"><a name="p1495155619208"></a><a name="p1495155619208"></a>创建application的名字。</p>
</td>
</tr>
<tr id="row09045612019"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p19961566209"><a name="p19961566209"></a><a name="p19961566209"></a>platform</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p13971756172013"><a name="p13971756172013"></a><a name="p13971756172013"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p69712569205"><a name="p69712569205"></a><a name="p69712569205"></a>应用平台。</p>
</td>
</tr>
<tr id="row189085692015"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p2982056202015"><a name="p2982056202015"></a><a name="p2982056202015"></a>create_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1199115620205"><a name="p1199115620205"></a><a name="p1199115620205"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p14100556162015"><a name="p14100556162015"></a><a name="p14100556162015"></a>创建application的时间。时间格式为UTC时间，YYYY-MM-DDTHH:MM:SSZ。</p>
</td>
</tr>
<tr id="row10902567200"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p610114562208"><a name="p610114562208"></a><a name="p610114562208"></a>application_urn</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p12101195618206"><a name="p12101195618206"></a><a name="p12101195618206"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p3102155616207"><a name="p3102155616207"></a><a name="p3102155616207"></a>Application的唯一资源标识。</p>
</td>
</tr>
<tr id="row89015567207"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p131031456202010"><a name="p131031456202010"></a><a name="p131031456202010"></a>application_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1010445610203"><a name="p1010445610203"></a><a name="p1010445610203"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p151042056122015"><a name="p151042056122015"></a><a name="p151042056122015"></a>Application的唯一标识ID。</p>
</td>
</tr>
<tr id="row1390105614202"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p15105125652014"><a name="p15105125652014"></a><a name="p15105125652014"></a>enabled</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1610615617205"><a name="p1610615617205"></a><a name="p1610615617205"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p5106115613201"><a name="p5106115613201"></a><a name="p5106115613201"></a>应用平台是否启用。</p>
</td>
</tr>
<tr id="row12901356162015"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1610765682018"><a name="p1610765682018"></a><a name="p1610765682018"></a>apple_certificate_expiration_date</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p16108256132014"><a name="p16108256132014"></a><a name="p16108256132014"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p151086563200"><a name="p151086563200"></a><a name="p151086563200"></a>苹果证书过期时间APNS、APNS_SANDBOX平台特有属性时间格式为UTC时间，YYYY-MM-DDTHH:MM:SSZ。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 400**

**表 6**  响应Body参数

<a name="table161092563202"></a>
<table><thead align="left"><tr id="row81101156172017"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p15111145614206"><a name="p15111145614206"></a><a name="p15111145614206"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p711285616207"><a name="p711285616207"></a><a name="p711285616207"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p14113145613203"><a name="p14113145613203"></a><a name="p14113145613203"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row71101556102020"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1511610568209"><a name="p1511610568209"></a><a name="p1511610568209"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p111710568204"><a name="p111710568204"></a><a name="p111710568204"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p17117175612020"><a name="p17117175612020"></a><a name="p17117175612020"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row1211035622012"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p121181956142016"><a name="p121181956142016"></a><a name="p121181956142016"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1911925692014"><a name="p1911925692014"></a><a name="p1911925692014"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1512014560203"><a name="p1512014560203"></a><a name="p1512014560203"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row1110356102012"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p2121556142012"><a name="p2121556142012"></a><a name="p2121556142012"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p0121756122018"><a name="p0121756122018"></a><a name="p0121756122018"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p18122175612014"><a name="p18122175612014"></a><a name="p18122175612014"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 403**

**表 7**  响应Body参数

<a name="table17123135611206"></a>
<table><thead align="left"><tr id="row3124195652015"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p16125956202015"><a name="p16125956202015"></a><a name="p16125956202015"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p20126105632011"><a name="p20126105632011"></a><a name="p20126105632011"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p1612775662016"><a name="p1612775662016"></a><a name="p1612775662016"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row161241356112017"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p141272056182016"><a name="p141272056182016"></a><a name="p141272056182016"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p12128165620206"><a name="p12128165620206"></a><a name="p12128165620206"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p11292564205"><a name="p11292564205"></a><a name="p11292564205"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row5124556202011"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p61301556182013"><a name="p61301556182013"></a><a name="p61301556182013"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p113015567207"><a name="p113015567207"></a><a name="p113015567207"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p18131205682013"><a name="p18131205682013"></a><a name="p18131205682013"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row7124256102014"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p71326562205"><a name="p71326562205"></a><a name="p71326562205"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p181323569208"><a name="p181323569208"></a><a name="p181323569208"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p81333560207"><a name="p81333560207"></a><a name="p81333560207"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 404**

**表 8**  响应Body参数

<a name="table19134115682017"></a>
<table><thead align="left"><tr id="row7134115615205"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p7135175610203"><a name="p7135175610203"></a><a name="p7135175610203"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p51369569205"><a name="p51369569205"></a><a name="p51369569205"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p13137195612017"><a name="p13137195612017"></a><a name="p13137195612017"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row41341856202015"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p313811560208"><a name="p313811560208"></a><a name="p313811560208"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p513935610203"><a name="p513935610203"></a><a name="p513935610203"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1414065682010"><a name="p1414065682010"></a><a name="p1414065682010"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row1013495616207"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p614013561207"><a name="p614013561207"></a><a name="p614013561207"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p7141165682010"><a name="p7141165682010"></a><a name="p7141165682010"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p814235612207"><a name="p814235612207"></a><a name="p814235612207"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row2134175610200"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p114345652017"><a name="p114345652017"></a><a name="p114345652017"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p17143356152014"><a name="p17143356152014"></a><a name="p17143356152014"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1414415564202"><a name="p1414415564202"></a><a name="p1414415564202"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 500**

**表 9**  响应Body参数

<a name="table814535617202"></a>
<table><thead align="left"><tr id="row1114612561205"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p1114775615201"><a name="p1114775615201"></a><a name="p1114775615201"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p171481256112020"><a name="p171481256112020"></a><a name="p171481256112020"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p11491956132012"><a name="p11491956132012"></a><a name="p11491956132012"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1414613561205"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p161506565208"><a name="p161506565208"></a><a name="p161506565208"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p215015610203"><a name="p215015610203"></a><a name="p215015610203"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p12151105652017"><a name="p12151105652017"></a><a name="p12151105652017"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row6146195618206"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p515114568205"><a name="p515114568205"></a><a name="p515114568205"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p141521656162020"><a name="p141521656162020"></a><a name="p141521656162020"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p615310562201"><a name="p615310562201"></a><a name="p615310562201"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row2146125652014"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p9154115692019"><a name="p9154115692019"></a><a name="p9154115692019"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p10154205652010"><a name="p10154205652010"></a><a name="p10154205652010"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1815520565206"><a name="p1815520565206"></a><a name="p1815520565206"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

## 请求示例<a name="section15155165652010"></a>

```
GET https://{SMN_Endpoint}/v2/{project_id}/notifications/applications?offset=0&limit=100&name=application_name&platform=APNS

null
```

## 响应示例<a name="section7158256102014"></a>

**状态码： 200**

OK

```
{
  "request_id" : "6a63a18b8bab40ffb71ebd9cb80d0085",
  "application_count" : 2,
  "applications" : [ {
    "create_time" : "2018-02-08T08:30:16Z",
    "apple_certificate_expiration_date" : "2018-03-09T12:21:40Z",
    "name" : "application_name001",
    "platform" : "APNS",
    "enabled" : "true",
    "application_urn" : "urn:smn:regionId:429ffced18074da0938112f2c362b935:app-APNS-application_name001",
    "application_id" : "b1b8643dc12b4g77ad6e35a16003119b"
  }, {
    "create_time" : "2018-01-11T12:58:58Z",
    "apple_certificate_expiration_date" : "2018-03-09T12:21:40Z",
    "name" : "application_name002",
    "platform" : "APNS",
    "enabled" : "true",
    "application_urn" : "urn:smn:regionId:429ffced18074da0938112f2c362b935:app-APNS-application_name002",
    "application_id" : "a3a4643dc12b4g77ad6e35a16002558c"
  } ]
}
```

## 状态码<a name="section5170656162020"></a>

<a name="status_code"></a>
<table><thead align="left"><tr id="row51715569205"><th class="cellrowborder" valign="top" width="15%" id="mcps1.1.3.1.1"><p id="p317235652018"><a name="p317235652018"></a><a name="p317235652018"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="85%" id="mcps1.1.3.1.2"><p id="p317395632018"><a name="p317395632018"></a><a name="p317395632018"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row91711856142017"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p171731056192015"><a name="p171731056192015"></a><a name="p171731056192015"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p9174856152018"><a name="p9174856152018"></a><a name="p9174856152018"></a>OK</p>
</td>
</tr>
<tr id="row171711456102020"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p7175105613209"><a name="p7175105613209"></a><a name="p7175105613209"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p9175195682012"><a name="p9175195682012"></a><a name="p9175195682012"></a>Bad Request</p>
</td>
</tr>
<tr id="row121711356152013"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p13176155616204"><a name="p13176155616204"></a><a name="p13176155616204"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p6278056112018"><a name="p6278056112018"></a><a name="p6278056112018"></a>Unauthorized</p>
</td>
</tr>
<tr id="row51711656182019"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p4279105614203"><a name="p4279105614203"></a><a name="p4279105614203"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p16279156132014"><a name="p16279156132014"></a><a name="p16279156132014"></a>Not Found</p>
</td>
</tr>
<tr id="row191719562201"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p12799562203"><a name="p12799562203"></a><a name="p12799562203"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p1227995632020"><a name="p1227995632020"></a><a name="p1227995632020"></a>Internal Server Error</p>
</td>
</tr>
</tbody>
</table>

## 错误码<a name="section17280125692017"></a>

请参见[错误码](错误码.md)。

