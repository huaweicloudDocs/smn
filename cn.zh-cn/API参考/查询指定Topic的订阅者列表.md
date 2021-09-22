# 查询指定Topic的订阅者列表<a name="ListSubscriptionsByTopic"></a>

## 功能介绍<a name="section17149321192016"></a>

分页获取特定Topic的订阅列表，订阅列表按照订阅创建时间进行升序排列。分页查询可以指定offset以及limit。如果指定Topic不存在订阅者，返回空列表。

## 调试<a name="section1056114122524"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=SMN&api=ListTopics)中调试该接口。

## URI<a name="section21512210201"></a>

GET /v2/\{project\_id\}/notifications/topics/\{topic\_urn\}/subscriptions

**表 1**  路径参数

<a name="table191542214207"></a>
<table><thead align="left"><tr id="row1915312116207"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p14155172116200"><a name="p14155172116200"></a><a name="p14155172116200"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p61551921162012"><a name="p61551921162012"></a><a name="p61551921162012"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p16156192182014"><a name="p16156192182014"></a><a name="p16156192182014"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p7157321112010"><a name="p7157321112010"></a><a name="p7157321112010"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row415312213202"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1015714212207"><a name="p1015714212207"></a><a name="p1015714212207"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p18158521122010"><a name="p18158521122010"></a><a name="p18158521122010"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p515992182019"><a name="p515992182019"></a><a name="p515992182019"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1616082132012"><a name="p1616082132012"></a><a name="p1616082132012"></a>项目ID。</p>
<p id="p4568812165217"><a name="p4568812165217"></a><a name="p4568812165217"></a>获取项目ID请参考<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
<tr id="row11531121132016"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p19162421142010"><a name="p19162421142010"></a><a name="p19162421142010"></a>topic_urn</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1216219212201"><a name="p1216219212201"></a><a name="p1216219212201"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1216332118205"><a name="p1216332118205"></a><a name="p1216332118205"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p5768161217528"><a name="p5768161217528"></a><a name="p5768161217528"></a>Topic的唯一的资源标识，可通过<a href="查询主题列表.md">查询主题列表</a>获取该标识。</p>
</td>
</tr>
</tbody>
</table>

**表 2**  Query参数

<a name="table016632182017"></a>
<table><thead align="left"><tr id="row6165721162019"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p3167182142011"><a name="p3167182142011"></a><a name="p3167182142011"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p1016722120202"><a name="p1016722120202"></a><a name="p1016722120202"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p11681421162015"><a name="p11681421162015"></a><a name="p11681421162015"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p141691218207"><a name="p141691218207"></a><a name="p141691218207"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row516532142011"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p9169172117203"><a name="p9169172117203"></a><a name="p9169172117203"></a>offset</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p2170142114208"><a name="p2170142114208"></a><a name="p2170142114208"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p2171621152012"><a name="p2171621152012"></a><a name="p2171621152012"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p5172112172013"><a name="p5172112172013"></a><a name="p5172112172013"></a>偏移量。</p>
<p id="p417313211207"><a name="p417313211207"></a><a name="p417313211207"></a>偏移量为一个大于0小于资源总个数的整数，表示查询该偏移量后面的所有的资源，默认值为0。</p>
<p id="p11173621192020"><a name="p11173621192020"></a><a name="p11173621192020"></a>缺省值：<strong id="b1117316213209"><a name="b1117316213209"></a><a name="b1117316213209"></a>0</strong></p>
</td>
</tr>
<tr id="row9165112152019"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p817482142015"><a name="p817482142015"></a><a name="p817482142015"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1017482114201"><a name="p1017482114201"></a><a name="p1017482114201"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p5175112112014"><a name="p5175112112014"></a><a name="p5175112112014"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p61765211205"><a name="p61765211205"></a><a name="p61765211205"></a>查询的数量限制。</p>
<p id="p3177521192011"><a name="p3177521192011"></a><a name="p3177521192011"></a>取值范围：1~100，取值一般为10，20，50。功能说明：每页返回的资源个数。默认值为100。</p>
<p id="p2177521102012"><a name="p2177521102012"></a><a name="p2177521102012"></a>缺省值：<strong id="b217832192011"><a name="b217832192011"></a><a name="b217832192011"></a>100</strong></p>
</td>
</tr>
</tbody>
</table>

## 请求参数<a name="section6178122162020"></a>

**表 3**  请求Header参数

