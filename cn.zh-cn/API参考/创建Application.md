# 创建Application<a name="CreateApplication"></a>

## 功能介绍<a name="section6298175820200"></a>

创建平台应用。

## 调试<a name="section1056114122524"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=SMN&api=ListTopics)中调试该接口。

## URI<a name="section230165832013"></a>

POST /v2/\{project\_id\}/notifications/applications

**表 1**  路径参数

<a name="table1430545842019"></a>
<table><thead align="left"><tr id="row9303125817209"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p1130612584207"><a name="p1130612584207"></a><a name="p1130612584207"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p1230605810208"><a name="p1230605810208"></a><a name="p1230605810208"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p13072058162019"><a name="p13072058162019"></a><a name="p13072058162019"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p133081358122010"><a name="p133081358122010"></a><a name="p133081358122010"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row430485810205"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p193091858102016"><a name="p193091858102016"></a><a name="p193091858102016"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p1030955842010"><a name="p1030955842010"></a><a name="p1030955842010"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p173102586205"><a name="p173102586205"></a><a name="p173102586205"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p15311195872013"><a name="p15311195872013"></a><a name="p15311195872013"></a>项目ID。</p>
<p id="p4568812165217"><a name="p4568812165217"></a><a name="p4568812165217"></a>获取项目ID请参考<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
</tbody>
</table>

## 请求参数<a name="section1631255822019"></a>

**表 2**  请求Header参数

<a name="HeaderParameter"></a>
<table><thead align="left"><tr id="row1031485814206"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p11315135820203"><a name="p11315135820203"></a><a name="p11315135820203"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p13316558172010"><a name="p13316558172010"></a><a name="p13316558172010"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p13161858142012"><a name="p13161858142012"></a><a name="p13161858142012"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p03171158132013"><a name="p03171158132013"></a><a name="p03171158132013"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row193141458152015"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p15318658172015"><a name="p15318658172015"></a><a name="p15318658172015"></a>X-Auth-Token</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p931835812201"><a name="p931835812201"></a><a name="p931835812201"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1331914582202"><a name="p1331914582202"></a><a name="p1331914582202"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p3320135813201"><a name="p3320135813201"></a><a name="p3320135813201"></a>用户Token。</p>
<p id="p1532112585200"><a name="p1532112585200"></a><a name="p1532112585200"></a>通过调用IAM服务获取用户Token接口获取（响应消息头中X-Subject-Token的值）。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  请求Body参数

<a name="requestParameter"></a>
<table><thead align="left"><tr id="row16322858122014"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p73231958152018"><a name="p73231958152018"></a><a name="p73231958152018"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.2"><p id="p432435816205"><a name="p432435816205"></a><a name="p432435816205"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p732465842013"><a name="p732465842013"></a><a name="p732465842013"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.5.1.4"><p id="p032511583207"><a name="p032511583207"></a><a name="p032511583207"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row183224580208"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p103261258172011"><a name="p103261258172011"></a><a name="p103261258172011"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p93271458112016"><a name="p93271458112016"></a><a name="p93271458112016"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p18328155812019"><a name="p18328155812019"></a><a name="p18328155812019"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p1032825832017"><a name="p1032825832017"></a><a name="p1032825832017"></a>应用名。</p>
<p id="p93291358192011"><a name="p93291358192011"></a><a name="p93291358192011"></a>最大支持64个字符，只能包含英文字母、下划线和数字。</p>
</td>
</tr>
<tr id="row7322105820207"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p433010580207"><a name="p433010580207"></a><a name="p433010580207"></a>platform</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p9331205832014"><a name="p9331205832014"></a><a name="p9331205832014"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p53311358162016"><a name="p53311358162016"></a><a name="p53311358162016"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p14332105852018"><a name="p14332105852018"></a><a name="p14332105852018"></a>应用平台。</p>
<p id="p433365852010"><a name="p433365852010"></a><a name="p433365852010"></a>目前仅支持HMS、APNS、APNS_SANDBOX。</p>
<p id="p7333125842016"><a name="p7333125842016"></a><a name="p7333125842016"></a>HMS是为开发者提供的消息推送平台。</p>
<p id="p18333195882012"><a name="p18333195882012"></a><a name="p18333195882012"></a>APNS和APNS_SANDBOX是用于推送iOS消息的服务平台。</p>
</td>
</tr>
<tr id="row1432295819204"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p03341958142017"><a name="p03341958142017"></a><a name="p03341958142017"></a>platform_principal</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p8335175810203"><a name="p8335175810203"></a><a name="p8335175810203"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p18335105813205"><a name="p18335105813205"></a><a name="p18335105813205"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p933614584204"><a name="p933614584204"></a><a name="p933614584204"></a>对于HMS平台是APP ID，只能包含英文字母和数字，最大20个字符。 对于苹果APNS、APNS_SandBox平台是推送证书，大小不超过8K，且是Base64编码。</p>
</td>
</tr>
<tr id="row1032225852013"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1733725819208"><a name="p1733725819208"></a><a name="p1733725819208"></a>platform_credential</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.2 "><p id="p173371458172012"><a name="p173371458172012"></a><a name="p173371458172012"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p20338145832018"><a name="p20338145832018"></a><a name="p20338145832018"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.5.1.4 "><p id="p633915819208"><a name="p633915819208"></a><a name="p633915819208"></a>对于HMS平台是APP SECRET， 只能包含英文字母和数字，32到64个字符。</p>
<p id="p19339135812206"><a name="p19339135812206"></a><a name="p19339135812206"></a>对于苹果APNS、APNS_SandBox平台是推送证书的私钥（private key）， 大小不超过8K，且是Base64编码。</p>
</td>
</tr>
</tbody>
</table>

