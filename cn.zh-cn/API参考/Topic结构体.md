# Topic结构体<a name="ZH-CN_TOPIC_0036017312"></a>

Topic结构体参数说明。

<a name="table10636317195533"></a>
<table><thead align="left"><tr id="row28583391195533"><th class="cellrowborder" valign="top" width="19.39%" id="mcps1.1.5.1.1"><p id="p33553343195533"><a name="p33553343195533"></a><a name="p33553343195533"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="18.32%" id="mcps1.1.5.1.2"><p id="p33466243195533"><a name="p33466243195533"></a><a name="p33466243195533"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="27.6%" id="mcps1.1.5.1.3"><p id="p26411156195533"><a name="p26411156195533"></a><a name="p26411156195533"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="34.69%" id="mcps1.1.5.1.4"><p id="p58928857195533"><a name="p58928857195533"></a><a name="p58928857195533"></a>约束</p>
</th>
</tr>
</thead>
<tbody><tr id="row8508090195533"><td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.1.5.1.1 "><p id="p18066721195533"><a name="p18066721195533"></a><a name="p18066721195533"></a>topic_urn</p>
</td>
<td class="cellrowborder" valign="top" width="18.32%" headers="mcps1.1.5.1.2 "><p id="p54118259195533"><a name="p54118259195533"></a><a name="p54118259195533"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="27.6%" headers="mcps1.1.5.1.3 "><p id="p21502874195533"><a name="p21502874195533"></a><a name="p21502874195533"></a>topicID</p>
</td>
<td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.1.5.1.4 "><p id="p64011262195533"><a name="p64011262195533"></a><a name="p64011262195533"></a>-</p>
</td>
</tr>
<tr id="row39230450195533"><td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.1.5.1.1 "><p id="p23549883195533"><a name="p23549883195533"></a><a name="p23549883195533"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="18.32%" headers="mcps1.1.5.1.2 "><p id="p28492405195533"><a name="p28492405195533"></a><a name="p28492405195533"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="27.6%" headers="mcps1.1.5.1.3 "><p id="p26183496195533"><a name="p26183496195533"></a><a name="p26183496195533"></a>创建topic的名字</p>
</td>
<td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.1.5.1.4 "><p id="p40488411195533"><a name="p40488411195533"></a><a name="p40488411195533"></a>-</p>
</td>
</tr>
<tr id="row28851380195533"><td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.1.5.1.1 "><p id="p55260426195533"><a name="p55260426195533"></a><a name="p55260426195533"></a>display_name</p>
</td>
<td class="cellrowborder" valign="top" width="18.32%" headers="mcps1.1.5.1.2 "><p id="p46909558195533"><a name="p46909558195533"></a><a name="p46909558195533"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="27.6%" headers="mcps1.1.5.1.3 "><p id="p41577821195533"><a name="p41577821195533"></a><a name="p41577821195533"></a>Topic的描述信息</p>
</td>
<td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.1.5.1.4 "><p id="p12360361195533"><a name="p12360361195533"></a><a name="p12360361195533"></a>-</p>
</td>
</tr>
<tr id="row44134393195533"><td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.1.5.1.1 "><p id="p18116055195533"><a name="p18116055195533"></a><a name="p18116055195533"></a>push_policy</p>
</td>
<td class="cellrowborder" valign="top" width="18.32%" headers="mcps1.1.5.1.2 "><p id="p58114317195533"><a name="p58114317195533"></a><a name="p58114317195533"></a>Int</p>
</td>
<td class="cellrowborder" valign="top" width="27.6%" headers="mcps1.1.5.1.3 "><p id="p9639236195533"><a name="p9639236195533"></a><a name="p9639236195533"></a>消息推送的策略，该属性目前不支持修改，后续将支持修改</p>
</td>
<td class="cellrowborder" valign="top" width="34.69%" headers="mcps1.1.5.1.4 "><p id="p42580643195533"><a name="p42580643195533"></a><a name="p42580643195533"></a>0表示发送失败，保留到失败队列，1表示直接丢弃发送失败的消息。</p>
</td>
</tr>
</tbody>
</table>

