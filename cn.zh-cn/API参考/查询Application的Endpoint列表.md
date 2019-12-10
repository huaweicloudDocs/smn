# 查询Application的Endpoint列表<a name="ZH-CN_TOPIC_0118712467"></a>

## 功能介绍<a name="zh-cn_topic_0118694309_section50470647"></a>

-   接口名称

    ListEndpointsByApplication

-   功能描述

    查询平台的endpoint列表。


## URI<a name="zh-cn_topic_0118694309_section51582645"></a>

-   URI格式

    GET /v2/\{project\_id\}/notifications/applications/\{application\_urn\}/endpoints?offset=\{offset\}&limit=\{limit\}&token=\{token\}&user\_data=\{user\_data\}&enabled=\{enabled\}

-   参数说明

    <a name="zh-cn_topic_0118694309_table47174532"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0118694309_row8478608"><th class="cellrowborder" valign="top" width="20.990000000000002%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0118694309_p15678685"><a name="zh-cn_topic_0118694309_p15678685"></a><a name="zh-cn_topic_0118694309_p15678685"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.75%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0118694309_p62013962"><a name="zh-cn_topic_0118694309_p62013962"></a><a name="zh-cn_topic_0118694309_p62013962"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="20.990000000000002%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0118694309_p57075007"><a name="zh-cn_topic_0118694309_p57075007"></a><a name="zh-cn_topic_0118694309_p57075007"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="38.269999999999996%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0118694309_p59672869"><a name="zh-cn_topic_0118694309_p59672869"></a><a name="zh-cn_topic_0118694309_p59672869"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0118694309_row584738"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0118694309_p47363850"><a name="zh-cn_topic_0118694309_p47363850"></a><a name="zh-cn_topic_0118694309_p47363850"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.75%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0118694309_p11266626"><a name="zh-cn_topic_0118694309_p11266626"></a><a name="zh-cn_topic_0118694309_p11266626"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0118694309_p40181490"><a name="zh-cn_topic_0118694309_p40181490"></a><a name="zh-cn_topic_0118694309_p40181490"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.269999999999996%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0118694309_p33475267"><a name="zh-cn_topic_0118694309_p33475267"></a><a name="zh-cn_topic_0118694309_p33475267"></a>项目ID</p>
    <p id="zh-cn_topic_0118694309_p32841951"><a name="zh-cn_topic_0118694309_p32841951"></a><a name="zh-cn_topic_0118694309_p32841951"></a>获取项目ID请参考<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0118694309_row56591389"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0118694309_p20499795"><a name="zh-cn_topic_0118694309_p20499795"></a><a name="zh-cn_topic_0118694309_p20499795"></a>application_urn</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.75%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0118694309_p49870669"><a name="zh-cn_topic_0118694309_p49870669"></a><a name="zh-cn_topic_0118694309_p49870669"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0118694309_p12992371"><a name="zh-cn_topic_0118694309_p12992371"></a><a name="zh-cn_topic_0118694309_p12992371"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.269999999999996%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0118694309_p45749167"><a name="zh-cn_topic_0118694309_p45749167"></a><a name="zh-cn_topic_0118694309_p45749167"></a>Application的唯一资源标识，可通过<a href="查询Application.md">查询Application</a>获取该标识。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0118694309_row65146268"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0118694309_p42356378"><a name="zh-cn_topic_0118694309_p42356378"></a><a name="zh-cn_topic_0118694309_p42356378"></a>offset</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.75%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0118694309_p8314568"><a name="zh-cn_topic_0118694309_p8314568"></a><a name="zh-cn_topic_0118694309_p8314568"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0118694309_p2391374"><a name="zh-cn_topic_0118694309_p2391374"></a><a name="zh-cn_topic_0118694309_p2391374"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.269999999999996%" headers="mcps1.1.5.1.4 "><p id="p146581828102110"><a name="p146581828102110"></a><a name="p146581828102110"></a>偏移量</p>
    <p id="p21821344207"><a name="p21821344207"></a><a name="p21821344207"></a>偏移量为一个大于0小于资源总个数的整数，表示查询该偏移量后面的所有的资源数，默认值为0。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0118694309_row11222187"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0118694309_p36581930"><a name="zh-cn_topic_0118694309_p36581930"></a><a name="zh-cn_topic_0118694309_p36581930"></a>limit</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.75%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0118694309_p10346342"><a name="zh-cn_topic_0118694309_p10346342"></a><a name="zh-cn_topic_0118694309_p10346342"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0118694309_p32747334"><a name="zh-cn_topic_0118694309_p32747334"></a><a name="zh-cn_topic_0118694309_p32747334"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.269999999999996%" headers="mcps1.1.5.1.4 "><a name="ul38160342182720"></a><a name="ul38160342182720"></a><ul id="ul38160342182720"><li>取值范围：0~100<p id="p3980022182720"><a name="p3980022182720"></a><a name="p3980022182720"></a>取值一般为10，20，50</p>
    </li><li>功能说明：每页返回的资源个数。</li></ul>
    <p id="p5184153012911"><a name="p5184153012911"></a><a name="p5184153012911"></a>默认值为100。</p>
    </td>
    </tr>
    <tr id="row1955012614458"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.1 "><p id="p555096184518"><a name="p555096184518"></a><a name="p555096184518"></a>enabled</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.75%" headers="mcps1.1.5.1.2 "><p id="p1572548124511"><a name="p1572548124511"></a><a name="p1572548124511"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.3 "><p id="p12572124824511"><a name="p12572124824511"></a><a name="p12572124824511"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.269999999999996%" headers="mcps1.1.5.1.4 "><p id="p20572134864517"><a name="p20572134864517"></a><a name="p20572134864517"></a>设备是否可用，值为true或false字符串。</p>
    </td>
    </tr>
    <tr id="row125141113194411"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.1 "><p id="p1199416220467"><a name="p1199416220467"></a><a name="p1199416220467"></a>token</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.75%" headers="mcps1.1.5.1.2 "><p id="p1757212480451"><a name="p1757212480451"></a><a name="p1757212480451"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.3 "><p id="p115721948164520"><a name="p115721948164520"></a><a name="p115721948164520"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.269999999999996%" headers="mcps1.1.5.1.4 "><p id="p20572114894512"><a name="p20572114894512"></a><a name="p20572114894512"></a>设备token，最大长度512个字节。</p>
    </td>
    </tr>
    <tr id="row296703610449"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.1 "><p id="p1796783634411"><a name="p1796783634411"></a><a name="p1796783634411"></a>user_data</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.75%" headers="mcps1.1.5.1.2 "><p id="p1457274894513"><a name="p1457274894513"></a><a name="p1457274894513"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.3 "><p id="p257254810459"><a name="p257254810459"></a><a name="p257254810459"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.269999999999996%" headers="mcps1.1.5.1.4 "><p id="p2572174844520"><a name="p2572174844520"></a><a name="p2572174844520"></a>用户数据，最大长度2048个字节。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="zh-cn_topic_0118694309_section61590629"></a>