## 响应参数<a name="section1434010586204"></a>

**状态码： 201**

**表 4**  响应Body参数

<a name="responseParameter"></a>
<table><thead align="left"><tr id="row1434265852016"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p63440587200"><a name="p63440587200"></a><a name="p63440587200"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p1734575832012"><a name="p1734575832012"></a><a name="p1734575832012"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p934635814206"><a name="p934635814206"></a><a name="p934635814206"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row133421582207"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p113468589205"><a name="p113468589205"></a><a name="p113468589205"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1734775822019"><a name="p1734775822019"></a><a name="p1734775822019"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p7348458142010"><a name="p7348458142010"></a><a name="p7348458142010"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row43428586204"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p143492058162011"><a name="p143492058162011"></a><a name="p143492058162011"></a>application_urn</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p93491658112010"><a name="p93491658112010"></a><a name="p93491658112010"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p7350958202016"><a name="p7350958202016"></a><a name="p7350958202016"></a>Application的唯一资源标识。</p>
</td>
</tr>
<tr id="row334215811208"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1635165814204"><a name="p1635165814204"></a><a name="p1635165814204"></a>application_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p18351858192015"><a name="p18351858192015"></a><a name="p18351858192015"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p6352358112010"><a name="p6352358112010"></a><a name="p6352358112010"></a>Application资源的ID。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 400**

**表 5**  响应Body参数

<a name="table18353115815204"></a>
<table><thead align="left"><tr id="row0354658122012"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p8356458142012"><a name="p8356458142012"></a><a name="p8356458142012"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p4357115817205"><a name="p4357115817205"></a><a name="p4357115817205"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p435815819201"><a name="p435815819201"></a><a name="p435815819201"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row6354758132014"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p103582582205"><a name="p103582582205"></a><a name="p103582582205"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p73592588209"><a name="p73592588209"></a><a name="p73592588209"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p83604583207"><a name="p83604583207"></a><a name="p83604583207"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row1235420582203"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p836020585204"><a name="p836020585204"></a><a name="p836020585204"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p17361958182019"><a name="p17361958182019"></a><a name="p17361958182019"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p436214587205"><a name="p436214587205"></a><a name="p436214587205"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row53544581202"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p13631588200"><a name="p13631588200"></a><a name="p13631588200"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1436475810201"><a name="p1436475810201"></a><a name="p1436475810201"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p836485819206"><a name="p836485819206"></a><a name="p836485819206"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 403**

**表 6**  响应Body参数

<a name="table133659585205"></a>
<table><thead align="left"><tr id="row93662058152012"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p13679588201"><a name="p13679588201"></a><a name="p13679588201"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p4368205819208"><a name="p4368205819208"></a><a name="p4368205819208"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p536825872015"><a name="p536825872015"></a><a name="p536825872015"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row136619584209"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p163691658122016"><a name="p163691658122016"></a><a name="p163691658122016"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p5370135815205"><a name="p5370135815205"></a><a name="p5370135815205"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1437011582202"><a name="p1437011582202"></a><a name="p1437011582202"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row153661658112019"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p03712587202"><a name="p03712587202"></a><a name="p03712587202"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p737215819209"><a name="p737215819209"></a><a name="p737215819209"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1137265812209"><a name="p1137265812209"></a><a name="p1137265812209"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row1136655892015"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p123731258132019"><a name="p123731258132019"></a><a name="p123731258132019"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p5374105872019"><a name="p5374105872019"></a><a name="p5374105872019"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p20374125815201"><a name="p20374125815201"></a><a name="p20374125815201"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 404**