<a name="HeaderParameter"></a>
<table><thead align="left"><tr id="row16179182113209"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p4180132119209"><a name="p4180132119209"></a><a name="p4180132119209"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p918118216206"><a name="p918118216206"></a><a name="p918118216206"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p1818222162013"><a name="p1818222162013"></a><a name="p1818222162013"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p118222120205"><a name="p118222120205"></a><a name="p118222120205"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1717912216209"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p51836212206"><a name="p51836212206"></a><a name="p51836212206"></a>X-Auth-Token</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p4184121162010"><a name="p4184121162010"></a><a name="p4184121162010"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p7184421112018"><a name="p7184421112018"></a><a name="p7184421112018"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p15185621142015"><a name="p15185621142015"></a><a name="p15185621142015"></a>用户Token。</p>
<p id="p151861621152012"><a name="p151861621152012"></a><a name="p151861621152012"></a>通过调用IAM服务获取用户Token接口获取（响应消息头中X-Subject-Token的值）。</p>
</td>
</tr>
</tbody>
</table>

## 响应参数<a name="section1418712218209"></a>

**状态码： 200**

**表 4**  响应Body参数

<a name="responseParameter"></a>
<table><thead align="left"><tr id="row718982132014"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p15191122113209"><a name="p15191122113209"></a><a name="p15191122113209"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p111911121172011"><a name="p111911121172011"></a><a name="p111911121172011"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p1919292122017"><a name="p1919292122017"></a><a name="p1919292122017"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row161891210203"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p71935216208"><a name="p71935216208"></a><a name="p71935216208"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p21948217200"><a name="p21948217200"></a><a name="p21948217200"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p2195102172013"><a name="p2195102172013"></a><a name="p2195102172013"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row101897215207"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p819642117204"><a name="p819642117204"></a><a name="p819642117204"></a>subscription_count</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p5196112118209"><a name="p5196112118209"></a><a name="p5196112118209"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p819762120203"><a name="p819762120203"></a><a name="p819762120203"></a>订阅者个数。</p>
</td>
</tr>
<tr id="row41899218200"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p61981721162014"><a name="p61981721162014"></a><a name="p61981721162014"></a>subscriptions</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p16199321112017"><a name="p16199321112017"></a><a name="p16199321112017"></a>Array of <a href="#response_ListSubscriptionsItem">ListSubscriptionsItem</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p3200421112016"><a name="p3200421112016"></a><a name="p3200421112016"></a>Subscription结构体。</p>
</td>
</tr>
</tbody>
</table>

**表 5**  ListSubscriptionsItem

<a name="response_ListSubscriptionsItem"></a>
<table><thead align="left"><tr id="row13201122112206"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p1520252132019"><a name="p1520252132019"></a><a name="p1520252132019"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p12203102112204"><a name="p12203102112204"></a><a name="p12203102112204"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p162031121172019"><a name="p162031121172019"></a><a name="p162031121172019"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1520119210204"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p120452111205"><a name="p120452111205"></a><a name="p120452111205"></a>topic_urn</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p520592113202"><a name="p520592113202"></a><a name="p520592113202"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p32051521122016"><a name="p32051521122016"></a><a name="p32051521122016"></a>Topic的唯一的资源标识。</p>
</td>
</tr>
<tr id="row220117216205"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p17206421182012"><a name="p17206421182012"></a><a name="p17206421182012"></a>protocol</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p520611219206"><a name="p520611219206"></a><a name="p520611219206"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p320762116200"><a name="p320762116200"></a><a name="p320762116200"></a>不同协议对应不同的endpoint（接受消息的接入点）。目前支持的协议包括：</p>
<a name="ul1922118171455"></a><a name="ul1922118171455"></a><ul id="ul1922118171455"><li>“default”：默认协议。</li><li>“email”：邮件传输协议，endpoint为邮箱地址。</li><li>“sms”：短信传输协议，endpoint为手机号码。</li><li>“functionstage”：FunctionGraph（函数）传输协议，endpoint为一个函数。</li><li>“http”、“https”：HTTP/HTTPS传输协议，endpoint为URL。</li></ul>
</td>
</tr>
<tr id="row1020112162010"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p8212321132014"><a name="p8212321132014"></a><a name="p8212321132014"></a>subscription_urn</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1021322118208"><a name="p1021322118208"></a><a name="p1021322118208"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p6213182116204"><a name="p6213182116204"></a><a name="p6213182116204"></a>订阅者的唯一资源标识。</p>
</td>
</tr>
<tr id="row18201421192013"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p22141821152017"><a name="p22141821152017"></a><a name="p22141821152017"></a>owner</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p202156217201"><a name="p202156217201"></a><a name="p202156217201"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p11215192114201"><a name="p11215192114201"></a><a name="p11215192114201"></a>Topic创建者的项目ID。</p>
</td>
</tr>
<tr id="row1520162113203"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p6216122172017"><a name="p6216122172017"></a><a name="p6216122172017"></a>endpoint</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1216142172016"><a name="p1216142172016"></a><a name="p1216142172016"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p172171215204"><a name="p172171215204"></a><a name="p172171215204"></a>接受消息的接入点。</p>
</td>
</tr>
<tr id="row1201152116206"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p4218921202017"><a name="p4218921202017"></a><a name="p4218921202017"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p19219202112012"><a name="p19219202112012"></a><a name="p19219202112012"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1722002182014"><a name="p1722002182014"></a><a name="p1722002182014"></a>备注。</p>
</td>
</tr>
<tr id="row1520162110203"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1022162114209"><a name="p1022162114209"></a><a name="p1022162114209"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p822111213208"><a name="p822111213208"></a><a name="p822111213208"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1822272102010"><a name="p1822272102010"></a><a name="p1822272102010"></a>订阅者状态：0表示订阅还未确认，1表示已经确认，3表示已经取消确认。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 400**

