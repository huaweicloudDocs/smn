# 授权操作与SMN接口的映射关系<a name="smn_ug_a6000"></a>

**表 1**  授权操作与SMN接口的映射关系

<a name="table40610457155253"></a>
<table><thead align="left"><tr id="row7466420155253"><th class="cellrowborder" valign="top" width="36.53%" id="mcps1.2.4.1.1"><p id="p7202482155253"><a name="p7202482155253"></a><a name="p7202482155253"></a><strong id="b457112616320"><a name="b457112616320"></a><a name="b457112616320"></a>授权操作</strong></p>
</th>
<th class="cellrowborder" valign="top" width="32.769999999999996%" id="mcps1.2.4.1.2"><p id="p46530145155253"><a name="p46530145155253"></a><a name="p46530145155253"></a><strong id="b3471693616320"><a name="b3471693616320"></a><a name="b3471693616320"></a>接口名称</strong></p>
</th>
<th class="cellrowborder" valign="top" width="30.7%" id="mcps1.2.4.1.3"><p id="p10845389155253"><a name="p10845389155253"></a><a name="p10845389155253"></a><strong id="b6060845516320"><a name="b6060845516320"></a><a name="b6060845516320"></a>接口功能</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="row30499637155253"><td class="cellrowborder" valign="top" width="36.53%" headers="mcps1.2.4.1.1 "><p id="p4199904616713"><a name="p4199904616713"></a><a name="p4199904616713"></a>SMN:UpdateTopic</p>
</td>
<td class="cellrowborder" valign="top" width="32.769999999999996%" headers="mcps1.2.4.1.2 "><p id="p56594888155253"><a name="p56594888155253"></a><a name="p56594888155253"></a>UpdateTopic</p>
</td>
<td class="cellrowborder" valign="top" width="30.7%" headers="mcps1.2.4.1.3 "><p id="p30182576161234"><a name="p30182576161234"></a><a name="p30182576161234"></a>修改主题的属性，目前仅仅支持修改topic的display_name字段。</p>
</td>
</tr>
<tr id="row52831096155253"><td class="cellrowborder" valign="top" width="36.53%" headers="mcps1.2.4.1.1 "><p id="p253506116713"><a name="p253506116713"></a><a name="p253506116713"></a>SMN:DeleteTopic</p>
</td>
<td class="cellrowborder" valign="top" width="32.769999999999996%" headers="mcps1.2.4.1.2 "><p id="p7542409155253"><a name="p7542409155253"></a><a name="p7542409155253"></a>DeleteTopic</p>
</td>
<td class="cellrowborder" valign="top" width="30.7%" headers="mcps1.2.4.1.3 "><p id="p1549416916138"><a name="p1549416916138"></a><a name="p1549416916138"></a>删除一个主题以及它的所有订阅者。删除Topic操作可能会导致未推送的消息无法再推送给该Topic的订阅者。</p>
</td>
</tr>
<tr id="row62598497155253"><td class="cellrowborder" valign="top" width="36.53%" headers="mcps1.2.4.1.1 "><p id="p1429388816713"><a name="p1429388816713"></a><a name="p1429388816713"></a>SMN:QueryTopicDetail</p>
</td>
<td class="cellrowborder" valign="top" width="32.769999999999996%" headers="mcps1.2.4.1.2 "><p id="p2493507155253"><a name="p2493507155253"></a><a name="p2493507155253"></a>QueryTopicDetail</p>
</td>
<td class="cellrowborder" valign="top" width="30.7%" headers="mcps1.2.4.1.3 "><p id="p51055184161330"><a name="p51055184161330"></a><a name="p51055184161330"></a>查询Topic的详细信息。</p>
</td>
</tr>
<tr id="row5827766155253"><td class="cellrowborder" valign="top" width="36.53%" headers="mcps1.2.4.1.1 "><p id="p3763483316713"><a name="p3763483316713"></a><a name="p3763483316713"></a>SMN:ListTopicAttributes</p>
</td>
<td class="cellrowborder" valign="top" width="32.769999999999996%" headers="mcps1.2.4.1.2 "><p id="p51030558155253"><a name="p51030558155253"></a><a name="p51030558155253"></a>ListTopicAttributes</p>
</td>
<td class="cellrowborder" valign="top" width="30.7%" headers="mcps1.2.4.1.3 "><p id="p61745869161340"><a name="p61745869161340"></a><a name="p61745869161340"></a>查询Topic的属性信息。</p>
</td>
</tr>
<tr id="row22966150155253"><td class="cellrowborder" valign="top" width="36.53%" headers="mcps1.2.4.1.1 "><p id="p4588028416713"><a name="p4588028416713"></a><a name="p4588028416713"></a>SMN:UpdateTopicAttribute</p>
</td>
<td class="cellrowborder" valign="top" width="32.769999999999996%" headers="mcps1.2.4.1.2 "><p id="p21511815155253"><a name="p21511815155253"></a><a name="p21511815155253"></a>UpdateTopicAttribute</p>
</td>
<td class="cellrowborder" valign="top" width="30.7%" headers="mcps1.2.4.1.3 "><p id="p14685560161438"><a name="p14685560161438"></a><a name="p14685560161438"></a>更新Topic的属性。</p>
</td>
</tr>
<tr id="row45748200155253"><td class="cellrowborder" valign="top" width="36.53%" headers="mcps1.2.4.1.1 "><p id="p3861765816713"><a name="p3861765816713"></a><a name="p3861765816713"></a>SMN:DeleteTopicAttributes</p>
</td>
<td class="cellrowborder" valign="top" width="32.769999999999996%" headers="mcps1.2.4.1.2 "><p id="p43102455155253"><a name="p43102455155253"></a><a name="p43102455155253"></a>DeleteTopicAttributes</p>
</td>
<td class="cellrowborder" valign="top" width="30.7%" headers="mcps1.2.4.1.3 "><p id="p1637937155253"><a name="p1637937155253"></a><a name="p1637937155253"></a>删除所有Topic属性。</p>
</td>
</tr>
<tr id="row14741435155253"><td class="cellrowborder" valign="top" width="36.53%" headers="mcps1.2.4.1.1 "><p id="p3831067116713"><a name="p3831067116713"></a><a name="p3831067116713"></a>SMN:DeleteTopicAttributeByName</p>
</td>
<td class="cellrowborder" valign="top" width="32.769999999999996%" headers="mcps1.2.4.1.2 "><p id="p14685611155253"><a name="p14685611155253"></a><a name="p14685611155253"></a>DeleteTopicAttributeByName</p>
</td>
<td class="cellrowborder" valign="top" width="30.7%" headers="mcps1.2.4.1.3 "><p id="p20696347161512"><a name="p20696347161512"></a><a name="p20696347161512"></a>删除指定名称的Topic属性。</p>
</td>
</tr>
<tr id="row3257009916547"><td class="cellrowborder" valign="top" width="36.53%" headers="mcps1.2.4.1.1 "><p id="p6285939916713"><a name="p6285939916713"></a><a name="p6285939916713"></a>SMN:ListSubscriptionsByTopic</p>
</td>
<td class="cellrowborder" valign="top" width="32.769999999999996%" headers="mcps1.2.4.1.2 "><p id="p1779667816547"><a name="p1779667816547"></a><a name="p1779667816547"></a>ListSubscriptionsByTopic</p>
</td>
<td class="cellrowborder" valign="top" width="30.7%" headers="mcps1.2.4.1.3 "><p id="p48133186161538"><a name="p48133186161538"></a><a name="p48133186161538"></a>分页获取特定主题的订阅列表，订阅列表按照订阅创建时间进行升序排列。分页查询可以指定offset以及limit。如果指定主题不存在订阅者，返回空列表。</p>
</td>
</tr>
<tr id="row6424497716551"><td class="cellrowborder" valign="top" width="36.53%" headers="mcps1.2.4.1.1 "><p id="p6625710816713"><a name="p6625710816713"></a><a name="p6625710816713"></a>SMN:Subscribe</p>
</td>
<td class="cellrowborder" valign="top" width="32.769999999999996%" headers="mcps1.2.4.1.2 "><p id="p52424616551"><a name="p52424616551"></a><a name="p52424616551"></a>Subscribe</p>
</td>
<td class="cellrowborder" valign="top" width="30.7%" headers="mcps1.2.4.1.3 "><p id="p61570312161554"><a name="p61570312161554"></a><a name="p61570312161554"></a>为指定Topic添加一个订阅者，并向订阅者发送一个确认的消息。待订阅者进行ConfirmSubscription确认后，该订阅者才能收到Topic发布的消息。</p>
</td>
</tr>
<tr id="row1552135216559"><td class="cellrowborder" valign="top" width="36.53%" headers="mcps1.2.4.1.1 "><p id="p184048016713"><a name="p184048016713"></a><a name="p184048016713"></a>SMN:Unsubscribe</p>
</td>
<td class="cellrowborder" valign="top" width="32.769999999999996%" headers="mcps1.2.4.1.2 "><p id="p3144820416559"><a name="p3144820416559"></a><a name="p3144820416559"></a>Unsubscribe</p>
</td>
<td class="cellrowborder" valign="top" width="30.7%" headers="mcps1.2.4.1.3 "><p id="p41500538161616"><a name="p41500538161616"></a><a name="p41500538161616"></a>删除一个订阅，订阅需要鉴权才能删除，仅仅订阅者或者这个主题的拥有者可以删除，删除时会对身份进行确认。</p>
</td>
</tr>
<tr id="row501468261662"><td class="cellrowborder" valign="top" width="36.53%" headers="mcps1.2.4.1.1 "><p id="p2425111816713"><a name="p2425111816713"></a><a name="p2425111816713"></a>SMN:Publish</p>
</td>
<td class="cellrowborder" valign="top" width="32.769999999999996%" headers="mcps1.2.4.1.2 "><p id="p456766331662"><a name="p456766331662"></a><a name="p456766331662"></a>Publish</p>
</td>
<td class="cellrowborder" valign="top" width="30.7%" headers="mcps1.2.4.1.3 "><p id="p88198101662"><a name="p88198101662"></a><a name="p88198101662"></a>将消息发送给Topic的所有订阅端点。当返回消息ID时，该消息已被保存并开始尝试将其推送给主题的订阅者。消息格式，取决于该主题每一个订阅者的通知协议。</p>
</td>
</tr>
</tbody>
</table>