**表 7**  响应Body参数

<a name="table153751258202015"></a>
<table><thead align="left"><tr id="row93777581201"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p537819585205"><a name="p537819585205"></a><a name="p537819585205"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p7379658162020"><a name="p7379658162020"></a><a name="p7379658162020"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p5380105852016"><a name="p5380105852016"></a><a name="p5380105852016"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row16377145810202"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1638065872015"><a name="p1638065872015"></a><a name="p1638065872015"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1538115862018"><a name="p1538115862018"></a><a name="p1538115862018"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p183821758192012"><a name="p183821758192012"></a><a name="p183821758192012"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row20377185892018"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p103833580201"><a name="p103833580201"></a><a name="p103833580201"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p33835585201"><a name="p33835585201"></a><a name="p33835585201"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p73841258182017"><a name="p73841258182017"></a><a name="p73841258182017"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row8377758162016"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p738565812010"><a name="p738565812010"></a><a name="p738565812010"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p538585832014"><a name="p538585832014"></a><a name="p538585832014"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p14386458102014"><a name="p14386458102014"></a><a name="p14386458102014"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

**状态码： 500**

**表 8**  响应Body参数

<a name="table638725842019"></a>
<table><thead align="left"><tr id="row2038895812207"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p739017581207"><a name="p739017581207"></a><a name="p739017581207"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p33918580201"><a name="p33918580201"></a><a name="p33918580201"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p133915583200"><a name="p133915583200"></a><a name="p133915583200"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row93881358132011"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p439255811203"><a name="p439255811203"></a><a name="p439255811203"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p539375812020"><a name="p539375812020"></a><a name="p539375812020"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1239445842016"><a name="p1239445842016"></a><a name="p1239445842016"></a>请求的唯一标识ID。</p>
</td>
</tr>
<tr id="row43886587201"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p11395175814203"><a name="p11395175814203"></a><a name="p11395175814203"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p6396155872017"><a name="p6396155872017"></a><a name="p6396155872017"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p2397165822013"><a name="p2397165822013"></a><a name="p2397165822013"></a>服务异常错误信息编码。</p>
</td>
</tr>
<tr id="row12388175872019"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p103981158102017"><a name="p103981158102017"></a><a name="p103981158102017"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p103981058102016"><a name="p103981058102016"></a><a name="p103981058102016"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p2039985817206"><a name="p2039985817206"></a><a name="p2039985817206"></a>服务异常错误信息描述。</p>
</td>
</tr>
</tbody>
</table>

## 请求示例<a name="section154008584205"></a>

创建Application

```
POST https://{SMN_Endpoint}/v2/{project_id}/notifications/applications

{
  "name" : "application_name",
  "platform" : "HMS",
  "platform_principal" : "appId",
  "platform_credential" : "appSecret"
}
```

## 响应示例<a name="section1540585817209"></a>

无

## 状态码<a name="section9407115802016"></a>

<a name="status_code"></a>
<table><thead align="left"><tr id="row640811583202"><th class="cellrowborder" valign="top" width="15%" id="mcps1.1.3.1.1"><p id="p640915587203"><a name="p640915587203"></a><a name="p640915587203"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="85%" id="mcps1.1.3.1.2"><p id="p7410145812010"><a name="p7410145812010"></a><a name="p7410145812010"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1040817587202"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p841185892019"><a name="p841185892019"></a><a name="p841185892019"></a>201</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p1941210582203"><a name="p1941210582203"></a><a name="p1941210582203"></a>OK</p>
</td>
</tr>
<tr id="row1140815585207"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p15412125822016"><a name="p15412125822016"></a><a name="p15412125822016"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p741325816207"><a name="p741325816207"></a><a name="p741325816207"></a>Bad Request</p>
</td>
</tr>
<tr id="row11408115862010"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p64145584206"><a name="p64145584206"></a><a name="p64145584206"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p241445812017"><a name="p241445812017"></a><a name="p241445812017"></a>Unauthorized</p>
</td>
</tr>
<tr id="row1340810588207"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p104152058162018"><a name="p104152058162018"></a><a name="p104152058162018"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p1141685813202"><a name="p1141685813202"></a><a name="p1141685813202"></a>Not Found</p>
</td>
</tr>
<tr id="row16408165814205"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p11417458162018"><a name="p11417458162018"></a><a name="p11417458162018"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p194181585201"><a name="p194181585201"></a><a name="p194181585201"></a>Internal Server Error</p>
</td>
</tr>
</tbody>
</table>

## 错误码<a name="section2419185810207"></a>

请参见[错误码](错误码.md)。

