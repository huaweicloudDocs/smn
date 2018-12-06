# HTTP\(S\)消息格式<a name="ZH-CN_TOPIC_0044402394"></a>

## 操作场景<a name="section32651219144241"></a>

描述SMN服务向HTTP\(S\)终端发送消息的格式，您可以通过消息类型区分消息。消息包括HTTP头部信息与HTTP Content部分。Content部分是JSON格式的字符串。

## HTTP\(S\)消息头部信息<a name="section46201434144241"></a>

当SMN服务向HTTP\(S\)终端发送消息时，头部包括请求X-SMN-TOPIC-URN，X-SMN-MESSAGE-ID，X-SMN-MESSAGE-TYPE，X-SMN-SUBSCRIPTION-URN，如[表1](#table59304739144241)所示。

**表 1**  消息HTTP头部参数说明

<a name="table59304739144241"></a>
<table><thead align="left"><tr id="row30468244144241"><th class="cellrowborder" valign="top" width="45.15%" id="mcps1.2.3.1.1"><p id="p52008685144241"><a name="p52008685144241"></a><a name="p52008685144241"></a><strong id="b17331199153917"><a name="b17331199153917"></a><a name="b17331199153917"></a>参数</strong></p>
</th>
<th class="cellrowborder" valign="top" width="54.85%" id="mcps1.2.3.1.2"><p id="p51953955144241"><a name="p51953955144241"></a><a name="p51953955144241"></a><strong id="b61649860153917"><a name="b61649860153917"></a><a name="b61649860153917"></a>说明</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="row47520797144241"><td class="cellrowborder" valign="top" width="45.15%" headers="mcps1.2.3.1.1 "><p id="p23979331144241"><a name="p23979331144241"></a><a name="p23979331144241"></a>X-SMN-MESSAGE-TYPE</p>
</td>
<td class="cellrowborder" valign="top" width="54.85%" headers="mcps1.2.3.1.2 "><p id="p63277695144241"><a name="p63277695144241"></a><a name="p63277695144241"></a>消息类型，消息类型分别有：</p>
<a name="ul32628343144241"></a><a name="ul32628343144241"></a><ul id="ul32628343144241"><li>SubscriptionConfirmation</li><li>Notification</li><li>UnsubscribeConfirmation</li></ul>
</td>
</tr>
<tr id="row64396778144241"><td class="cellrowborder" valign="top" width="45.15%" headers="mcps1.2.3.1.1 "><p id="p48756504144241"><a name="p48756504144241"></a><a name="p48756504144241"></a>X-SMN-MESSAGE-ID</p>
</td>
<td class="cellrowborder" valign="top" width="54.85%" headers="mcps1.2.3.1.2 "><p id="p56962718144241"><a name="p56962718144241"></a><a name="p56962718144241"></a>消息唯一标识</p>
</td>
</tr>
<tr id="row42902418144241"><td class="cellrowborder" valign="top" width="45.15%" headers="mcps1.2.3.1.1 "><p id="p52543824144241"><a name="p52543824144241"></a><a name="p52543824144241"></a>X-SMN-TOPIC-URN</p>
</td>
<td class="cellrowborder" valign="top" width="54.85%" headers="mcps1.2.3.1.2 "><p id="p28191355144241"><a name="p28191355144241"></a><a name="p28191355144241"></a>主题的唯一标识，表示消息归属的主题</p>
</td>
</tr>
<tr id="row52395604144241"><td class="cellrowborder" valign="top" width="45.15%" headers="mcps1.2.3.1.1 "><p id="p16185549144241"><a name="p16185549144241"></a><a name="p16185549144241"></a>X-SMN-SUBSCRIPTION-URN</p>
</td>
<td class="cellrowborder" valign="top" width="54.85%" headers="mcps1.2.3.1.2 "><p id="p35961062144241"><a name="p35961062144241"></a><a name="p35961062144241"></a>订阅终端的唯一标识</p>
</td>
</tr>
</tbody>
</table>

## HTTP\(S\)订阅确认消息的格式<a name="section55214102144241"></a>

添加HTTP\(S\)订阅终端以后，SMN会向订阅终端推送一条订阅确认的消息，下面将描述消息的HTTP Content，它是JSON格式的字符串，其中包括subscribe\_url值，订阅确认需要GET请求subscribe\_url地址进行确认，具体JSON 字段说明如[表2](#table52870937144241)所示。

**表 2**  HTTP\(S\)订阅确认消息的格式参数说明

<a name="table52870937144241"></a>
<table><thead align="left"><tr id="row40646338144241"><th class="cellrowborder" valign="top" width="30.3%" id="mcps1.2.3.1.1"><p id="p4019045144241"><a name="p4019045144241"></a><a name="p4019045144241"></a><strong id="b982317815399"><a name="b982317815399"></a><a name="b982317815399"></a>参数</strong></p>
</th>
<th class="cellrowborder" valign="top" width="69.69999999999999%" id="mcps1.2.3.1.2"><p id="p57107266144241"><a name="p57107266144241"></a><a name="p57107266144241"></a><strong id="b5747991715399"><a name="b5747991715399"></a><a name="b5747991715399"></a>说明</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="row62285823144241"><td class="cellrowborder" valign="top" width="30.3%" headers="mcps1.2.3.1.1 "><p id="p11986884144241"><a name="p11986884144241"></a><a name="p11986884144241"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="69.69999999999999%" headers="mcps1.2.3.1.2 "><p id="p31413562144241"><a name="p31413562144241"></a><a name="p31413562144241"></a>消息类型，SubscriptionConfirmation</p>
</td>
</tr>
<tr id="row14286607144241"><td class="cellrowborder" valign="top" width="30.3%" headers="mcps1.2.3.1.1 "><p id="p16364496144241"><a name="p16364496144241"></a><a name="p16364496144241"></a>subscribe_url</p>
</td>
<td class="cellrowborder" valign="top" width="69.69999999999999%" headers="mcps1.2.3.1.2 "><p id="p50455831144241"><a name="p50455831144241"></a><a name="p50455831144241"></a>订阅确认需要访问的URL</p>
</td>
</tr>
<tr id="row51449295144241"><td class="cellrowborder" valign="top" width="30.3%" headers="mcps1.2.3.1.1 "><p id="p6643351144241"><a name="p6643351144241"></a><a name="p6643351144241"></a>topic_urn</p>
</td>
<td class="cellrowborder" valign="top" width="69.69999999999999%" headers="mcps1.2.3.1.2 "><p id="p1240535144241"><a name="p1240535144241"></a><a name="p1240535144241"></a>主题的唯一标识，表示消息归属的主题</p>
</td>
</tr>
<tr id="row11164820144241"><td class="cellrowborder" valign="top" width="30.3%" headers="mcps1.2.3.1.1 "><p id="p31935228144241"><a name="p31935228144241"></a><a name="p31935228144241"></a>message_id</p>
</td>
<td class="cellrowborder" valign="top" width="69.69999999999999%" headers="mcps1.2.3.1.2 "><p id="p36616689144241"><a name="p36616689144241"></a><a name="p36616689144241"></a>消息唯一标识</p>
</td>
</tr>
<tr id="row61114747144241"><td class="cellrowborder" valign="top" width="30.3%" headers="mcps1.2.3.1.1 "><p id="p51347502144241"><a name="p51347502144241"></a><a name="p51347502144241"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="69.69999999999999%" headers="mcps1.2.3.1.2 "><p id="p65506977144241"><a name="p65506977144241"></a><a name="p65506977144241"></a>订阅确认消息的描述</p>
</td>
</tr>
<tr id="row52691882144241"><td class="cellrowborder" valign="top" width="30.3%" headers="mcps1.2.3.1.1 "><p id="p40184032144241"><a name="p40184032144241"></a><a name="p40184032144241"></a>signature</p>
</td>
<td class="cellrowborder" valign="top" width="69.69999999999999%" headers="mcps1.2.3.1.2 "><p id="p33681196144241"><a name="p33681196144241"></a><a name="p33681196144241"></a>签名信息</p>
<p id="p34695308144241"><a name="p34695308144241"></a><a name="p34695308144241"></a>签名字段包括message，message_id，subscribe_url，timestamp，topic_urn和type，具体签名信息校验，请参见<a href="校验消息签名.md">校验消息签名</a></p>
</td>
</tr>
<tr id="row43822323144241"><td class="cellrowborder" valign="top" width="30.3%" headers="mcps1.2.3.1.1 "><p id="p59947295144241"><a name="p59947295144241"></a><a name="p59947295144241"></a>signature_version</p>
</td>
<td class="cellrowborder" valign="top" width="69.69999999999999%" headers="mcps1.2.3.1.2 "><p id="p23892760144241"><a name="p23892760144241"></a><a name="p23892760144241"></a>签名的版本信息，目前是V1</p>
</td>
</tr>
<tr id="row13708253144241"><td class="cellrowborder" valign="top" width="30.3%" headers="mcps1.2.3.1.1 "><p id="p36626675144241"><a name="p36626675144241"></a><a name="p36626675144241"></a>signing_cert_url</p>
</td>
<td class="cellrowborder" valign="top" width="69.69999999999999%" headers="mcps1.2.3.1.2 "><p id="p13970698144241"><a name="p13970698144241"></a><a name="p13970698144241"></a>用于消息签名的证书URL</p>
</td>
</tr>
<tr id="row58627421144241"><td class="cellrowborder" valign="top" width="30.3%" headers="mcps1.2.3.1.1 "><p id="p51200664144241"><a name="p51200664144241"></a><a name="p51200664144241"></a>timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="69.69999999999999%" headers="mcps1.2.3.1.2 "><p id="p53613095144241"><a name="p53613095144241"></a><a name="p53613095144241"></a>消息第一次发送的时间戳</p>
</td>
</tr>
</tbody>
</table>

## HTTP\(S\)推送消息的格式<a name="section12755810144241"></a>

HTTP\(S\)订阅终端订阅确认后，终端将收到SMN推送的消息，下面将描述HTTP Content信息，它是JSON串，具体字段说明如[表3](#table37962339144241)所示。

**表 3**  HTTP\(S\)推送消息的格式参数说明

<a name="table37962339144241"></a>
<table><thead align="left"><tr id="row7026846144241"><th class="cellrowborder" valign="top" width="30.3%" id="mcps1.2.3.1.1"><p id="p32303664144241"><a name="p32303664144241"></a><a name="p32303664144241"></a><strong id="b1201045415393"><a name="b1201045415393"></a><a name="b1201045415393"></a>参数</strong></p>
</th>
<th class="cellrowborder" valign="top" width="69.69999999999999%" id="mcps1.2.3.1.2"><p id="p66460015144241"><a name="p66460015144241"></a><a name="p66460015144241"></a><strong id="b3332270615393"><a name="b3332270615393"></a><a name="b3332270615393"></a>说明</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="row14552130144241"><td class="cellrowborder" valign="top" width="30.3%" headers="mcps1.2.3.1.1 "><p id="p37871890144241"><a name="p37871890144241"></a><a name="p37871890144241"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="69.69999999999999%" headers="mcps1.2.3.1.2 "><p id="p47724230144241"><a name="p47724230144241"></a><a name="p47724230144241"></a>消息类型，Notification</p>
</td>
</tr>
<tr id="row26864889144241"><td class="cellrowborder" valign="top" width="30.3%" headers="mcps1.2.3.1.1 "><p id="p28572415144241"><a name="p28572415144241"></a><a name="p28572415144241"></a>topic_urn</p>
</td>
<td class="cellrowborder" valign="top" width="69.69999999999999%" headers="mcps1.2.3.1.2 "><p id="p32664285144241"><a name="p32664285144241"></a><a name="p32664285144241"></a>主题的唯一标识，表示消息归属的主题</p>
</td>
</tr>
<tr id="row25543117144241"><td class="cellrowborder" valign="top" width="30.3%" headers="mcps1.2.3.1.1 "><p id="p55726628144241"><a name="p55726628144241"></a><a name="p55726628144241"></a>message_id</p>
</td>
<td class="cellrowborder" valign="top" width="69.69999999999999%" headers="mcps1.2.3.1.2 "><p id="p17562982144241"><a name="p17562982144241"></a><a name="p17562982144241"></a>消息唯一标识</p>
</td>
</tr>
<tr id="row23849116144241"><td class="cellrowborder" valign="top" width="30.3%" headers="mcps1.2.3.1.1 "><p id="p52730220144241"><a name="p52730220144241"></a><a name="p52730220144241"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="69.69999999999999%" headers="mcps1.2.3.1.2 "><p id="p43289437144241"><a name="p43289437144241"></a><a name="p43289437144241"></a>订阅推送消息的描述</p>
</td>
</tr>
<tr id="row54060617144241"><td class="cellrowborder" valign="top" width="30.3%" headers="mcps1.2.3.1.1 "><p id="p16833870144241"><a name="p16833870144241"></a><a name="p16833870144241"></a>unsubscribe_url</p>
</td>
<td class="cellrowborder" valign="top" width="69.69999999999999%" headers="mcps1.2.3.1.2 "><p id="p21366215144241"><a name="p21366215144241"></a><a name="p21366215144241"></a>通过访问该链接可以取消终端订阅</p>
</td>
</tr>
<tr id="row58078211144241"><td class="cellrowborder" valign="top" width="30.3%" headers="mcps1.2.3.1.1 "><p id="p6714630144241"><a name="p6714630144241"></a><a name="p6714630144241"></a>signature</p>
</td>
<td class="cellrowborder" valign="top" width="69.69999999999999%" headers="mcps1.2.3.1.2 "><p id="p7014129144241"><a name="p7014129144241"></a><a name="p7014129144241"></a>签名信息</p>
<p id="p63127165144241"><a name="p63127165144241"></a><a name="p63127165144241"></a>签名字段包括message，message_id，subject， timestamp，topic_urn和type,具体签名信息校验，如果subject不存在，则不参与校验，请参见<a href="校验消息签名.md">校验消息签名</a></p>
</td>
</tr>
<tr id="row1873911211287"><td class="cellrowborder" valign="top" width="30.3%" headers="mcps1.2.3.1.1 "><p id="p9739111242810"><a name="p9739111242810"></a><a name="p9739111242810"></a>subject</p>
</td>
<td class="cellrowborder" valign="top" width="69.69999999999999%" headers="mcps1.2.3.1.2 "><p id="p16739912122814"><a name="p16739912122814"></a><a name="p16739912122814"></a>消息标题</p>
</td>
</tr>
<tr id="row31273581144241"><td class="cellrowborder" valign="top" width="30.3%" headers="mcps1.2.3.1.1 "><p id="p50132129144241"><a name="p50132129144241"></a><a name="p50132129144241"></a>signature_version</p>
</td>
<td class="cellrowborder" valign="top" width="69.69999999999999%" headers="mcps1.2.3.1.2 "><p id="p34170678144241"><a name="p34170678144241"></a><a name="p34170678144241"></a>签名的版本信息，目前是V1</p>
</td>
</tr>
<tr id="row39100652144241"><td class="cellrowborder" valign="top" width="30.3%" headers="mcps1.2.3.1.1 "><p id="p13036277144241"><a name="p13036277144241"></a><a name="p13036277144241"></a>signing_cert_url</p>
</td>
<td class="cellrowborder" valign="top" width="69.69999999999999%" headers="mcps1.2.3.1.2 "><p id="p49305522144241"><a name="p49305522144241"></a><a name="p49305522144241"></a>用于消息签名的证书URL</p>
</td>
</tr>
<tr id="row41096520144241"><td class="cellrowborder" valign="top" width="30.3%" headers="mcps1.2.3.1.1 "><p id="p40483823144241"><a name="p40483823144241"></a><a name="p40483823144241"></a>timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="69.69999999999999%" headers="mcps1.2.3.1.2 "><p id="p57964222144241"><a name="p57964222144241"></a><a name="p57964222144241"></a>消息第一次发送的时间戳</p>
</td>
</tr>
</tbody>
</table>

## HTTP\(S\)取消订阅消息的格式<a name="section51915957144241"></a>

HTTP\(S\)订阅终端取消订阅确认后，终端将收到SMN推送的取消订阅确认消息，下面将描述HTTP Content信息，它是JSON串，具体字段说明如[表4](#table64442359144241)所示。

**表 4**  HTTP\(S\)取消订阅消息的格式参数说明

<a name="table64442359144241"></a>
<table><thead align="left"><tr id="row47856547144241"><th class="cellrowborder" valign="top" width="30.3%" id="mcps1.2.3.1.1"><p id="p51175085144241"><a name="p51175085144241"></a><a name="p51175085144241"></a><strong id="b44234363153857"><a name="b44234363153857"></a><a name="b44234363153857"></a>参数</strong></p>
</th>
<th class="cellrowborder" valign="top" width="69.69999999999999%" id="mcps1.2.3.1.2"><p id="p51541240144241"><a name="p51541240144241"></a><a name="p51541240144241"></a><strong id="b26213628153857"><a name="b26213628153857"></a><a name="b26213628153857"></a>说明</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="row14090924144241"><td class="cellrowborder" valign="top" width="30.3%" headers="mcps1.2.3.1.1 "><p id="p514159144241"><a name="p514159144241"></a><a name="p514159144241"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="69.69999999999999%" headers="mcps1.2.3.1.2 "><p id="p41646956144241"><a name="p41646956144241"></a><a name="p41646956144241"></a>消息类型，UnsubscribeConfirmation</p>
</td>
</tr>
<tr id="row39278287144241"><td class="cellrowborder" valign="top" width="30.3%" headers="mcps1.2.3.1.1 "><p id="p27424659144241"><a name="p27424659144241"></a><a name="p27424659144241"></a>subscribe_url</p>
</td>
<td class="cellrowborder" valign="top" width="69.69999999999999%" headers="mcps1.2.3.1.2 "><p id="p6804900144241"><a name="p6804900144241"></a><a name="p6804900144241"></a>再次订阅确认需要访问的URL</p>
</td>
</tr>
<tr id="row61244100144241"><td class="cellrowborder" valign="top" width="30.3%" headers="mcps1.2.3.1.1 "><p id="p61825074144241"><a name="p61825074144241"></a><a name="p61825074144241"></a>topic_urn</p>
</td>
<td class="cellrowborder" valign="top" width="69.69999999999999%" headers="mcps1.2.3.1.2 "><p id="p41775137144241"><a name="p41775137144241"></a><a name="p41775137144241"></a>主题的唯一标识，表示消息归属的主题</p>
</td>
</tr>
<tr id="row40431921144241"><td class="cellrowborder" valign="top" width="30.3%" headers="mcps1.2.3.1.1 "><p id="p53760131144241"><a name="p53760131144241"></a><a name="p53760131144241"></a>message_id</p>
</td>
<td class="cellrowborder" valign="top" width="69.69999999999999%" headers="mcps1.2.3.1.2 "><p id="p59603370144241"><a name="p59603370144241"></a><a name="p59603370144241"></a>消息唯一标识</p>
</td>
</tr>
<tr id="row66668289144241"><td class="cellrowborder" valign="top" width="30.3%" headers="mcps1.2.3.1.1 "><p id="p31422338144241"><a name="p31422338144241"></a><a name="p31422338144241"></a>message</p>
</td>
<td class="cellrowborder" valign="top" width="69.69999999999999%" headers="mcps1.2.3.1.2 "><p id="p62181451144241"><a name="p62181451144241"></a><a name="p62181451144241"></a>取消订阅确认消息的描述</p>
</td>
</tr>
<tr id="row22762155144241"><td class="cellrowborder" valign="top" width="30.3%" headers="mcps1.2.3.1.1 "><p id="p31795252144241"><a name="p31795252144241"></a><a name="p31795252144241"></a>signature</p>
</td>
<td class="cellrowborder" valign="top" width="69.69999999999999%" headers="mcps1.2.3.1.2 "><p id="p25278618144241"><a name="p25278618144241"></a><a name="p25278618144241"></a>签名信息</p>
<p id="p26180971144241"><a name="p26180971144241"></a><a name="p26180971144241"></a>签名字段包括message，message_id，subscribe_url、timestamp，topic_urn和type,具体签名信息校验，请参见<a href="校验消息签名.md">校验消息签名</a></p>
</td>
</tr>
<tr id="row34302148144241"><td class="cellrowborder" valign="top" width="30.3%" headers="mcps1.2.3.1.1 "><p id="p27010586144241"><a name="p27010586144241"></a><a name="p27010586144241"></a>signature_version</p>
</td>
<td class="cellrowborder" valign="top" width="69.69999999999999%" headers="mcps1.2.3.1.2 "><p id="p40373894144241"><a name="p40373894144241"></a><a name="p40373894144241"></a>签名的版本信息，目前是V1</p>
</td>
</tr>
<tr id="row27820726144241"><td class="cellrowborder" valign="top" width="30.3%" headers="mcps1.2.3.1.1 "><p id="p38886363144241"><a name="p38886363144241"></a><a name="p38886363144241"></a>signing_cert_url</p>
</td>
<td class="cellrowborder" valign="top" width="69.69999999999999%" headers="mcps1.2.3.1.2 "><p id="p62787721144241"><a name="p62787721144241"></a><a name="p62787721144241"></a>用于消息签名的证书URL</p>
</td>
</tr>
<tr id="row28218578144241"><td class="cellrowborder" valign="top" width="30.3%" headers="mcps1.2.3.1.1 "><p id="p4003487144241"><a name="p4003487144241"></a><a name="p4003487144241"></a>timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="69.69999999999999%" headers="mcps1.2.3.1.2 "><p id="p55847049144241"><a name="p55847049144241"></a><a name="p55847049144241"></a>消息第一次发送的时间戳</p>
</td>
</tr>
</tbody>
</table>

