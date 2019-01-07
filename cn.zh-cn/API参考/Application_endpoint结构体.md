# Application\_endpoint结构体<a name="ZH-CN_TOPIC_0118716353"></a>

<a name="table219819244718"></a>
<table><thead align="left"><tr id="row1526011204718"><th class="cellrowborder" valign="top" width="23.232323232323235%" id="mcps1.1.5.1.1"><p id="p182602274711"><a name="p182602274711"></a><a name="p182602274711"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.171717171717173%" id="mcps1.1.5.1.2"><p id="p19260192154719"><a name="p19260192154719"></a><a name="p19260192154719"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="27.272727272727277%" id="mcps1.1.5.1.3"><p id="p126017204718"><a name="p126017204718"></a><a name="p126017204718"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="32.323232323232325%" id="mcps1.1.5.1.4"><p id="p16260132194713"><a name="p16260132194713"></a><a name="p16260132194713"></a>约束</p>
</th>
</tr>
</thead>
<tbody><tr id="row15260132164715"><td class="cellrowborder" valign="top" width="23.232323232323235%" headers="mcps1.1.5.1.1 "><p id="p326014254720"><a name="p326014254720"></a><a name="p326014254720"></a>create_time</p>
</td>
<td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.2 "><p id="p426010254715"><a name="p426010254715"></a><a name="p426010254715"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="27.272727272727277%" headers="mcps1.1.5.1.3 "><p id="p1926072174714"><a name="p1926072174714"></a><a name="p1926072174714"></a>创建application的时间</p>
</td>
<td class="cellrowborder" valign="top" width="32.323232323232325%" headers="mcps1.1.5.1.4 "><p id="p122602023472"><a name="p122602023472"></a><a name="p122602023472"></a>-</p>
</td>
</tr>
<tr id="row926062154712"><td class="cellrowborder" valign="top" width="23.232323232323235%" headers="mcps1.1.5.1.1 "><p id="p4260627473"><a name="p4260627473"></a><a name="p4260627473"></a>endpoint_urn</p>
</td>
<td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.2 "><p id="p132600210471"><a name="p132600210471"></a><a name="p132600210471"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="27.272727272727277%" headers="mcps1.1.5.1.3 "><p id="p102601428470"><a name="p102601428470"></a><a name="p102601428470"></a>Application endpoint的唯一资源标示</p>
</td>
<td class="cellrowborder" valign="top" width="32.323232323232325%" headers="mcps1.1.5.1.4 "><p id="p122606234717"><a name="p122606234717"></a><a name="p122606234717"></a>-</p>
</td>
</tr>
<tr id="row2026012218470"><td class="cellrowborder" valign="top" width="23.232323232323235%" headers="mcps1.1.5.1.1 "><p id="p1026016213472"><a name="p1026016213472"></a><a name="p1026016213472"></a>user_data</p>
</td>
<td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.2 "><p id="p026072164713"><a name="p026072164713"></a><a name="p026072164713"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="27.272727272727277%" headers="mcps1.1.5.1.3 "><p id="p3260102154711"><a name="p3260102154711"></a><a name="p3260102154711"></a>用户自定义数据</p>
</td>
<td class="cellrowborder" valign="top" width="32.323232323232325%" headers="mcps1.1.5.1.4 "><p id="p142609264710"><a name="p142609264710"></a><a name="p142609264710"></a>最大长度支持UTF-8编码后2048字节</p>
</td>
</tr>
<tr id="row426020218474"><td class="cellrowborder" valign="top" width="23.232323232323235%" headers="mcps1.1.5.1.1 "><p id="p7260152204714"><a name="p7260152204714"></a><a name="p7260152204714"></a>enabled</p>
</td>
<td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.2 "><p id="p182601124471"><a name="p182601124471"></a><a name="p182601124471"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="27.272727272727277%" headers="mcps1.1.5.1.3 "><p id="p17260102184712"><a name="p17260102184712"></a><a name="p17260102184712"></a>endpoint启用开关</p>
</td>
<td class="cellrowborder" valign="top" width="32.323232323232325%" headers="mcps1.1.5.1.4 "><p id="p22601227479"><a name="p22601227479"></a><a name="p22601227479"></a>true或false字符串</p>
</td>
</tr>
<tr id="row52603214715"><td class="cellrowborder" valign="top" width="23.232323232323235%" headers="mcps1.1.5.1.1 "><p id="p12604220478"><a name="p12604220478"></a><a name="p12604220478"></a>token</p>
</td>
<td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.2 "><p id="p1426012124719"><a name="p1426012124719"></a><a name="p1426012124719"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="27.272727272727277%" headers="mcps1.1.5.1.3 "><p id="p92605210470"><a name="p92605210470"></a><a name="p92605210470"></a>设备token</p>
</td>
<td class="cellrowborder" valign="top" width="32.323232323232325%" headers="mcps1.1.5.1.4 "><p id="p1226022144720"><a name="p1226022144720"></a><a name="p1226022144720"></a>最大长度512个字节</p>
</td>
</tr>
</tbody>
</table>

