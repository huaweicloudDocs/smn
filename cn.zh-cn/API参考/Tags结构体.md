# Tags结构体<a name="ZH-CN_TOPIC_0106008078"></a>

<a name="table12385184281216"></a>
<table><thead align="left"><tr id="row12526442141213"><th class="cellrowborder" valign="top" width="13%" id="mcps1.1.6.1.1"><p id="p1252612428129"><a name="p1252612428129"></a><a name="p1252612428129"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17%" id="mcps1.1.6.1.2"><p id="p852612421125"><a name="p852612421125"></a><a name="p852612421125"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15%" id="mcps1.1.6.1.3"><p id="p14526542121214"><a name="p14526542121214"></a><a name="p14526542121214"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="14.000000000000002%" id="mcps1.1.6.1.4"><p id="p17526124281215"><a name="p17526124281215"></a><a name="p17526124281215"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="41%" id="mcps1.1.6.1.5"><p id="p12294162622414"><a name="p12294162622414"></a><a name="p12294162622414"></a>约束</p>
</th>
</tr>
</thead>
<tbody><tr id="row1526194218129"><td class="cellrowborder" valign="top" width="13%" headers="mcps1.1.6.1.1 "><p id="p65262427126"><a name="p65262427126"></a><a name="p65262427126"></a>key</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.6.1.2 "><p id="p4526154211123"><a name="p4526154211123"></a><a name="p4526154211123"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.3 "><p id="p35261242171216"><a name="p35261242171216"></a><a name="p35261242171216"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.1.6.1.4 "><p id="p552604213129"><a name="p552604213129"></a><a name="p552604213129"></a>键</p>
</td>
<td class="cellrowborder" valign="top" width="41%" headers="mcps1.1.6.1.5 "><p id="p6294172612244"><a name="p6294172612244"></a><a name="p6294172612244"></a>最大长度127个unicode字符。 key不能为空。</p>
</td>
</tr>
<tr id="row55261142141216"><td class="cellrowborder" valign="top" width="13%" headers="mcps1.1.6.1.1 "><p id="p1852614219127"><a name="p1852614219127"></a><a name="p1852614219127"></a>values</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.6.1.2 "><p id="p11526104271211"><a name="p11526104271211"></a><a name="p11526104271211"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.6.1.3 "><p id="p45262426129"><a name="p45262426129"></a><a name="p45262426129"></a>String列表</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.1.6.1.4 "><p id="p152694220126"><a name="p152694220126"></a><a name="p152694220126"></a>值列表</p>
</td>
<td class="cellrowborder" valign="top" width="41%" headers="mcps1.1.6.1.5 "><p id="p18294152612244"><a name="p18294152612244"></a><a name="p18294152612244"></a>每个值最大长度255个unicode字符， *为系统保留字符，如果里面的value是以*开头，表示按照*后面的值全模糊匹配。values字段不能缺失，但是可以为空列表，空列表情况下，表示任何值。value之间为或的关系。</p>
</td>
</tr>
</tbody>
</table>