**表 6**  响应Body参数

<a name="table13223192117202"></a>
<table><thead align="left"><tr id="row42241021182020"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p122672142018"><a name="p122672142018"></a><a name="p122672142018"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p4226152102012"><a name="p4226152102012"></a><a name="p4226152102012"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p19227182117204"><a name="p19227182117204"></a><a name="p19227182117204"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1722412116201"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p422810212200"><a name="p422810212200"></a><a name="p422810212200"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p62281121162014"><a name="p62281121162014"></a><a name="p62281121162014"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p182291621132010"><a name="p182291621132010"></a><a name="p182291621132010"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row1022422192011"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p19230321162019"><a name="p19230321162019"></a><a name="p19230321162019"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1723122152015"><a name="p1723122152015"></a><a name="p1723122152015"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p723214218202"><a name="p723214218202"></a><a name="p723214218202"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row1522422142014"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p923211212202"><a name="p923211212202"></a><a name="p923211212202"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p923322117205"><a name="p923322117205"></a><a name="p923322117205"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p182341521112014"><a name="p182341521112014"></a><a name="p182341521112014"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 403**

**表 7**  响应Body参数

<a name="table192351521182016"></a>
<table><thead align="left"><tr id="row1236162115209"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p1237132142011"><a name="p1237132142011"></a><a name="p1237132142011"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p1423852117208"><a name="p1423852117208"></a><a name="p1423852117208"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p152393218207"><a name="p152393218207"></a><a name="p152393218207"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row12361121202018"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p724062116200"><a name="p724062116200"></a><a name="p724062116200"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p16240521182017"><a name="p16240521182017"></a><a name="p16240521182017"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p19241421192010"><a name="p19241421192010"></a><a name="p19241421192010"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row1323652162019"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1224202111201"><a name="p1224202111201"></a><a name="p1224202111201"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p15243122112014"><a name="p15243122112014"></a><a name="p15243122112014"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p524415218201"><a name="p524415218201"></a><a name="p524415218201"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row1923610210202"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p024492120205"><a name="p024492120205"></a><a name="p024492120205"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p132457217200"><a name="p132457217200"></a><a name="p132457217200"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p19246192132010"><a name="p19246192132010"></a><a name="p19246192132010"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 404**

**表 8**  响应Body参数

<a name="table16247192115203"></a>
<table><thead align="left"><tr id="row142484213205"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p425022117207"><a name="p425022117207"></a><a name="p425022117207"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p62511321102014"><a name="p62511321102014"></a><a name="p62511321102014"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p82511521122015"><a name="p82511521122015"></a><a name="p82511521122015"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1248142119201"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1625215215209"><a name="p1625215215209"></a><a name="p1625215215209"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p19253132116209"><a name="p19253132116209"></a><a name="p19253132116209"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p525319213207"><a name="p525319213207"></a><a name="p525319213207"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row122486215202"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p6254132112013"><a name="p6254132112013"></a><a name="p6254132112013"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1725414215209"><a name="p1725414215209"></a><a name="p1725414215209"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p42551821172014"><a name="p42551821172014"></a><a name="p42551821172014"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row724812216202"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1825632122015"><a name="p1825632122015"></a><a name="p1825632122015"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p13256122162018"><a name="p13256122162018"></a><a name="p13256122162018"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1725710214204"><a name="p1725710214204"></a><a name="p1725710214204"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 500**

