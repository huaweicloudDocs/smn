# 查询指定Topic的订阅者列表<a name="smn_api_52002"></a>

## 功能介绍<a name="zh-cn_topic_0025373770"></a>

-   接口名称

    ListSubscriptionsByTopic


-   功能描述

    分页获取特定Topic的订阅列表，订阅列表按照订阅创建时间进行升序排列。分页查询可以指定offset以及limit。如果指定Topic不存在订阅者，返回空列表。


## URI<a name="section37356392"></a>

-   URI格式

    GET /v2/\{project\_id\}/notifications/topics/\{topic\_urn\}/subscriptions?offset=\{offset\}&limit=\{limit\}


-   参数说明

    <a name="table10143581"></a>
    <table><thead align="left"><tr id="row8289053"><th class="cellrowborder" valign="top" width="24.709999999999997%" id="mcps1.1.5.1.1"><p id="p324668"><a name="p324668"></a><a name="p324668"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="20.06%" id="mcps1.1.5.1.2"><p id="p26298136"><a name="p26298136"></a><a name="p26298136"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.61%" id="mcps1.1.5.1.3"><p id="p49774232"><a name="p49774232"></a><a name="p49774232"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="35.620000000000005%" id="mcps1.1.5.1.4"><p id="p5180964"><a name="p5180964"></a><a name="p5180964"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row35224963"><td class="cellrowborder" valign="top" width="24.709999999999997%" headers="mcps1.1.5.1.1 "><p id="p34649765"><a name="p34649765"></a><a name="p34649765"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.06%" headers="mcps1.1.5.1.2 "><p id="p55167604"><a name="p55167604"></a><a name="p55167604"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.61%" headers="mcps1.1.5.1.3 "><p id="p39390935"><a name="p39390935"></a><a name="p39390935"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.620000000000005%" headers="mcps1.1.5.1.4 "><p id="p7542769155117"><a name="p7542769155117"></a><a name="p7542769155117"></a>项目ID</p>
    <p id="p36549175"><a name="p36549175"></a><a name="p36549175"></a>获取项目ID请参考<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    <tr id="row2129750"><td class="cellrowborder" valign="top" width="24.709999999999997%" headers="mcps1.1.5.1.1 "><p id="p38292076"><a name="p38292076"></a><a name="p38292076"></a>topic_urn</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.06%" headers="mcps1.1.5.1.2 "><p id="p14650458"><a name="p14650458"></a><a name="p14650458"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.61%" headers="mcps1.1.5.1.3 "><p id="p45836489"><a name="p45836489"></a><a name="p45836489"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.620000000000005%" headers="mcps1.1.5.1.4 "><p id="p21768161"><a name="p21768161"></a><a name="p21768161"></a>Topic的唯一的资源标识，可通过<a href="查询主题列表.md">查询主题列表</a>获取该标识。</p>
    </td>
    </tr>
    <tr id="row31297682"><td class="cellrowborder" valign="top" width="24.709999999999997%" headers="mcps1.1.5.1.1 "><p id="p52084342"><a name="p52084342"></a><a name="p52084342"></a>offset</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.06%" headers="mcps1.1.5.1.2 "><p id="p37545213172528"><a name="p37545213172528"></a><a name="p37545213172528"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.61%" headers="mcps1.1.5.1.3 "><p id="p7035667"><a name="p7035667"></a><a name="p7035667"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.620000000000005%" headers="mcps1.1.5.1.4 "><p id="p146581828102110"><a name="p146581828102110"></a><a name="p146581828102110"></a>偏移量</p>
    <p id="p21821344207"><a name="p21821344207"></a><a name="p21821344207"></a>偏移量为一个大于0小于资源总个数的整数，表示查询该偏移量后面的所有的资源数，默认值为0。</p>
    </td>
    </tr>
    <tr id="row45251091"><td class="cellrowborder" valign="top" width="24.709999999999997%" headers="mcps1.1.5.1.1 "><p id="p41459726"><a name="p41459726"></a><a name="p41459726"></a>limit</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.06%" headers="mcps1.1.5.1.2 "><p id="p6679585172531"><a name="p6679585172531"></a><a name="p6679585172531"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.61%" headers="mcps1.1.5.1.3 "><p id="p25040094"><a name="p25040094"></a><a name="p25040094"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.620000000000005%" headers="mcps1.1.5.1.4 "><a name="ul38160342182720"></a><a name="ul38160342182720"></a><ul id="ul38160342182720"><li>取值范围：1~100<p id="p3980022182720"><a name="p3980022182720"></a><a name="p3980022182720"></a>取值一般为10，20，50</p>
    </li><li>功能说明：每页返回的资源个数。</li></ul>
    <p id="p5184153012911"><a name="p5184153012911"></a><a name="p5184153012911"></a>默认值为100。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="section663215"></a>

