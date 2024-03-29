# API概览<a name="smn_api_20000"></a>

通过使用消息通知服务所提供的接口，您可以完整的使用消息通知服务的所有功能。例如创建Topic、添加订阅。

**表 1**  接口说明

<a name="table5876102613294"></a>
<table><thead align="left"><tr id="row3878122616298"><th class="cellrowborder" valign="top" width="23.86%" id="mcps1.2.3.1.1"><p id="p68781126182914"><a name="p68781126182914"></a><a name="p68781126182914"></a><strong id="b125201844173712"><a name="b125201844173712"></a><a name="b125201844173712"></a>类型</strong></p>
</th>
<th class="cellrowborder" valign="top" width="76.14%" id="mcps1.2.3.1.2"><p id="p158781726112914"><a name="p158781726112914"></a><a name="p158781726112914"></a><strong id="b15203449370"><a name="b15203449370"></a><a name="b15203449370"></a>说明</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="row148781026122919"><td class="cellrowborder" valign="top" width="23.86%" headers="mcps1.2.3.1.1 "><p id="p14287143404415"><a name="p14287143404415"></a><a name="p14287143404415"></a>Topic操作</p>
</td>
<td class="cellrowborder" valign="top" width="76.14%" headers="mcps1.2.3.1.2 "><p id="p56591328178"><a name="p56591328178"></a><a name="p56591328178"></a>包含创建Topic、更新Topic、删除Topic等接口。</p>
</td>
</tr>
<tr id="row1987820263297"><td class="cellrowborder" valign="top" width="23.86%" headers="mcps1.2.3.1.1 "><p id="p8939172693215"><a name="p8939172693215"></a><a name="p8939172693215"></a>订阅操作</p>
</td>
<td class="cellrowborder" valign="top" width="76.14%" headers="mcps1.2.3.1.2 "><p id="p86434284717"><a name="p86434284717"></a><a name="p86434284717"></a>包含查询订阅列表、订阅、取消订阅等接口。</p>
</td>
</tr>
<tr id="row87746166614"><td class="cellrowborder" valign="top" width="23.86%" headers="mcps1.2.3.1.1 "><p id="p197741716567"><a name="p197741716567"></a><a name="p197741716567"></a>模板操作</p>
</td>
<td class="cellrowborder" valign="top" width="76.14%" headers="mcps1.2.3.1.2 "><p id="p1477491610610"><a name="p1477491610610"></a><a name="p1477491610610"></a>包含创建消息模板、更新消息模板、删除消息模板等接口。</p>
</td>
</tr>
<tr id="row816313459617"><td class="cellrowborder" valign="top" width="23.86%" headers="mcps1.2.3.1.1 "><p id="p1216317451267"><a name="p1216317451267"></a><a name="p1216317451267"></a>消息发布</p>
</td>
<td class="cellrowborder" valign="top" width="76.14%" headers="mcps1.2.3.1.2 "><p id="p18775185318516"><a name="p18775185318516"></a><a name="p18775185318516"></a>包含消息发布、使用消息结构体方式的消息发布和使用消息模板方式的消息发布接口。</p>
</td>
</tr>
<tr id="row9878726192911"><td class="cellrowborder" valign="top" width="23.86%" headers="mcps1.2.3.1.1 "><p id="p16101194212247"><a name="p16101194212247"></a><a name="p16101194212247"></a>使用标签管理服务</p>
</td>
<td class="cellrowborder" valign="top" width="76.14%" headers="mcps1.2.3.1.2 "><p id="p14101184217244"><a name="p14101184217244"></a><a name="p14101184217244"></a>包含查询资源实例、添加资源标签和查询项目标签等接口。</p>
</td>
</tr>
<tr id="row128488411202"><td class="cellrowborder" valign="top" width="23.86%" headers="mcps1.2.3.1.1 "><p id="p83642497201"><a name="p83642497201"></a><a name="p83642497201"></a>查询版本操作</p>
</td>
<td class="cellrowborder" valign="top" width="76.14%" headers="mcps1.2.3.1.2 "><p id="p1638084912207"><a name="p1638084912207"></a><a name="p1638084912207"></a>包含查询SMN支持的API版本号信息和查询SMN API V2版本信息接口。</p>
</td>
</tr>
<tr id="row9878172662914"><td class="cellrowborder" valign="top" width="23.86%" headers="mcps1.2.3.1.1 "><p id="p1435451910453"><a name="p1435451910453"></a><a name="p1435451910453"></a>Application操作</p>
</td>
<td class="cellrowborder" valign="top" width="76.14%" headers="mcps1.2.3.1.2 "><p id="p20353333105515"><a name="p20353333105515"></a><a name="p20353333105515"></a>包含创建Application、更新Application和删除Application等接口。</p>
</td>
</tr>
<tr id="row117351143103220"><td class="cellrowborder" valign="top" width="23.86%" headers="mcps1.2.3.1.1 "><p id="p1459204410473"><a name="p1459204410473"></a><a name="p1459204410473"></a>Application endpoint操作</p>
</td>
<td class="cellrowborder" valign="top" width="76.14%" headers="mcps1.2.3.1.2 "><p id="p73531233135516"><a name="p73531233135516"></a><a name="p73531233135516"></a>包含创建Application endpoint、更新Application endpoint和删除Application endpoint等接口。</p>
</td>
</tr>
<tr id="row11736144363213"><td class="cellrowborder" valign="top" width="23.86%" headers="mcps1.2.3.1.1 "><p id="p51011542102411"><a name="p51011542102411"></a><a name="p51011542102411"></a>Application直发消息操作</p>
</td>
<td class="cellrowborder" valign="top" width="76.14%" headers="mcps1.2.3.1.2 "><p id="p1135373315512"><a name="p1135373315512"></a><a name="p1135373315512"></a>包含APP消息发布和使用消息结构体方式的App消息发布接口。</p>
</td>
</tr>
</tbody>
</table>

