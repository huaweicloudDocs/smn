# Sms\_template结构体<a name="ZH-CN_TOPIC_0093942647"></a>

Sms\_template结构体参数说明。

<a name="table5134820185815"></a>
<table><thead align="left"><tr id="row724342018581"><th class="cellrowborder" valign="top" width="19.39%" id="mcps1.1.5.1.1"><p id="p9243120135815"><a name="p9243120135815"></a><a name="p9243120135815"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="19.39%" id="mcps1.1.5.1.2"><p id="p8243320135814"><a name="p8243320135814"></a><a name="p8243320135814"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="26.529999999999998%" id="mcps1.1.5.1.3"><p id="p3243820105819"><a name="p3243820105819"></a><a name="p3243820105819"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="34.69%" id="mcps1.1.5.1.4"><p id="p124372013585"><a name="p124372013585"></a><a name="p124372013585"></a>约束</p>
</th>
</tr>
</thead>
<tbody><tr id="row6243172019587"><td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.1.5.1.1 "><p id="p424322018589"><a name="p424322018589"></a><a name="p424322018589"></a>sms_template_name</p>
</td>
<td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.1.5.1.2 "><p id="p102431202589"><a name="p102431202589"></a><a name="p102431202589"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.1.5.1.3 "><p id="p62432204581"><a name="p62432204581"></a><a name="p62432204581"></a>短信模板名称</p>
</td>
<td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.1.5.1.4 "><p id="p17243102014588"><a name="p17243102014588"></a><a name="p17243102014588"></a>64个字符</p>
</td>
</tr>
<tr id="row142431720165819"><td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.1.5.1.1 "><p id="p122430205585"><a name="p122430205585"></a><a name="p122430205585"></a>sms_template_type</p>
</td>
<td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.1.5.1.2 "><p id="p4243142085814"><a name="p4243142085814"></a><a name="p4243142085814"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.1.5.1.3 "><p id="p19243132035810"><a name="p19243132035810"></a><a name="p19243132035810"></a>短信模板类型</p>
</td>
<td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.1.5.1.4 "><p id="p378082816588"><a name="p378082816588"></a><a name="p378082816588"></a>0：通知类模板</p>
<p id="p11514182915585"><a name="p11514182915585"></a><a name="p11514182915585"></a>1：推广类模板</p>
</td>
</tr>
<tr id="row7243172035811"><td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.1.5.1.1 "><p id="p0243120155817"><a name="p0243120155817"></a><a name="p0243120155817"></a>sms_template_id</p>
</td>
<td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.1.5.1.2 "><p id="p16243142016584"><a name="p16243142016584"></a><a name="p16243142016584"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.1.5.1.3 "><p id="p7243620145817"><a name="p7243620145817"></a><a name="p7243620145817"></a>短信模板唯一标示</p>
</td>
<td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.1.5.1.4 "><p id="p8243220115814"><a name="p8243220115814"></a><a name="p8243220115814"></a>UUID</p>
</td>
</tr>
<tr id="row1724342055818"><td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.1.5.1.1 "><p id="p5243720205817"><a name="p5243720205817"></a><a name="p5243720205817"></a>reply</p>
</td>
<td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.1.5.1.2 "><p id="p1243120195814"><a name="p1243120195814"></a><a name="p1243120195814"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.1.5.1.3 "><p id="p024322013582"><a name="p024322013582"></a><a name="p024322013582"></a>运营商审批返回的失败原因</p>
</td>
<td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.1.5.1.4 "><p id="p775982465812"><a name="p775982465812"></a><a name="p775982465812"></a>-</p>
</td>
</tr>
<tr id="row0243152035816"><td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.1.5.1.1 "><p id="p142430203586"><a name="p142430203586"></a><a name="p142430203586"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.1.5.1.2 "><p id="p1243220155810"><a name="p1243220155810"></a><a name="p1243220155810"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.1.5.1.3 "><p id="p424352045814"><a name="p424352045814"></a><a name="p424352045814"></a>模板状态</p>
</td>
<td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.1.5.1.4 "><p id="p152431206585"><a name="p152431206585"></a><a name="p152431206585"></a>0：审批中</p>
<p id="p102439204583"><a name="p102439204583"></a><a name="p102439204583"></a>1：审批通过</p>
<p id="p18243162016584"><a name="p18243162016584"></a><a name="p18243162016584"></a>2：审批不通过</p>
<p id="p62431720135810"><a name="p62431720135810"></a><a name="p62431720135810"></a>3：已失效</p>
</td>
</tr>
<tr id="row32432020105819"><td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.1.5.1.1 "><p id="p3243520175814"><a name="p3243520175814"></a><a name="p3243520175814"></a>create_time</p>
</td>
<td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.1.5.1.2 "><p id="p624315204585"><a name="p624315204585"></a><a name="p624315204585"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.1.5.1.3 "><p id="p18243172065815"><a name="p18243172065815"></a><a name="p18243172065815"></a>模板创建时间</p>
</td>
<td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.1.5.1.4 "><p id="p12438204589"><a name="p12438204589"></a><a name="p12438204589"></a>-</p>
</td>
</tr>
<tr id="row4243152019580"><td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.1.5.1.1 "><p id="p724382020580"><a name="p724382020580"></a><a name="p724382020580"></a>validity_end_time</p>
</td>
<td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.1.5.1.2 "><p id="p14243112017587"><a name="p14243112017587"></a><a name="p14243112017587"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.1.5.1.3 "><p id="p12243720155812"><a name="p12243720155812"></a><a name="p12243720155812"></a>模板失效时间</p>
</td>
<td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.1.5.1.4 "><p id="p13243142065814"><a name="p13243142065814"></a><a name="p13243142065814"></a>-</p>
</td>
</tr>
<tr id="row1997134217424"><td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.1.5.1.1 "><p id="p12269848134213"><a name="p12269848134213"></a><a name="p12269848134213"></a>sign_id</p>
</td>
<td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.1.5.1.2 "><p id="p1126954814427"><a name="p1126954814427"></a><a name="p1126954814427"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.1.5.1.3 "><p id="p926964812423"><a name="p926964812423"></a><a name="p926964812423"></a>该短信模板关联的签名ID</p>
</td>
<td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.1.5.1.4 "><p id="p112691248144213"><a name="p112691248144213"></a><a name="p112691248144213"></a>-</p>
</td>
</tr>
</tbody>
</table>

