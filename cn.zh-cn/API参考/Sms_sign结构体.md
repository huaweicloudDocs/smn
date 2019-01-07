# Sms\_sign结构体<a name="ZH-CN_TOPIC_0064407677"></a>

Sms\_sign结构体参数说明。

<a name="table6516386385736"></a>
<table><thead align="left"><tr id="row2379487285736"><th class="cellrowborder" valign="top" width="19.39%" id="mcps1.1.5.1.1"><p id="p4833649885736"><a name="p4833649885736"></a><a name="p4833649885736"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="19.45%" id="mcps1.1.5.1.2"><p id="p2294225685736"><a name="p2294225685736"></a><a name="p2294225685736"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="26.47%" id="mcps1.1.5.1.3"><p id="p4638345185736"><a name="p4638345185736"></a><a name="p4638345185736"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="34.69%" id="mcps1.1.5.1.4"><p id="p6607202685736"><a name="p6607202685736"></a><a name="p6607202685736"></a>约束</p>
</th>
</tr>
</thead>
<tbody><tr id="row5023387885736"><td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.1.5.1.1 "><p id="p4241227885736"><a name="p4241227885736"></a><a name="p4241227885736"></a>sign_id</p>
</td>
<td class="cellrowborder" valign="top" width="19.45%" headers="mcps1.1.5.1.2 "><p id="p1284246685736"><a name="p1284246685736"></a><a name="p1284246685736"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="26.47%" headers="mcps1.1.5.1.3 "><p id="p3360685185736"><a name="p3360685185736"></a><a name="p3360685185736"></a>签名的唯一标识</p>
</td>
<td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.1.5.1.4 "><p id="p3780044985736"><a name="p3780044985736"></a><a name="p3780044985736"></a>-</p>
</td>
</tr>
<tr id="row21294698114836"><td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.1.5.1.1 "><p id="p57434560114836"><a name="p57434560114836"></a><a name="p57434560114836"></a>sign_type</p>
</td>
<td class="cellrowborder" valign="top" width="19.45%" headers="mcps1.1.5.1.2 "><p id="p21687772114836"><a name="p21687772114836"></a><a name="p21687772114836"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="26.47%" headers="mcps1.1.5.1.3 "><p id="p138551111497"><a name="p138551111497"></a><a name="p138551111497"></a>签名类型</p>
</td>
<td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.1.5.1.4 "><a name="ul28430383114923"></a><a name="ul28430383114923"></a><ul id="ul28430383114923"><li>0通知类签名</li><li>1推广类签名</li></ul>
</td>
</tr>
<tr id="row465972685736"><td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.1.5.1.1 "><p id="p4189353885736"><a name="p4189353885736"></a><a name="p4189353885736"></a>sign_name</p>
</td>
<td class="cellrowborder" valign="top" width="19.45%" headers="mcps1.1.5.1.2 "><p id="p3793338185736"><a name="p3793338185736"></a><a name="p3793338185736"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="26.47%" headers="mcps1.1.5.1.3 "><p id="p5270505885736"><a name="p5270505885736"></a><a name="p5270505885736"></a>签名名称</p>
</td>
<td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.1.5.1.4 "><p id="p4125129585736"><a name="p4125129585736"></a><a name="p4125129585736"></a>签名只能由中文、英文字母和数字组成，长度为2到8个字符</p>
</td>
</tr>
<tr id="row3571733785736"><td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.1.5.1.1 "><p id="p742317885736"><a name="p742317885736"></a><a name="p742317885736"></a>reply</p>
</td>
<td class="cellrowborder" valign="top" width="19.45%" headers="mcps1.1.5.1.2 "><p id="p6440651185736"><a name="p6440651185736"></a><a name="p6440651185736"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="26.47%" headers="mcps1.1.5.1.3 "><p id="p4954488085736"><a name="p4954488085736"></a><a name="p4954488085736"></a>运营商审批返回的错误编码，具体信息请参考<a href="审批失败错误码说明.md">审批失败错误码说明</a></p>
</td>
<td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.1.5.1.4 "><a name="ul66246736104631"></a><a name="ul66246736104631"></a><ul id="ul66246736104631"><li>ERROR_001</li><li>ERROR_002</li><li>ERROR_003</li><li>ERROR_004</li><li>ERROR_005</li><li>ERROR_006</li><li>ERROR_007</li></ul>
</td>
</tr>
<tr id="row1364932785736"><td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.1.5.1.1 "><p id="p3185368785736"><a name="p3185368785736"></a><a name="p3185368785736"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="19.45%" headers="mcps1.1.5.1.2 "><p id="p3001183185736"><a name="p3001183185736"></a><a name="p3001183185736"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="26.47%" headers="mcps1.1.5.1.3 "><p id="p1503925685736"><a name="p1503925685736"></a><a name="p1503925685736"></a>签名的审批状态</p>
</td>
<td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.1.5.1.4 "><a name="ul35431032104659"></a><a name="ul35431032104659"></a><ul id="ul35431032104659"><li>0待审批</li><li>1处理中</li><li>2审批中</li><li>3审批通过</li><li>4审批不通过</li><li>5已删除</li></ul>
</td>
</tr>
<tr id="row2487316985736"><td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.1.5.1.1 "><p id="p146079485736"><a name="p146079485736"></a><a name="p146079485736"></a>create_time</p>
</td>
<td class="cellrowborder" valign="top" width="19.45%" headers="mcps1.1.5.1.2 "><p id="p5121548885736"><a name="p5121548885736"></a><a name="p5121548885736"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="26.47%" headers="mcps1.1.5.1.3 "><p id="p5481383485736"><a name="p5481383485736"></a><a name="p5481383485736"></a>签名创建时间</p>
</td>
<td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.1.5.1.4 "><p id="p1073555285736"><a name="p1073555285736"></a><a name="p1073555285736"></a>-</p>
</td>
</tr>
</tbody>
</table>

