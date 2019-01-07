# application消息体格式<a name="ZH-CN_TOPIC_0119034074"></a>

**表 1**  application消息体格式

<a name="table330018303493"></a>
<table><thead align="left"><tr id="row1830043010494"><th class="cellrowborder" valign="top" width="18%" id="mcps1.2.4.1.1"><p id="p96605944916"><a name="p96605944916"></a><a name="p96605944916"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.2.4.1.2"><p id="p0661259124915"><a name="p0661259124915"></a><a name="p0661259124915"></a>样例</p>
</th>
<th class="cellrowborder" valign="top" width="42%" id="mcps1.2.4.1.3"><p id="p13003300491"><a name="p13003300491"></a><a name="p13003300491"></a>备注</p>
</th>
</tr>
</thead>
<tbody><tr id="row16300183010496"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.4.1.1 "><p id="p156695912494"><a name="p156695912494"></a><a name="p156695912494"></a>华为透传消息</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.4.1.2 "><p id="p966105954914"><a name="p966105954914"></a><a name="p966105954914"></a>"hps": {</p>
<p id="p1666459204910"><a name="p1666459204910"></a><a name="p1666459204910"></a>"msg" : {</p>
<p id="p146645910494"><a name="p146645910494"></a><a name="p146645910494"></a>"type" : 1,</p>
<p id="p166145974917"><a name="p166145974917"></a><a name="p166145974917"></a>"body" : {"key":"value"}</p>
<p id="p266125912494"><a name="p266125912494"></a><a name="p266125912494"></a>}</p>
<p id="p166659184910"><a name="p166659184910"></a><a name="p166659184910"></a>}</p>
</td>
<td class="cellrowborder" rowspan="2" valign="top" width="42%" headers="mcps1.2.4.1.3 "><p id="p224933318552"><a name="p224933318552"></a><a name="p224933318552"></a>body为用户自定义格式。</p>
<div class="note" id="note149582146569"><a name="note149582146569"></a><a name="note149582146569"></a><span class="notetitle"> 说明： </span><div class="notebody"><a name="ul1328752085611"></a><a name="ul1328752085611"></a><ul id="ul1328752085611"><li>推荐使用JSON格式，如样例所示</li><li>对于纯文本可以将body设置为字符串(采用UTF-8编码)</li><li>消息体最大2K<p id="p13856165714563"><a name="p13856165714563"></a><a name="p13856165714563"></a>详细的字段介绍及其使用请参见<a href="http://developer.huawei.com/consumer/cn/service/hms/catalog/huaweipush_agent.html?page=hmssdk_huaweipush_api_reference_agent_s2">华为推送平台</a>的接口定义。</p>
</li></ul>
</div></div>
<p id="p11300630194915"><a name="p11300630194915"></a><a name="p11300630194915"></a></p>
</td>
</tr>
<tr id="row113003307499"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p6661859114915"><a name="p6661859114915"></a><a name="p6661859114915"></a>华为系统通知栏消息</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p146610599491"><a name="p146610599491"></a><a name="p146610599491"></a>"hps": {</p>
<p id="p46610593494"><a name="p46610593494"></a><a name="p46610593494"></a>"msg": {</p>
<p id="p11661593493"><a name="p11661593493"></a><a name="p11661593493"></a>"type": 3,</p>
<p id="p1766659104912"><a name="p1766659104912"></a><a name="p1766659104912"></a>"body": {</p>
<p id="p1666159114920"><a name="p1666159114920"></a><a name="p1666159114920"></a>"content": "Push message content",</p>
<p id="p1966185918499"><a name="p1966185918499"></a><a name="p1966185918499"></a>"title": "Push message content"</p>
<p id="p266105924918"><a name="p266105924918"></a><a name="p266105924918"></a>},</p>
<p id="p76615994919"><a name="p76615994919"></a><a name="p76615994919"></a>"action": {</p>
<p id="p1066195912494"><a name="p1066195912494"></a><a name="p1066195912494"></a>"type": 1,</p>
<p id="p156685924920"><a name="p156685924920"></a><a name="p156685924920"></a>"param": {</p>
<p id="p1661459144919"><a name="p1661459144919"></a><a name="p1661459144919"></a>"intent":"#Intent;compo=com.rvr/.Activity;S.W=U;end"</p>
<p id="p966195944917"><a name="p966195944917"></a><a name="p966195944917"></a>}</p>
<p id="p5665593492"><a name="p5665593492"></a><a name="p5665593492"></a>}</p>
<p id="p1766175920497"><a name="p1766175920497"></a><a name="p1766175920497"></a>},</p>
<p id="p186605912490"><a name="p186605912490"></a><a name="p186605912490"></a>"ext": {</p>
<p id="p96625916498"><a name="p96625916498"></a><a name="p96625916498"></a>"biTag": "Trump",</p>
<p id="p136610597496"><a name="p136610597496"></a><a name="p136610597496"></a>"icon": "http://upload.w.org/00/150pxsvg.png"</p>
<p id="p066145912495"><a name="p066145912495"></a><a name="p066145912495"></a>}</p>
<p id="p666175964911"><a name="p666175964911"></a><a name="p666175964911"></a>}</p>
</td>
</tr>
<tr id="row34135184916"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.4.1.1 "><p id="p5661859104918"><a name="p5661859104918"></a><a name="p5661859104918"></a>苹果平台消息格式</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.4.1.2 "><p id="p26685915499"><a name="p26685915499"></a><a name="p26685915499"></a>{</p>
<p id="p1866155916498"><a name="p1866155916498"></a><a name="p1866155916498"></a>"aps": {</p>
<p id="p1266259154916"><a name="p1266259154916"></a><a name="p1266259154916"></a>"alert": "hello world"</p>
<p id="p1766359184910"><a name="p1766359184910"></a><a name="p1766359184910"></a>}</p>
<p id="p566259164913"><a name="p566259164913"></a><a name="p566259164913"></a>}</p>
</td>
<td class="cellrowborder" valign="top" width="42%" headers="mcps1.2.4.1.3 "><p id="p1737461618554"><a name="p1737461618554"></a><a name="p1737461618554"></a>消息体最大4K。</p>
<p id="p637431695512"><a name="p637431695512"></a><a name="p637431695512"></a>详细的字段介绍及其使用参见<a href="https://developer.apple.com/library/content/documentation/NetworkingInternet/Conceptual/RemoteNotificationsPG/PayloadKeyReference.html">苹果推送平台</a>的接口定义。</p>
</td>
</tr>
</tbody>
</table>

