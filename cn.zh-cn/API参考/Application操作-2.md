# Application操作<a name="smn_api_80008"></a>

<a name="zh-cn_topic_0173593947_table1932617316219"></a>
<table><thead align="left"><tr id="zh-cn_topic_0173593947_row5326143118220"><th class="cellrowborder" valign="top" width="20%" id="mcps1.1.6.1.1"><p id="zh-cn_topic_0173593947_p129431911184814"><a name="zh-cn_topic_0173593947_p129431911184814"></a><a name="zh-cn_topic_0173593947_p129431911184814"></a><strong id="zh-cn_topic_0173593947_b11287572488"><a name="zh-cn_topic_0173593947_b11287572488"></a><a name="zh-cn_topic_0173593947_b11287572488"></a>权限</strong></p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.1.6.1.2"><p id="zh-cn_topic_0173593947_p13672191463819"><a name="zh-cn_topic_0173593947_p13672191463819"></a><a name="zh-cn_topic_0173593947_p13672191463819"></a><strong id="zh-cn_topic_0173593947_b1131557124814"><a name="zh-cn_topic_0173593947_b1131557124814"></a><a name="zh-cn_topic_0173593947_b1131557124814"></a>对应API接口</strong></p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.1.6.1.3"><p id="zh-cn_topic_0173593947_p7202482155253"><a name="zh-cn_topic_0173593947_p7202482155253"></a><a name="zh-cn_topic_0173593947_p7202482155253"></a><strong id="zh-cn_topic_0173593947_b1512920574485"><a name="zh-cn_topic_0173593947_b1512920574485"></a><a name="zh-cn_topic_0173593947_b1512920574485"></a>授权项</strong></p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.1.6.1.4"><p id="zh-cn_topic_0173593947_p39201783549"><a name="zh-cn_topic_0173593947_p39201783549"></a><a name="zh-cn_topic_0173593947_p39201783549"></a><strong id="zh-cn_topic_0173593947_b7920148205417"><a name="zh-cn_topic_0173593947_b7920148205417"></a><a name="zh-cn_topic_0173593947_b7920148205417"></a>IAM项目</strong></p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.1.6.1.5"><p id="zh-cn_topic_0173593947_p726171334917"><a name="zh-cn_topic_0173593947_p726171334917"></a><a name="zh-cn_topic_0173593947_p726171334917"></a><strong id="zh-cn_topic_0173593947_b144514764913"><a name="zh-cn_topic_0173593947_b144514764913"></a><a name="zh-cn_topic_0173593947_b144514764913"></a>企业项目</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0173593947_row2032619312029"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0173593947_p14330528141214"><a name="zh-cn_topic_0173593947_p14330528141214"></a><a name="zh-cn_topic_0173593947_p14330528141214"></a>创建应用</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0173593947_p0483183531219"><a name="zh-cn_topic_0173593947_p0483183531219"></a><a name="zh-cn_topic_0173593947_p0483183531219"></a>POST /v2/{project_id}/notifications/applications</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0173593947_p14415193119118"><a name="zh-cn_topic_0173593947_p14415193119118"></a><a name="zh-cn_topic_0173593947_p14415193119118"></a>smn:application:create</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0173593947_p343133104815"><a name="zh-cn_topic_0173593947_p343133104815"></a><a name="zh-cn_topic_0173593947_p343133104815"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0173593947_p46517711487"><a name="zh-cn_topic_0173593947_p46517711487"></a><a name="zh-cn_topic_0173593947_p46517711487"></a>√</p>
</td>
</tr>
<tr id="zh-cn_topic_0173593947_row180934617563"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0173593947_p1585164817562"><a name="zh-cn_topic_0173593947_p1585164817562"></a><a name="zh-cn_topic_0173593947_p1585164817562"></a>查询应用</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0173593947_p13851548145618"><a name="zh-cn_topic_0173593947_p13851548145618"></a><a name="zh-cn_topic_0173593947_p13851548145618"></a>GET /v2/{project_id}/notifications/applications?offset={offset}&amp;limit={limit}&amp;name={name}&amp;platform={platform}</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0173593947_p14851548195614"><a name="zh-cn_topic_0173593947_p14851548195614"></a><a name="zh-cn_topic_0173593947_p14851548195614"></a>smn:application:list</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0173593947_p148514818568"><a name="zh-cn_topic_0173593947_p148514818568"></a><a name="zh-cn_topic_0173593947_p148514818568"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0173593947_p128564875610"><a name="zh-cn_topic_0173593947_p128564875610"></a><a name="zh-cn_topic_0173593947_p128564875610"></a>√</p>
</td>
</tr>
<tr id="zh-cn_topic_0173593947_row123266311021"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0173593947_p1969154211128"><a name="zh-cn_topic_0173593947_p1969154211128"></a><a name="zh-cn_topic_0173593947_p1969154211128"></a>更新应用</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0173593947_p464775491218"><a name="zh-cn_topic_0173593947_p464775491218"></a><a name="zh-cn_topic_0173593947_p464775491218"></a>PUT /v2/{project_id}/notifications/applications/{application_urn}</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0173593947_p1729912611419"><a name="zh-cn_topic_0173593947_p1729912611419"></a><a name="zh-cn_topic_0173593947_p1729912611419"></a>smn:application:update</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0173593947_p3665115895110"><a name="zh-cn_topic_0173593947_p3665115895110"></a><a name="zh-cn_topic_0173593947_p3665115895110"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0173593947_p7665165815118"><a name="zh-cn_topic_0173593947_p7665165815118"></a><a name="zh-cn_topic_0173593947_p7665165815118"></a>√</p>
</td>
</tr>
<tr id="zh-cn_topic_0173593947_row12327163119217"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0173593947_p1045919216139"><a name="zh-cn_topic_0173593947_p1045919216139"></a><a name="zh-cn_topic_0173593947_p1045919216139"></a>删除应用</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0173593947_p1650151791311"><a name="zh-cn_topic_0173593947_p1650151791311"></a><a name="zh-cn_topic_0173593947_p1650151791311"></a>DELETE /v2/{project_id}/notifications/applications/{application_urn}</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0173593947_p8576640191118"><a name="zh-cn_topic_0173593947_p8576640191118"></a><a name="zh-cn_topic_0173593947_p8576640191118"></a>smn:application:delete</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0173593947_p1925614118523"><a name="zh-cn_topic_0173593947_p1925614118523"></a><a name="zh-cn_topic_0173593947_p1925614118523"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0173593947_p625661175215"><a name="zh-cn_topic_0173593947_p625661175215"></a><a name="zh-cn_topic_0173593947_p625661175215"></a>√</p>
</td>
</tr>
</tbody>
</table>

