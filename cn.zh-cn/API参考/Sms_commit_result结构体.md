# Sms\_commit\_result结构体<a name="ZH-CN_TOPIC_0094908499"></a>

Result结构体参数说明。

-   提交成功

    <a name="table382015620503"></a>
    <table><thead align="left"><tr id="row1282018614504"><th class="cellrowborder" valign="top" width="25%" id="mcps1.1.5.1.1"><p id="p4820196185019"><a name="p4820196185019"></a><a name="p4820196185019"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="25%" id="mcps1.1.5.1.2"><p id="p188201566506"><a name="p188201566506"></a><a name="p188201566506"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="25%" id="mcps1.1.5.1.3"><p id="p78207613506"><a name="p78207613506"></a><a name="p78207613506"></a>说明</p>
    </th>
    <th class="cellrowborder" valign="top" width="25%" id="mcps1.1.5.1.4"><p id="p48204645010"><a name="p48204645010"></a><a name="p48204645010"></a>约束</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row16820186205011"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.1 "><p id="p782016616509"><a name="p782016616509"></a><a name="p782016616509"></a>message_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.2 "><p id="p108200620506"><a name="p108200620506"></a><a name="p108200620506"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.3 "><p id="p14820116205015"><a name="p14820116205015"></a><a name="p14820116205015"></a>唯一的消息ID</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.4 "><p id="p98207617504"><a name="p98207617504"></a><a name="p98207617504"></a>-</p>
    </td>
    </tr>
    <tr id="row382018617505"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.1 "><p id="p1082015614504"><a name="p1082015614504"></a><a name="p1082015614504"></a>endpoint</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.2 "><p id="p158203645013"><a name="p158203645013"></a><a name="p158203645013"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.3 "><p id="p18203605017"><a name="p18203605017"></a><a name="p18203605017"></a>手机号码</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.4 "><p id="p10820126195011"><a name="p10820126195011"></a><a name="p10820126195011"></a>-</p>
    </td>
    </tr>
    </tbody>
    </table>

-   提交失败

    <a name="table11944201514344"></a>
    <table><thead align="left"><tr id="row1194471517343"><th class="cellrowborder" valign="top" width="25%" id="mcps1.1.5.1.1"><p id="p9243120135815"><a name="p9243120135815"></a><a name="p9243120135815"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="25%" id="mcps1.1.5.1.2"><p id="p8243320135814"><a name="p8243320135814"></a><a name="p8243320135814"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="25%" id="mcps1.1.5.1.3"><p id="p3243820105819"><a name="p3243820105819"></a><a name="p3243820105819"></a>说明</p>
    </th>
    <th class="cellrowborder" valign="top" width="25%" id="mcps1.1.5.1.4"><p id="p124372013585"><a name="p124372013585"></a><a name="p124372013585"></a>约束</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row394441513342"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.1 "><p id="p99448153348"><a name="p99448153348"></a><a name="p99448153348"></a>endpoint</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.2 "><p id="p9308141713434"><a name="p9308141713434"></a><a name="p9308141713434"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.3 "><p id="p1944815193415"><a name="p1944815193415"></a><a name="p1944815193415"></a>手机号码</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.4 "><p id="p6039915215391"><a name="p6039915215391"></a><a name="p6039915215391"></a>-</p>
    </td>
    </tr>
    <tr id="row1594413159343"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.1 "><p id="p4944615173410"><a name="p4944615173410"></a><a name="p4944615173410"></a>code</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.2 "><p id="p1542131818435"><a name="p1542131818435"></a><a name="p1542131818435"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.3 "><p id="p1794471513349"><a name="p1794471513349"></a><a name="p1794471513349"></a>错误码，请参考<a href="错误码说明.md">错误码说明</a>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.4 "><p id="p16944101583419"><a name="p16944101583419"></a><a name="p16944101583419"></a>-</p>
    </td>
    </tr>
    <tr id="row1294414154345"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.1 "><p id="p6278699416319"><a name="p6278699416319"></a><a name="p6278699416319"></a>message</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.2 "><p id="p17609122084518"><a name="p17609122084518"></a><a name="p17609122084518"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.3 "><p id="p3126308016319"><a name="p3126308016319"></a><a name="p3126308016319"></a>错误提示信息</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.4 "><p id="p14746152114411"><a name="p14746152114411"></a><a name="p14746152114411"></a>-</p>
    </td>
    </tr>
    </tbody>
    </table>


