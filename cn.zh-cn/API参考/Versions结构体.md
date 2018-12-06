# Versions结构体<a name="ZH-CN_TOPIC_0133222574"></a>

<a name="table219819244718"></a>
<table><thead align="left"><tr id="row1526011204718"><th class="cellrowborder" valign="top" width="21%" id="mcps1.1.4.1.1"><p id="p182602274711"><a name="p182602274711"></a><a name="p182602274711"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="39%" id="mcps1.1.4.1.2"><p id="p19260192154719"><a name="p19260192154719"></a><a name="p19260192154719"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.1.4.1.3"><p id="p126017204718"><a name="p126017204718"></a><a name="p126017204718"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row15260132164715"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.1.4.1.1 "><p id="p8907105518498"><a name="p8907105518498"></a><a name="p8907105518498"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.1.4.1.2 "><p id="p129078554491"><a name="p129078554491"></a><a name="p129078554491"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.4.1.3 "><p id="p88531517575"><a name="p88531517575"></a><a name="p88531517575"></a>版本ID（版本号），如v2</p>
</td>
</tr>
<tr id="row826819249365"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0118694332_p9543622"><a name="zh-cn_topic_0118694332_p9543622"></a><a name="zh-cn_topic_0118694332_p9543622"></a>min_version</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0118694332_p34835893"><a name="zh-cn_topic_0118694332_p34835893"></a><a name="zh-cn_topic_0118694332_p34835893"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.4.1.3 "><p id="p7948334354"><a name="p7948334354"></a><a name="p7948334354"></a>若该版本API支持微版本，则填支持的最小微版本号；若不支持微版本，则填空。</p>
</td>
</tr>
<tr id="row972024243711"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.1.4.1.1 "><p id="p2069817541346"><a name="p2069817541346"></a><a name="p2069817541346"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.1.4.1.2 "><p id="p1698115415341"><a name="p1698115415341"></a><a name="p1698115415341"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.4.1.3 "><p id="p1098793361817"><a name="p1098793361817"></a><a name="p1098793361817"></a>版本状态，为如下3种：</p>
<a name="ul1496114571817"></a><a name="ul1496114571817"></a><ul id="ul1496114571817"><li>CURRENT：表示该版本为主推版本</li><li>SUPPORTED：表示为老版本，但是现在还继续支持</li><li>DEPRECATED：表示为废弃版本，存在后续删除的可能</li></ul>
</td>
</tr>
<tr id="row79551828143611"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.1.4.1.1 "><p id="p14902136113515"><a name="p14902136113515"></a><a name="p14902136113515"></a>updated</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.1.4.1.2 "><p id="p99021268355"><a name="p99021268355"></a><a name="p99021268355"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.4.1.3 "><p id="p590215614356"><a name="p590215614356"></a><a name="p590215614356"></a>版本发布时间，要求用UTC时间表示。如v2发布的时间2014-06-28T12:20:21Z。</p>
</td>
</tr>
<tr id="row17393526173617"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.1.4.1.1 "><p id="p29120166354"><a name="p29120166354"></a><a name="p29120166354"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.1.4.1.2 "><p id="p691191611356"><a name="p691191611356"></a><a name="p691191611356"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.4.1.3 "><p id="p209171618355"><a name="p209171618355"></a><a name="p209171618355"></a>若该版本API支持微版本，则填支持的最大微版本号；若不支持微版本，则填空。</p>
</td>
</tr>
<tr id="row926062154712"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.1.4.1.1 "><p id="p1390725544917"><a name="p1390725544917"></a><a name="p1390725544917"></a>links</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.1.4.1.2 "><p id="p13515150155715"><a name="p13515150155715"></a><a name="p13515150155715"></a>Links结构体数组，结构体说明请参见<a href="Links结构体.md">Links结构体</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.4.1.3 "><p id="p1785191514575"><a name="p1785191514575"></a><a name="p1785191514575"></a>API的URL地址</p>
</td>
</tr>
</tbody>
</table>