-   请求样例

    ```
    GET https://{SMN_Endpoint}/v2/{project_id}/notifications/applications/{application_urn}/endpoints?offset=0&limit=10
    ```


## 响应消息<a name="zh-cn_topic_0118694309_section17444750"></a>

-   要素说明

    <a name="zh-cn_topic_0118694309_table321477"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0118694309_row19082474"><th class="cellrowborder" valign="top" width="29.872987298729875%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0118694309_p2176568"><a name="zh-cn_topic_0118694309_p2176568"></a><a name="zh-cn_topic_0118694309_p2176568"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="35.063506350635066%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0118694309_p42084359"><a name="zh-cn_topic_0118694309_p42084359"></a><a name="zh-cn_topic_0118694309_p42084359"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="35.063506350635066%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0118694309_p53389951"><a name="zh-cn_topic_0118694309_p53389951"></a><a name="zh-cn_topic_0118694309_p53389951"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0118694309_row50309255"><td class="cellrowborder" valign="top" width="29.872987298729875%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0118694309_p48517864"><a name="zh-cn_topic_0118694309_p48517864"></a><a name="zh-cn_topic_0118694309_p48517864"></a>request_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0118694309_p37632913"><a name="zh-cn_topic_0118694309_p37632913"></a><a name="zh-cn_topic_0118694309_p37632913"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0118694309_p28367147"><a name="zh-cn_topic_0118694309_p28367147"></a><a name="zh-cn_topic_0118694309_p28367147"></a>请求的唯一标识ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0118694309_row10120656"><td class="cellrowborder" valign="top" width="29.872987298729875%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0118694309_p14466778"><a name="zh-cn_topic_0118694309_p14466778"></a><a name="zh-cn_topic_0118694309_p14466778"></a>next_page_flag</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0118694309_p30958352"><a name="zh-cn_topic_0118694309_p30958352"></a><a name="zh-cn_topic_0118694309_p30958352"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0118694309_p24598620"><a name="zh-cn_topic_0118694309_p24598620"></a><a name="zh-cn_topic_0118694309_p24598620"></a>是否有下一页标识</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0118694309_row14327361"><td class="cellrowborder" valign="top" width="29.872987298729875%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0118694309_p19665615"><a name="zh-cn_topic_0118694309_p19665615"></a><a name="zh-cn_topic_0118694309_p19665615"></a>endpoints</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0118694309_p49410957"><a name="zh-cn_topic_0118694309_p49410957"></a><a name="zh-cn_topic_0118694309_p49410957"></a>Application_endpoint结构体数组</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0118694309_p42864547"><a name="zh-cn_topic_0118694309_p42864547"></a><a name="zh-cn_topic_0118694309_p42864547"></a>请参见<a href="#table219819244718">表1</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 1**  Application\_endpoint结构体

    <a name="table219819244718"></a>
    <table><thead align="left"><tr id="row1526011204718"><th class="cellrowborder" valign="top" width="26.07%" id="mcps1.2.4.1.1"><p id="p182602274711"><a name="p182602274711"></a><a name="p182602274711"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="30.349999999999998%" id="mcps1.2.4.1.2"><p id="p19260192154719"><a name="p19260192154719"></a><a name="p19260192154719"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="43.580000000000005%" id="mcps1.2.4.1.3"><p id="p126017204718"><a name="p126017204718"></a><a name="p126017204718"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row15260132164715"><td class="cellrowborder" valign="top" width="26.07%" headers="mcps1.2.4.1.1 "><p id="p326014254720"><a name="p326014254720"></a><a name="p326014254720"></a>create_time</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.349999999999998%" headers="mcps1.2.4.1.2 "><p id="p426010254715"><a name="p426010254715"></a><a name="p426010254715"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="43.580000000000005%" headers="mcps1.2.4.1.3 "><p id="p1926072174714"><a name="p1926072174714"></a><a name="p1926072174714"></a>创建application的时间</p>
    <p id="p32767359297"><a name="p32767359297"></a><a name="p32767359297"></a>时间格式为UTC时间，YYYY-MM-DDTHH:MM:SSZ</p>
    </td>
    </tr>
    <tr id="row926062154712"><td class="cellrowborder" valign="top" width="26.07%" headers="mcps1.2.4.1.1 "><p id="p4260627473"><a name="p4260627473"></a><a name="p4260627473"></a>endpoint_urn</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.349999999999998%" headers="mcps1.2.4.1.2 "><p id="p132600210471"><a name="p132600210471"></a><a name="p132600210471"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="43.580000000000005%" headers="mcps1.2.4.1.3 "><p id="p102601428470"><a name="p102601428470"></a><a name="p102601428470"></a>Application endpoint的唯一资源标识</p>
    </td>
    </tr>
    <tr id="row2026012218470"><td class="cellrowborder" valign="top" width="26.07%" headers="mcps1.2.4.1.1 "><p id="p1026016213472"><a name="p1026016213472"></a><a name="p1026016213472"></a>user_data</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.349999999999998%" headers="mcps1.2.4.1.2 "><p id="p026072164713"><a name="p026072164713"></a><a name="p026072164713"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="43.580000000000005%" headers="mcps1.2.4.1.3 "><p id="p3260102154711"><a name="p3260102154711"></a><a name="p3260102154711"></a>用户自定义数据</p>
    <p id="p142609264710"><a name="p142609264710"></a><a name="p142609264710"></a>最大长度支持UTF-8编码后2048字节</p>
    </td>
    </tr>
    <tr id="row426020218474"><td class="cellrowborder" valign="top" width="26.07%" headers="mcps1.2.4.1.1 "><p id="p7260152204714"><a name="p7260152204714"></a><a name="p7260152204714"></a>enabled</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.349999999999998%" headers="mcps1.2.4.1.2 "><p id="p182601124471"><a name="p182601124471"></a><a name="p182601124471"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="43.580000000000005%" headers="mcps1.2.4.1.3 "><p id="p17260102184712"><a name="p17260102184712"></a><a name="p17260102184712"></a>endpoint启用开关</p>
    <p id="p8810184718297"><a name="p8810184718297"></a><a name="p8810184718297"></a>true或false字符串</p>
    </td>
    </tr>
    <tr id="row52603214715"><td class="cellrowborder" valign="top" width="26.07%" headers="mcps1.2.4.1.1 "><p id="p12604220478"><a name="p12604220478"></a><a name="p12604220478"></a>token</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.349999999999998%" headers="mcps1.2.4.1.2 "><p id="p1426012124719"><a name="p1426012124719"></a><a name="p1426012124719"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="43.580000000000005%" headers="mcps1.2.4.1.3 "><p id="p92605210470"><a name="p92605210470"></a><a name="p92605210470"></a>设备token</p>
    <p id="p1226022144720"><a name="p1226022144720"></a><a name="p1226022144720"></a>最大长度512个字节</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "endpoints": [{
            "create_time": "2018-01-12T01:25:14Z",
            "endpoint_urn": "urn:smn:regionId:429ffced18074da0938112f2c362b935:endpoint-APNS-application_name-62f0bafec61c45fbbb5d0fc6bd696a2d",
            "user_data": "no user data",
            "enabled": "true",
            "token": "1f2fda4c1013c47ac4c59bd22379d88e14b07b0ebf47f2f79d1a6b06ed03390d"
        }],
        "request_id": "c90d871f77f7425cae0a8b772a563d17",
        "next_page_flag": false
    }
    ```


## 返回值<a name="section242171292113"></a>

请参考[返回值](返回值.md)。

## 错误码<a name="section73211020122511"></a>

请参考[错误码说明](错误码说明.md)。