**表 9**  响应Body参数

<a name="table12581321112018"></a>
<table><thead align="left"><tr id="row10259521112019"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p19261521192014"><a name="p19261521192014"></a><a name="p19261521192014"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p20262021162013"><a name="p20262021162013"></a><a name="p20262021162013"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p72621721182018"><a name="p72621721182018"></a><a name="p72621721182018"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row17259202114207"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p62631021122011"><a name="p62631021122011"></a><a name="p62631021122011"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p142631021172011"><a name="p142631021172011"></a><a name="p142631021172011"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p182641621142018"><a name="p182641621142018"></a><a name="p182641621142018"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row1425914213205"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p11265102110201"><a name="p11265102110201"></a><a name="p11265102110201"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p10266142172010"><a name="p10266142172010"></a><a name="p10266142172010"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p726792142015"><a name="p726792142015"></a><a name="p726792142015"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row1925942110205"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1826792182019"><a name="p1826792182019"></a><a name="p1826792182019"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p19272321182017"><a name="p19272321182017"></a><a name="p19272321182017"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1827372172011"><a name="p1827372172011"></a><a name="p1827372172011"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

## 请求示例<a name="section16273021162020"></a>

查询指定Topic的订阅者列表

```
GET https://{SMN_Endpoint}/v2/{project_id}/notifications/topics/urn:smn:regionId:762bdb3251034f268af0e395c53ea09b:test_topic_v1/subscriptions?offset=0&limit=100 

null
```

## 响应示例<a name="section227711216200"></a>

**状态码： 200**

OK

```
{
  "request_id" : "6a63a18b8bab40ffb71ebd9cb80d0085",
  "subscription_count" : 2,
  "subscriptions" : [ {
    "topic_urn" : "urn:smn:regionId:762bdb3251034f268af0e395c53ea09b:test_topic_v1",
    "protocol" : "sms",
    "subscription_urn" : "urn:smn:regionId:762bdb3251034f268af0e395c53ea09b:test_topic_v1:2e778e84408e44058e6cbc6d3c377837",
    "owner" : "762bdb3251034f268af0e395c53ea09b",
    "endpoint" : "xxxxxxxxxxx",
    "remark" : "",
    "status" : 0
  }, {
    "topic_urn" : "urn:smn:regionId:762bdb3251034f268af0e395c53ea09b:test_topic_v1",
    "protocol" : "email",
    "subscription_urn" : "urn:smn:regionId:762bdb3251034f268af0e395c53ea09b:test_topic_v1:a2d52a9f5c3b47f48c3fafb177a58796",
    "owner" : "762bdb3251034f268af0e395c53ea09b",
    "endpoint" : "xx@xx.com",
    "remark" : "",
    "status" : 0
  } ]
}
```

## 状态码<a name="section3291162112018"></a>

<a name="status_code"></a>
<table><thead align="left"><tr id="row20292172115202"><th class="cellrowborder" valign="top" width="15%" id="mcps1.1.3.1.1"><p id="p18293122182012"><a name="p18293122182012"></a><a name="p18293122182012"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="85%" id="mcps1.1.3.1.2"><p id="p1629452117200"><a name="p1629452117200"></a><a name="p1629452117200"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1829292111201"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p7294132116203"><a name="p7294132116203"></a><a name="p7294132116203"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p192951621182010"><a name="p192951621182010"></a><a name="p192951621182010"></a>OK</p>
</td>
</tr>
<tr id="row152921921102010"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p172961221182012"><a name="p172961221182012"></a><a name="p172961221182012"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p122961121182010"><a name="p122961121182010"></a><a name="p122961121182010"></a>Bad Request</p>
</td>
</tr>
<tr id="row142921521192017"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p3297142182018"><a name="p3297142182018"></a><a name="p3297142182018"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p929816219208"><a name="p929816219208"></a><a name="p929816219208"></a>Unauthorized</p>
</td>
</tr>
<tr id="row1292202162010"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p9299102132016"><a name="p9299102132016"></a><a name="p9299102132016"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p1146312162017"><a name="p1146312162017"></a><a name="p1146312162017"></a>Not Found</p>
</td>
</tr>
<tr id="row3292142182010"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p144641121192013"><a name="p144641121192013"></a><a name="p144641121192013"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p1346412218201"><a name="p1346412218201"></a><a name="p1346412218201"></a>Internal Server Error</p>
</td>
</tr>
</tbody>
</table>

## 错误码<a name="section94641621182016"></a>

请参见[错误码](错误码.md)。

