# Promotion\_sms\_commit\_result结构体<a name="ZH-CN_TOPIC_0106446347"></a>

-   提交成功

    <a name="table567461853110"></a>
    <table><thead align="left"><tr id="row5768161818316"><th class="cellrowborder" valign="top" width="25%" id="mcps1.1.5.1.1"><p id="p17681218143114"><a name="p17681218143114"></a><a name="p17681218143114"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="25%" id="mcps1.1.5.1.2"><p id="p57681818183119"><a name="p57681818183119"></a><a name="p57681818183119"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="25%" id="mcps1.1.5.1.3"><p id="p107687189318"><a name="p107687189318"></a><a name="p107687189318"></a>说明</p>
    </th>
    <th class="cellrowborder" valign="top" width="25%" id="mcps1.1.5.1.4"><p id="p18768121812310"><a name="p18768121812310"></a><a name="p18768121812310"></a>约束</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row5768101873117"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.1 "><p id="p1276891814319"><a name="p1276891814319"></a><a name="p1276891814319"></a>message_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.2 "><p id="p1176811815319"><a name="p1176811815319"></a><a name="p1176811815319"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.3 "><p id="p14768218143113"><a name="p14768218143113"></a><a name="p14768218143113"></a>唯一的消息ID</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.4 "><p id="p1576871816319"><a name="p1576871816319"></a><a name="p1576871816319"></a>-</p>
    </td>
    </tr>
    <tr id="row11768181813113"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.1 "><p id="p1976891893111"><a name="p1976891893111"></a><a name="p1976891893111"></a>endpoint</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.2 "><p id="p6768121843120"><a name="p6768121843120"></a><a name="p6768121843120"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.3 "><p id="p177682186313"><a name="p177682186313"></a><a name="p177682186313"></a>手机号码</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.4 "><p id="p14768131815310"><a name="p14768131815310"></a><a name="p14768131815310"></a>-</p>
    </td>
    </tr>
    </tbody>
    </table>


-   提交失败

    <a name="table1368991843110"></a>
    <table><thead align="left"><tr id="row11768201810315"><th class="cellrowborder" valign="top" width="25%" id="mcps1.1.5.1.1"><p id="p18768918193115"><a name="p18768918193115"></a><a name="p18768918193115"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="25%" id="mcps1.1.5.1.2"><p id="p076841818318"><a name="p076841818318"></a><a name="p076841818318"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="25%" id="mcps1.1.5.1.3"><p id="p177689188319"><a name="p177689188319"></a><a name="p177689188319"></a>说明</p>
    </th>
    <th class="cellrowborder" valign="top" width="25%" id="mcps1.1.5.1.4"><p id="p127684182314"><a name="p127684182314"></a><a name="p127684182314"></a>约束</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row17768518133117"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.1 "><p id="p476821814315"><a name="p476821814315"></a><a name="p476821814315"></a>endpoint</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.2 "><p id="p1176801815318"><a name="p1176801815318"></a><a name="p1176801815318"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.3 "><p id="p1376861817318"><a name="p1376861817318"></a><a name="p1376861817318"></a>手机号码</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.4 "><p id="p197681318133116"><a name="p197681318133116"></a><a name="p197681318133116"></a>-</p>
    </td>
    </tr>
    <tr id="row37681418143113"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.1 "><p id="p576831811313"><a name="p576831811313"></a><a name="p576831811313"></a>code</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.2 "><p id="p11768218163116"><a name="p11768218163116"></a><a name="p11768218163116"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.3 "><p id="p57681718123117"><a name="p57681718123117"></a><a name="p57681718123117"></a>错误码，请参考<a href="错误码说明.md">错误码说明</a></p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.4 "><p id="p11768161883116"><a name="p11768161883116"></a><a name="p11768161883116"></a>-</p>
    </td>
    </tr>
    <tr id="row2076819184312"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.1 "><p id="p20768018123112"><a name="p20768018123112"></a><a name="p20768018123112"></a>message</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.2 "><p id="p676817187319"><a name="p676817187319"></a><a name="p676817187319"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.3 "><p id="p97681189318"><a name="p97681189318"></a><a name="p97681189318"></a>错误提示信息</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.4 "><p id="p107688187319"><a name="p107688187319"></a><a name="p107688187319"></a>-</p>
    </td>
    </tr>
    <tr id="row1276831803112"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.1 "><p id="p14768191817318"><a name="p14768191817318"></a><a name="p14768191817318"></a>sensitive_word</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.2 "><p id="p276811819312"><a name="p276811819312"></a><a name="p276811819312"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.3 "><p id="p18768131811317"><a name="p18768131811317"></a><a name="p18768131811317"></a>内容中包含的敏感关键词</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.4 "><p id="p197681818163113"><a name="p197681818163113"></a><a name="p197681818163113"></a>-</p>
    </td>
    </tr>
    </tbody>
    </table>


