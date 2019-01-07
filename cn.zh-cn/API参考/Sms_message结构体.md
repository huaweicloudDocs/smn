# Sms\_message结构体<a name="ZH-CN_TOPIC_0102842875"></a>

<a name="table920655716319"></a>
<table><thead align="left"><tr id="row5615067816319"><th class="cellrowborder" valign="top" width="13.131313131313133%" id="mcps1.1.6.1.1"><p id="p5191106116319"><a name="p5191106116319"></a><a name="p5191106116319"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.88888888888889%" id="mcps1.1.6.1.2"><p id="p4404643716319"><a name="p4404643716319"></a><a name="p4404643716319"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="18.28282828282828%" id="mcps1.1.6.1.3"><p id="p1099166216319"><a name="p1099166216319"></a><a name="p1099166216319"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="20.393939393939394%" id="mcps1.1.6.1.4"><p id="p1790939916319"><a name="p1790939916319"></a><a name="p1790939916319"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="30.303030303030305%" id="mcps1.1.6.1.5"><p id="p4137517616319"><a name="p4137517616319"></a><a name="p4137517616319"></a>约束</p>
</th>
</tr>
</thead>
<tbody><tr id="row6305495416319"><td class="cellrowborder" valign="top" width="13.131313131313133%" headers="mcps1.1.6.1.1 "><p id="p717763616319"><a name="p717763616319"></a><a name="p717763616319"></a>endpoint</p>
</td>
<td class="cellrowborder" valign="top" width="17.88888888888889%" headers="mcps1.1.6.1.2 "><p id="p4451766316319"><a name="p4451766316319"></a><a name="p4451766316319"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="18.28282828282828%" headers="mcps1.1.6.1.3 "><p id="p4916096316319"><a name="p4916096316319"></a><a name="p4916096316319"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="20.393939393939394%" headers="mcps1.1.6.1.4 "><p id="p278534415466"><a name="p278534415466"></a><a name="p278534415466"></a>手机号码</p>
</td>
<td class="cellrowborder" valign="top" width="30.303030303030305%" headers="mcps1.1.6.1.5 "><p id="p2482112016476"><a name="p2482112016476"></a><a name="p2482112016476"></a>终端节点必须是一个电话号码，国际号码必须以“+[国家码]”开头，国内号码可以省略“+”或“+[国家码]”。</p>
</td>
</tr>
<tr id="row17933345197"><td class="cellrowborder" valign="top" width="13.131313131313133%" headers="mcps1.1.6.1.1 "><p id="p6278699416319"><a name="p6278699416319"></a><a name="p6278699416319"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="17.88888888888889%" headers="mcps1.1.6.1.2 "><p id="p5258174716319"><a name="p5258174716319"></a><a name="p5258174716319"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="18.28282828282828%" headers="mcps1.1.6.1.3 "><p id="p3126308016319"><a name="p3126308016319"></a><a name="p3126308016319"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="20.393939393939394%" headers="mcps1.1.6.1.4 "><p id="p4928152916319"><a name="p4928152916319"></a><a name="p4928152916319"></a>消息内容</p>
</td>
<td class="cellrowborder" valign="top" width="30.303030303030305%" headers="mcps1.1.6.1.5 "><p id="p5602156133414"><a name="p5602156133414"></a><a name="p5602156133414"></a>长度不超过490个字符。如果传递sign_id参数，则message中不需要携带签名，系统会自动拼接签名信息于message头部。如果传递message_include_sign _flag参数，则message的签名信息由用户拼接。将签名放置于“【】”括号中，并添加到内容头部。例如：“【XX商城】您的验证码为123456，请尽快完成验证。”</p>
</td>
</tr>
<tr id="row158087791914"><td class="cellrowborder" valign="top" width="13.131313131313133%" headers="mcps1.1.6.1.1 "><p id="p43393709141623"><a name="p43393709141623"></a><a name="p43393709141623"></a>sign_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.88888888888889%" headers="mcps1.1.6.1.2 "><p id="p25229539141623"><a name="p25229539141623"></a><a name="p25229539141623"></a>当message_include_sign_flag参数不传递或为“false”时，此参数必选</p>
</td>
<td class="cellrowborder" valign="top" width="18.28282828282828%" headers="mcps1.1.6.1.3 "><p id="p30326749141623"><a name="p30326749141623"></a><a name="p30326749141623"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="20.393939393939394%" headers="mcps1.1.6.1.4 "><p id="p14312045155411"><a name="p14312045155411"></a><a name="p14312045155411"></a>签名ID</p>
<p id="p41902898141725"><a name="p41902898141725"></a><a name="p41902898141725"></a>短信签名ID在创建短信签名时由系统自动生成，是短信签名的唯一标识。请在SMN控制台左侧导航栏单击“短信”，在页面的短信签名列表中获取签名ID。</p>
</td>
<td class="cellrowborder" valign="top" width="30.303030303030305%" headers="mcps1.1.6.1.5 "><p id="p57930313141758"><a name="p57930313141758"></a><a name="p57930313141758"></a>-</p>
</td>
</tr>
<tr id="row2089181013199"><td class="cellrowborder" valign="top" width="13.131313131313133%" headers="mcps1.1.6.1.1 "><p id="p3274606558"><a name="p3274606558"></a><a name="p3274606558"></a>message_include_sign_flag</p>
</td>
<td class="cellrowborder" valign="top" width="17.88888888888889%" headers="mcps1.1.6.1.2 "><p id="p137416295564"><a name="p137416295564"></a><a name="p137416295564"></a>当sign_id参数不传递时，此参数必选且为“true”</p>
</td>
<td class="cellrowborder" valign="top" width="18.28282828282828%" headers="mcps1.1.6.1.3 "><p id="p1287154145411"><a name="p1287154145411"></a><a name="p1287154145411"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="20.393939393939394%" headers="mcps1.1.6.1.4 "><p id="p12795534162917"><a name="p12795534162917"></a><a name="p12795534162917"></a>如果您需要在message中自行拼接签名信息，请将此参数设置为"true"。</p>
</td>
<td class="cellrowborder" valign="top" width="30.303030303030305%" headers="mcps1.1.6.1.5 "><p id="p2080662075512"><a name="p2080662075512"></a><a name="p2080662075512"></a>"true" 或 "false"，不传参数则默认为"false"。</p>
</td>
</tr>
<tr id="row97861051104611"><td class="cellrowborder" valign="top" width="13.131313131313133%" headers="mcps1.1.6.1.1 "><p id="p1881735817461"><a name="p1881735817461"></a><a name="p1881735817461"></a>extend_src_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.88888888888889%" headers="mcps1.1.6.1.2 "><p id="p4817155813467"><a name="p4817155813467"></a><a name="p4817155813467"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.28282828282828%" headers="mcps1.1.6.1.3 "><p id="p481735816467"><a name="p481735816467"></a><a name="p481735816467"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="20.393939393939394%" headers="mcps1.1.6.1.4 "><p id="p19661123110282"><a name="p19661123110282"></a><a name="p19661123110282"></a>短信发送方号码的扩展号码</p>
</td>
<td class="cellrowborder" valign="top" width="30.303030303030305%" headers="mcps1.1.6.1.5 "><p id="p138173585469"><a name="p138173585469"></a><a name="p138173585469"></a>8位以内的数字。该字段仅限可自定义扩展号码的签名使用。</p>
</td>
</tr>
<tr id="row950216121519"><td class="cellrowborder" valign="top" width="13.131313131313133%" headers="mcps1.1.6.1.1 "><p id="p1350251212114"><a name="p1350251212114"></a><a name="p1350251212114"></a>extend_code</p>
</td>
<td class="cellrowborder" valign="top" width="17.88888888888889%" headers="mcps1.1.6.1.2 "><p id="p65039123115"><a name="p65039123115"></a><a name="p65039123115"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.28282828282828%" headers="mcps1.1.6.1.3 "><p id="p550341215116"><a name="p550341215116"></a><a name="p550341215116"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="20.393939393939394%" headers="mcps1.1.6.1.4 "><p id="p650317121919"><a name="p650317121919"></a><a name="p650317121919"></a>扩展字段，短信状态通知时，会返回该字段内容。</p>
</td>
<td class="cellrowborder" valign="top" width="30.303030303030305%" headers="mcps1.1.6.1.5 "><p id="p139121634751"><a name="p139121634751"></a><a name="p139121634751"></a>长度小于等于32个字节</p>
</td>
</tr>
</tbody>
</table>

