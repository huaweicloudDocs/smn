# Sms\_report\_data结构体<a name="ZH-CN_TOPIC_0080900093"></a>

Sms\_report\_data结构体参数说明。

<a name="table61405338103716"></a>
<table><thead align="left"><tr id="row35573802103716"><th class="cellrowborder" valign="top" width="19.39193919391939%" id="mcps1.1.5.1.1"><p id="p62905748103716"><a name="p62905748103716"></a><a name="p62905748103716"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="19.251925192519252%" id="mcps1.1.5.1.2"><p id="p62200855103716"><a name="p62200855103716"></a><a name="p62200855103716"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="26.662666266626662%" id="mcps1.1.5.1.3"><p id="p5104474103716"><a name="p5104474103716"></a><a name="p5104474103716"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="34.69346934693469%" id="mcps1.1.5.1.4"><p id="p10809221103716"><a name="p10809221103716"></a><a name="p10809221103716"></a>约束</p>
</th>
</tr>
</thead>
<tbody><tr id="row3131713103716"><td class="cellrowborder" valign="top" width="19.39193919391939%" headers="mcps1.1.5.1.1 "><p id="p52342197103716"><a name="p52342197103716"></a><a name="p52342197103716"></a>message_id</p>
</td>
<td class="cellrowborder" valign="top" width="19.251925192519252%" headers="mcps1.1.5.1.2 "><p id="p11859594103716"><a name="p11859594103716"></a><a name="p11859594103716"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="26.662666266626662%" headers="mcps1.1.5.1.3 "><p id="p21103080103716"><a name="p21103080103716"></a><a name="p21103080103716"></a>唯一的消息ID。</p>
</td>
<td class="cellrowborder" valign="top" width="34.69346934693469%" headers="mcps1.1.5.1.4 "><p id="p31627894103716"><a name="p31627894103716"></a><a name="p31627894103716"></a>-</p>
</td>
</tr>
<tr id="row16215590103716"><td class="cellrowborder" valign="top" width="19.39193919391939%" headers="mcps1.1.5.1.1 "><p id="p38394432103716"><a name="p38394432103716"></a><a name="p38394432103716"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="19.251925192519252%" headers="mcps1.1.5.1.2 "><p id="p22941278103716"><a name="p22941278103716"></a><a name="p22941278103716"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="26.662666266626662%" headers="mcps1.1.5.1.3 "><p id="p46304233103716"><a name="p46304233103716"></a><a name="p46304233103716"></a>短信的发送状态。</p>
</td>
<td class="cellrowborder" valign="top" width="34.69346934693469%" headers="mcps1.1.5.1.4 "><p id="p14956111511456"><a name="p14956111511456"></a><a name="p14956111511456"></a>0 ：短信已发送，等待短信接收状态</p>
<p id="p119561715104511"><a name="p119561715104511"></a><a name="p119561715104511"></a>1 ：短信发送成功</p>
<p id="p11956181544517"><a name="p11956181544517"></a><a name="p11956181544517"></a>2 ：短信发送失败</p>
</td>
</tr>
<tr id="row27403103716"><td class="cellrowborder" valign="top" width="19.39193919391939%" headers="mcps1.1.5.1.1 "><p id="p2219652103716"><a name="p2219652103716"></a><a name="p2219652103716"></a>sign_id</p>
</td>
<td class="cellrowborder" valign="top" width="19.251925192519252%" headers="mcps1.1.5.1.2 "><p id="p45574085103716"><a name="p45574085103716"></a><a name="p45574085103716"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="26.662666266626662%" headers="mcps1.1.5.1.3 "><p id="p513399103716"><a name="p513399103716"></a><a name="p513399103716"></a>短信签名ID。</p>
</td>
<td class="cellrowborder" valign="top" width="34.69346934693469%" headers="mcps1.1.5.1.4 "><p id="p41585345103716"><a name="p41585345103716"></a><a name="p41585345103716"></a>-</p>
</td>
</tr>
<tr id="row38723791103716"><td class="cellrowborder" valign="top" width="19.39193919391939%" headers="mcps1.1.5.1.1 "><p id="p49619377103716"><a name="p49619377103716"></a><a name="p49619377103716"></a>status_desc</p>
</td>
<td class="cellrowborder" valign="top" width="19.251925192519252%" headers="mcps1.1.5.1.2 "><p id="p59746624103716"><a name="p59746624103716"></a><a name="p59746624103716"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="26.662666266626662%" headers="mcps1.1.5.1.3 "><p id="p7638371103716"><a name="p7638371103716"></a><a name="p7638371103716"></a>发送状态描述，包含错误码。</p>
</td>
<td class="cellrowborder" valign="top" width="34.69346934693469%" headers="mcps1.1.5.1.4 "><p id="p49344087103922"><a name="p49344087103922"></a><a name="p49344087103922"></a>当前仅只支持特定的状态，请参见<a href="Cmpp发送状态描述表.md">Cmpp发送状态描述表</a>。</p>
</td>
</tr>
<tr id="row65446045103716"><td class="cellrowborder" valign="top" width="19.39193919391939%" headers="mcps1.1.5.1.1 "><p id="p66638274103716"><a name="p66638274103716"></a><a name="p66638274103716"></a>fee_num</p>
</td>
<td class="cellrowborder" valign="top" width="19.251925192519252%" headers="mcps1.1.5.1.2 "><p id="p28991128103716"><a name="p28991128103716"></a><a name="p28991128103716"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="26.662666266626662%" headers="mcps1.1.5.1.3 "><p id="p66580038103716"><a name="p66580038103716"></a><a name="p66580038103716"></a>短信计费条数。</p>
</td>
<td class="cellrowborder" valign="top" width="34.69346934693469%" headers="mcps1.1.5.1.4 "><p id="p8284231175014"><a name="p8284231175014"></a><a name="p8284231175014"></a>计算短信字数时，包含短信签名。当短信字数不超过70时，按照70字/条计费。当短信字数超过70时，即为长短信，按照67字/条计算。</p>
<p id="p198005151504"><a name="p198005151504"></a><a name="p198005151504"></a>例如，系统发送一条包含490个字符的短信，则计算为490/67=7.31，即8条。</p>
</td>
</tr>
<tr id="row17139749103716"><td class="cellrowborder" valign="top" width="19.39193919391939%" headers="mcps1.1.5.1.1 "><p id="p46142391103716"><a name="p46142391103716"></a><a name="p46142391103716"></a>extend_code</p>
</td>
<td class="cellrowborder" valign="top" width="19.251925192519252%" headers="mcps1.1.5.1.2 "><p id="p46546206103716"><a name="p46546206103716"></a><a name="p46546206103716"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="26.662666266626662%" headers="mcps1.1.5.1.3 "><p id="p12146370103716"><a name="p12146370103716"></a><a name="p12146370103716"></a>扩展码。</p>
</td>
<td class="cellrowborder" valign="top" width="34.69346934693469%" headers="mcps1.1.5.1.4 "><p id="p44331914103716"><a name="p44331914103716"></a><a name="p44331914103716"></a>-</p>
</td>
</tr>
<tr id="row63442911103716"><td class="cellrowborder" valign="top" width="19.39193919391939%" headers="mcps1.1.5.1.1 "><p id="p38602201103716"><a name="p38602201103716"></a><a name="p38602201103716"></a>nation_code</p>
</td>
<td class="cellrowborder" valign="top" width="19.251925192519252%" headers="mcps1.1.5.1.2 "><p id="p39770604103716"><a name="p39770604103716"></a><a name="p39770604103716"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="26.662666266626662%" headers="mcps1.1.5.1.3 "><p id="p193471103716"><a name="p193471103716"></a><a name="p193471103716"></a>国家码。</p>
</td>
<td class="cellrowborder" valign="top" width="34.69346934693469%" headers="mcps1.1.5.1.4 "><p id="p15671162103716"><a name="p15671162103716"></a><a name="p15671162103716"></a>-</p>
</td>
</tr>
<tr id="row6822734103716"><td class="cellrowborder" valign="top" width="19.39193919391939%" headers="mcps1.1.5.1.1 "><p id="p15770618103716"><a name="p15770618103716"></a><a name="p15770618103716"></a>mobile</p>
</td>
<td class="cellrowborder" valign="top" width="19.251925192519252%" headers="mcps1.1.5.1.2 "><p id="p2351649103716"><a name="p2351649103716"></a><a name="p2351649103716"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="26.662666266626662%" headers="mcps1.1.5.1.3 "><p id="p56265901103716"><a name="p56265901103716"></a><a name="p56265901103716"></a>接收短信的移动电话号码。</p>
</td>
<td class="cellrowborder" valign="top" width="34.69346934693469%" headers="mcps1.1.5.1.4 "><p id="p61244166103716"><a name="p61244166103716"></a><a name="p61244166103716"></a>-</p>
</td>
</tr>
<tr id="row14326587103716"><td class="cellrowborder" valign="top" width="19.39193919391939%" headers="mcps1.1.5.1.1 "><p id="p19602865103716"><a name="p19602865103716"></a><a name="p19602865103716"></a>submit_time</p>
</td>
<td class="cellrowborder" valign="top" width="19.251925192519252%" headers="mcps1.1.5.1.2 "><p id="p44328232103716"><a name="p44328232103716"></a><a name="p44328232103716"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="26.662666266626662%" headers="mcps1.1.5.1.3 "><p id="p33817031103716"><a name="p33817031103716"></a><a name="p33817031103716"></a>短信提交时间。</p>
</td>
<td class="cellrowborder" valign="top" width="34.69346934693469%" headers="mcps1.1.5.1.4 "><p id="p54825015103716"><a name="p54825015103716"></a><a name="p54825015103716"></a>-</p>
</td>
</tr>
<tr id="row23663093103716"><td class="cellrowborder" valign="top" width="19.39193919391939%" headers="mcps1.1.5.1.1 "><p id="p37662369103716"><a name="p37662369103716"></a><a name="p37662369103716"></a>deliver_time</p>
</td>
<td class="cellrowborder" valign="top" width="19.251925192519252%" headers="mcps1.1.5.1.2 "><p id="p30753009103716"><a name="p30753009103716"></a><a name="p30753009103716"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="26.662666266626662%" headers="mcps1.1.5.1.3 "><p id="p7965773103716"><a name="p7965773103716"></a><a name="p7965773103716"></a>短信送达时间。</p>
</td>
<td class="cellrowborder" valign="top" width="34.69346934693469%" headers="mcps1.1.5.1.4 "><p id="p41247902103716"><a name="p41247902103716"></a><a name="p41247902103716"></a>-</p>
</td>
</tr>
</tbody>
</table>

