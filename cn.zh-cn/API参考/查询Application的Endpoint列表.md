# 查询Application的Endpoint列表<a name="ZH-CN_TOPIC_0118712467"></a>

## 功能介绍<a name="zh-cn_topic_0118694309_section50470647"></a>

-   接口名称

    ListEndpointsByApplication

-   功能描述

    查询平台的endpoint列表。


## URI<a name="zh-cn_topic_0118694309_section51582645"></a>

-   URI格式

    GET /v2/\{project\_id\}/notifications/applications/\{application\_urn\}/endpoints?offset=0&limit=10&token=xxxxxxxxxxxx&user\_data=xxxxxx&enabled=true

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
    <td class="cellrowborder" valign="top" width="38.269999999999996%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0118694309_p45749167"><a name="zh-cn_topic_0118694309_p45749167"></a><a name="zh-cn_topic_0118694309_p45749167"></a>Application的唯一资源标示</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0118694309_row65146268"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0118694309_p42356378"><a name="zh-cn_topic_0118694309_p42356378"></a><a name="zh-cn_topic_0118694309_p42356378"></a>offset</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.75%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0118694309_p8314568"><a name="zh-cn_topic_0118694309_p8314568"></a><a name="zh-cn_topic_0118694309_p8314568"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0118694309_p2391374"><a name="zh-cn_topic_0118694309_p2391374"></a><a name="zh-cn_topic_0118694309_p2391374"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.269999999999996%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0118694309_p59483605"><a name="zh-cn_topic_0118694309_p59483605"></a><a name="zh-cn_topic_0118694309_p59483605"></a>分页列表的起始页，默认值为0。</p>
    <p id="p167291933721"><a name="p167291933721"></a><a name="p167291933721"></a>offset大于等于0。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0118694309_row11222187"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0118694309_p36581930"><a name="zh-cn_topic_0118694309_p36581930"></a><a name="zh-cn_topic_0118694309_p36581930"></a>limit</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.75%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0118694309_p10346342"><a name="zh-cn_topic_0118694309_p10346342"></a><a name="zh-cn_topic_0118694309_p10346342"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0118694309_p32747334"><a name="zh-cn_topic_0118694309_p32747334"></a><a name="zh-cn_topic_0118694309_p32747334"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.269999999999996%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0118694309_p35288370"><a name="zh-cn_topic_0118694309_p35288370"></a><a name="zh-cn_topic_0118694309_p35288370"></a>一次返回列表的最大条目数，默认值为100。</p>
    <p id="p1260434019220"><a name="p1260434019220"></a><a name="p1260434019220"></a>limit大于0且不大于100。</p>
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


## 请求<a name="zh-cn_topic_0118694309_section61590629"></a>

-   请求样例

    ```
    GET /v2/{project_id}/notifications/applications/{application_urn}/endpoints?offset=0&limit=10
    ```


## 响应<a name="zh-cn_topic_0118694309_section17444750"></a>

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
    <td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0118694309_p28367147"><a name="zh-cn_topic_0118694309_p28367147"></a><a name="zh-cn_topic_0118694309_p28367147"></a>请求的唯一标示ID。</p>
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
    <td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0118694309_p42864547"><a name="zh-cn_topic_0118694309_p42864547"></a><a name="zh-cn_topic_0118694309_p42864547"></a>请参见<a href="Application_endpoint结构体.md">Application_endpoint结构体</a>。</p>
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