请求样例

```
GET https://{SMN_Endpoint}/v2/{project_id}/notifications/topics/urn:smn:regionId:762bdb3251034f268af0e395c53ea09b:test_topic_v1/subscriptions?offset=0&limit=100 
```

## 响应消息<a name="section5968939"></a>

-   要素说明

    <a name="table30212363"></a>
    <table><thead align="left"><tr id="row20364417"><th class="cellrowborder" valign="top" width="27.53724627537246%" id="mcps1.1.4.1.1"><p id="p38905106"><a name="p38905106"></a><a name="p38905106"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="38.50614938506149%" id="mcps1.1.4.1.2"><p id="p64305920"><a name="p64305920"></a><a name="p64305920"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.95660433956604%" id="mcps1.1.4.1.3"><p id="p41397042"><a name="p41397042"></a><a name="p41397042"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row16425092"><td class="cellrowborder" valign="top" width="27.53724627537246%" headers="mcps1.1.4.1.1 "><p id="p55364084"><a name="p55364084"></a><a name="p55364084"></a>request_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.50614938506149%" headers="mcps1.1.4.1.2 "><p id="p55305800"><a name="p55305800"></a><a name="p55305800"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.95660433956604%" headers="mcps1.1.4.1.3 "><p id="p50584809"><a name="p50584809"></a><a name="p50584809"></a>请求的唯一标识ID。</p>
    </td>
    </tr>
    <tr id="row33559471"><td class="cellrowborder" valign="top" width="27.53724627537246%" headers="mcps1.1.4.1.1 "><p id="p33962670"><a name="p33962670"></a><a name="p33962670"></a>subscription_count</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.50614938506149%" headers="mcps1.1.4.1.2 "><p id="p66621782"><a name="p66621782"></a><a name="p66621782"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.95660433956604%" headers="mcps1.1.4.1.3 "><p id="p27655246"><a name="p27655246"></a><a name="p27655246"></a>订阅者个数。</p>
    </td>
    </tr>
    <tr id="row28015283"><td class="cellrowborder" valign="top" width="27.53724627537246%" headers="mcps1.1.4.1.1 "><p id="p54645451"><a name="p54645451"></a><a name="p54645451"></a>subscriptions</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.50614938506149%" headers="mcps1.1.4.1.2 "><p id="p64205424"><a name="p64205424"></a><a name="p64205424"></a>Subscription结构体数组</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.95660433956604%" headers="mcps1.1.4.1.3 "><p id="p33256841"><a name="p33256841"></a><a name="p33256841"></a>请参见<a href="#table62621618105717">表1</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 1**  Subscription结构体

    <a name="table62621618105717"></a>
    <table><thead align="left"><tr id="smn_api_52001_row57429145195712"><th class="cellrowborder" valign="top" width="28.6971302869713%" id="mcps1.2.4.1.1"><p id="smn_api_52001_p21249193195712"><a name="smn_api_52001_p21249193195712"></a><a name="smn_api_52001_p21249193195712"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="31.786821317868213%" id="mcps1.2.4.1.2"><p id="smn_api_52001_p43463090195712"><a name="smn_api_52001_p43463090195712"></a><a name="smn_api_52001_p43463090195712"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="39.51604839516049%" id="mcps1.2.4.1.3"><p id="smn_api_52001_p30849371195712"><a name="smn_api_52001_p30849371195712"></a><a name="smn_api_52001_p30849371195712"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="smn_api_52001_row2389422195712"><td class="cellrowborder" valign="top" width="28.6971302869713%" headers="mcps1.2.4.1.1 "><p id="smn_api_52001_p59325480195712"><a name="smn_api_52001_p59325480195712"></a><a name="smn_api_52001_p59325480195712"></a>topic_urn</p>
    </td>
    <td class="cellrowborder" valign="top" width="31.786821317868213%" headers="mcps1.2.4.1.2 "><p id="smn_api_52001_p40634595195712"><a name="smn_api_52001_p40634595195712"></a><a name="smn_api_52001_p40634595195712"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="39.51604839516049%" headers="mcps1.2.4.1.3 "><p id="smn_api_52001_p3067911195712"><a name="smn_api_52001_p3067911195712"></a><a name="smn_api_52001_p3067911195712"></a>Topic的唯一的资源标识</p>
    </td>
    </tr>
    <tr id="smn_api_52001_row21914642195712"><td class="cellrowborder" valign="top" width="28.6971302869713%" headers="mcps1.2.4.1.1 "><p id="smn_api_52001_p30255586195712"><a name="smn_api_52001_p30255586195712"></a><a name="smn_api_52001_p30255586195712"></a>protocol</p>
    </td>
    <td class="cellrowborder" valign="top" width="31.786821317868213%" headers="mcps1.2.4.1.2 "><p id="smn_api_52001_p34783382195712"><a name="smn_api_52001_p34783382195712"></a><a name="smn_api_52001_p34783382195712"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="39.51604839516049%" headers="mcps1.2.4.1.3 "><p id="smn_api_52001_p65990551195712"><a name="smn_api_52001_p65990551195712"></a><a name="smn_api_52001_p65990551195712"></a>不同协议对应不同的endpoint（接受消息的接入点）。</p>
    <p id="smn_api_52001_p15571735514"><a name="smn_api_52001_p15571735514"></a><a name="smn_api_52001_p15571735514"></a>目前支持的协议包括：</p>
    <a name="smn_api_52001_ul1715273514576"></a><a name="smn_api_52001_ul1715273514576"></a><ul id="smn_api_52001_ul1715273514576"><li>“email”：邮件传输协议，endpoint为邮箱地址。</li><li>“sms”：短信传输协议，endpoint为手机号码。</li><li>“functionstage”：FunctionGraph（函数）传输协议，endpoint为一个函数。</li><li>“functiongraph”：FunctionGraph（工作流）传输协议，endpoint为由一组函数编排成的工作流。</li><li>“http”、“https”：HTTP/HTTPS传输协议，endpoint为URL。</li></ul>
    </td>
    </tr>
    <tr id="smn_api_52001_row57165101195712"><td class="cellrowborder" valign="top" width="28.6971302869713%" headers="mcps1.2.4.1.1 "><p id="smn_api_52001_p66970508195712"><a name="smn_api_52001_p66970508195712"></a><a name="smn_api_52001_p66970508195712"></a>subscription_urn</p>
    </td>
    <td class="cellrowborder" valign="top" width="31.786821317868213%" headers="mcps1.2.4.1.2 "><p id="smn_api_52001_p55902100195712"><a name="smn_api_52001_p55902100195712"></a><a name="smn_api_52001_p55902100195712"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="39.51604839516049%" headers="mcps1.2.4.1.3 "><p id="smn_api_52001_p31776236195712"><a name="smn_api_52001_p31776236195712"></a><a name="smn_api_52001_p31776236195712"></a>订阅者的唯一资源标识。</p>
    </td>
    </tr>
    <tr id="smn_api_52001_row12318113195712"><td class="cellrowborder" valign="top" width="28.6971302869713%" headers="mcps1.2.4.1.1 "><p id="smn_api_52001_p58243097195712"><a name="smn_api_52001_p58243097195712"></a><a name="smn_api_52001_p58243097195712"></a>owner</p>
    </td>
    <td class="cellrowborder" valign="top" width="31.786821317868213%" headers="mcps1.2.4.1.2 "><p id="smn_api_52001_p20070430195712"><a name="smn_api_52001_p20070430195712"></a><a name="smn_api_52001_p20070430195712"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="39.51604839516049%" headers="mcps1.2.4.1.3 "><p id="smn_api_52001_p15092119195712"><a name="smn_api_52001_p15092119195712"></a><a name="smn_api_52001_p15092119195712"></a>Topic创建者的项目ID</p>
    </td>
    </tr>
    <tr id="smn_api_52001_row63410262195712"><td class="cellrowborder" valign="top" width="28.6971302869713%" headers="mcps1.2.4.1.1 "><p id="smn_api_52001_p35957569195712"><a name="smn_api_52001_p35957569195712"></a><a name="smn_api_52001_p35957569195712"></a>endpoint</p>
    </td>
    <td class="cellrowborder" valign="top" width="31.786821317868213%" headers="mcps1.2.4.1.2 "><p id="smn_api_52001_p26881981195712"><a name="smn_api_52001_p26881981195712"></a><a name="smn_api_52001_p26881981195712"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="39.51604839516049%" headers="mcps1.2.4.1.3 "><p id="smn_api_52001_p29956849195712"><a name="smn_api_52001_p29956849195712"></a><a name="smn_api_52001_p29956849195712"></a>接受消息的接入点</p>
    </td>
    </tr>
    <tr id="smn_api_52001_row28162748195712"><td class="cellrowborder" valign="top" width="28.6971302869713%" headers="mcps1.2.4.1.1 "><p id="smn_api_52001_p66590149195712"><a name="smn_api_52001_p66590149195712"></a><a name="smn_api_52001_p66590149195712"></a>remark</p>
    </td>
    <td class="cellrowborder" valign="top" width="31.786821317868213%" headers="mcps1.2.4.1.2 "><p id="smn_api_52001_p25092994195712"><a name="smn_api_52001_p25092994195712"></a><a name="smn_api_52001_p25092994195712"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="39.51604839516049%" headers="mcps1.2.4.1.3 "><p id="smn_api_52001_p19266652195712"><a name="smn_api_52001_p19266652195712"></a><a name="smn_api_52001_p19266652195712"></a>备注</p>
    </td>
    </tr>
    <tr id="smn_api_52001_row19637006195712"><td class="cellrowborder" valign="top" width="28.6971302869713%" headers="mcps1.2.4.1.1 "><p id="smn_api_52001_p47093678195712"><a name="smn_api_52001_p47093678195712"></a><a name="smn_api_52001_p47093678195712"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="31.786821317868213%" headers="mcps1.2.4.1.2 "><p id="smn_api_52001_p56491591195712"><a name="smn_api_52001_p56491591195712"></a><a name="smn_api_52001_p56491591195712"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="39.51604839516049%" headers="mcps1.2.4.1.3 "><p id="smn_api_52001_p12416128195712"><a name="smn_api_52001_p12416128195712"></a><a name="smn_api_52001_p12416128195712"></a>订阅者状态</p>
    <a name="smn_api_52001_ul1357151620117"></a><a name="smn_api_52001_ul1357151620117"></a><ul id="smn_api_52001_ul1357151620117"><li>0表示订阅还未确认</li><li>1表示已经确认</li><li>3表示已经取消确认</li></ul>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "request_id": "4650b14bf221492fb819c231d167e6fe", 
        "subscription_count": 2, 
        "subscriptions": [
            {
                "topic_urn": "urn:smn:regionId:762bdb3251034f268af0e395c53ea09b:test_topic_v1", 
                "protocol": "sms", 
                "subscription_urn": "urn:smn:regionId:762bdb3251034f268af0e395c53ea09b:test_topic_v1:2e778e84408e44058e6cbc6d3c377837", 
                "owner": "762bdb3251034f268af0e395c53ea09b", 
                "endpoint": "xxxxxxxxxx", 
                "remark": "", 
                "status": 0
            }, 
            {
                "topic_urn": "urn:smn:regionId:762bdb3251034f268af0e395c53ea09b:test_topic_v1", 
                "protocol": "email", 
                "subscription_urn": "urn:smn:regionId:762bdb3251034f268af0e395c53ea09b:test_topic_v1:a2d52a9f5c3b47f48c3fafb177a58796", 
                "owner": "762bdb3251034f268af0e395c53ea09b", 
                "endpoint": "xx@xx.com", 
                "remark": "", 
                "status": 0
            }
    ] 
    }
    ```


## 返回值<a name="section53720453"></a>

请参考[返回值](返回值.md)。

## 错误码<a name="section73211020122511"></a>

请参考[错误码说明](错误码说明.md)。

