# Resource结构体<a name="ZH-CN_TOPIC_0106008080"></a>

<a name="table97917514177"></a>
<table><thead align="left"><tr id="row20931851161717"><th class="cellrowborder" valign="top" width="14.85148514851485%" id="mcps1.1.6.1.1"><p id="p169312051161713"><a name="p169312051161713"></a><a name="p169312051161713"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="11.881188118811881%" id="mcps1.1.6.1.2"><p id="p6931195111719"><a name="p6931195111719"></a><a name="p6931195111719"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="18.81188118811881%" id="mcps1.1.6.1.3"><p id="p093195116179"><a name="p093195116179"></a><a name="p093195116179"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="39.603960396039604%" id="mcps1.1.6.1.4"><p id="p59319515179"><a name="p59319515179"></a><a name="p59319515179"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="14.85148514851485%" id="mcps1.1.6.1.5"><p id="p835715919265"><a name="p835715919265"></a><a name="p835715919265"></a>约束</p>
</th>
</tr>
</thead>
<tbody><tr id="row393195119172"><td class="cellrowborder" valign="top" width="14.85148514851485%" headers="mcps1.1.6.1.1 "><p id="p1793165110171"><a name="p1793165110171"></a><a name="p1793165110171"></a>resource_id</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.1.6.1.2 "><p id="p6931185117179"><a name="p6931185117179"></a><a name="p6931185117179"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="18.81188118811881%" headers="mcps1.1.6.1.3 "><p id="p69311951191710"><a name="p69311951191710"></a><a name="p69311951191710"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="39.603960396039604%" headers="mcps1.1.6.1.4 "><p id="p1931175111170"><a name="p1931175111170"></a><a name="p1931175111170"></a>资源ID</p>
</td>
<td class="cellrowborder" valign="top" width="14.85148514851485%" headers="mcps1.1.6.1.5 "><p id="p8357199268"><a name="p8357199268"></a><a name="p8357199268"></a>-</p>
</td>
</tr>
<tr id="row493125112176"><td class="cellrowborder" valign="top" width="14.85148514851485%" headers="mcps1.1.6.1.1 "><p id="p2931165110176"><a name="p2931165110176"></a><a name="p2931165110176"></a>resource_detail</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.1.6.1.2 "><p id="p6931105151716"><a name="p6931105151716"></a><a name="p6931105151716"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="18.81188118811881%" headers="mcps1.1.6.1.3 "><p id="p293145151713"><a name="p293145151713"></a><a name="p293145151713"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="39.603960396039604%" headers="mcps1.1.6.1.4 "><p id="p1793113514176"><a name="p1793113514176"></a><a name="p1793113514176"></a>资源详情。 资源对象，用于扩展。默认为空。</p>
<p id="p826215381712"><a name="p826215381712"></a><a name="p826215381712"></a>对于topic资源类型，该字段内容为{"topic_urn":"${TopicUrn}","display_name":"display name"}；</p>
<p id="p1226217381177"><a name="p1226217381177"></a><a name="p1226217381177"></a>对于其它资源类型为null。</p>
</td>
<td class="cellrowborder" valign="top" width="14.85148514851485%" headers="mcps1.1.6.1.5 "><p id="p935789192614"><a name="p935789192614"></a><a name="p935789192614"></a>-</p>
</td>
</tr>
<tr id="row8931195121716"><td class="cellrowborder" valign="top" width="14.85148514851485%" headers="mcps1.1.6.1.1 "><p id="p29311851181715"><a name="p29311851181715"></a><a name="p29311851181715"></a>tags</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.1.6.1.2 "><p id="p10931155119177"><a name="p10931155119177"></a><a name="p10931155119177"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="18.81188118811881%" headers="mcps1.1.6.1.3 "><p id="p69311851201711"><a name="p69311851201711"></a><a name="p69311851201711"></a>Resource_tag结构体数组</p>
</td>
<td class="cellrowborder" valign="top" width="39.603960396039604%" headers="mcps1.1.6.1.4 "><p id="p20931135117174"><a name="p20931135117174"></a><a name="p20931135117174"></a>标签列表，没有标签默认为空数组。结构体说明请参见<a href="Resource_tag结构体.md">Resource_tag结构体</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="14.85148514851485%" headers="mcps1.1.6.1.5 "><p id="p15357159112611"><a name="p15357159112611"></a><a name="p15357159112611"></a>-</p>
</td>
</tr>
<tr id="row493125112175"><td class="cellrowborder" valign="top" width="14.85148514851485%" headers="mcps1.1.6.1.1 "><p id="p9931135131716"><a name="p9931135131716"></a><a name="p9931135131716"></a>resource_name</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.1.6.1.2 "><p id="p29311512174"><a name="p29311512174"></a><a name="p29311512174"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="18.81188118811881%" headers="mcps1.1.6.1.3 "><p id="p99312519176"><a name="p99312519176"></a><a name="p99312519176"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="39.603960396039604%" headers="mcps1.1.6.1.4 "><p id="p893175191714"><a name="p893175191714"></a><a name="p893175191714"></a>资源名称</p>
</td>
<td class="cellrowborder" valign="top" width="14.85148514851485%" headers="mcps1.1.6.1.5 "><p id="p203574915267"><a name="p203574915267"></a><a name="p203574915267"></a>-</p>
</td>
</tr>
</tbody>
</table>

