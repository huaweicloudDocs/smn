# 创建Application<a name="ZH-CN_TOPIC_0118712458"></a>

## 功能介绍<a name="zh-cn_topic_0118694335_section8024025"></a>

-   接口名称

    CreateApplication

-   功能描述

    创建平台应用。


## URI<a name="zh-cn_topic_0118694335_section5107365"></a>

-   URI格式

    POST /v2/\{project\_id\}/notifications/applications

-   参数说明

    <a name="zh-cn_topic_0118694335_table29857724"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0118694335_row54175106"><th class="cellrowborder" valign="top" width="20.990000000000002%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0118694335_p26107438"><a name="zh-cn_topic_0118694335_p26107438"></a><a name="zh-cn_topic_0118694335_p26107438"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.75%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0118694335_p34327759"><a name="zh-cn_topic_0118694335_p34327759"></a><a name="zh-cn_topic_0118694335_p34327759"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="20.990000000000002%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0118694335_p29085133"><a name="zh-cn_topic_0118694335_p29085133"></a><a name="zh-cn_topic_0118694335_p29085133"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="38.269999999999996%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0118694335_p7085583"><a name="zh-cn_topic_0118694335_p7085583"></a><a name="zh-cn_topic_0118694335_p7085583"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0118694335_row49181313"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0118694335_p24263425"><a name="zh-cn_topic_0118694335_p24263425"></a><a name="zh-cn_topic_0118694335_p24263425"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.75%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0118694335_p19180389"><a name="zh-cn_topic_0118694335_p19180389"></a><a name="zh-cn_topic_0118694335_p19180389"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0118694335_p10107670"><a name="zh-cn_topic_0118694335_p10107670"></a><a name="zh-cn_topic_0118694335_p10107670"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.269999999999996%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0118694335_p13414907"><a name="zh-cn_topic_0118694335_p13414907"></a><a name="zh-cn_topic_0118694335_p13414907"></a>项目ID</p>
    <p id="zh-cn_topic_0118694335_p53625300"><a name="zh-cn_topic_0118694335_p53625300"></a><a name="zh-cn_topic_0118694335_p53625300"></a>获取项目ID请参考<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求<a name="zh-cn_topic_0118694335_section45966287"></a>

-   参数说明

    <a name="zh-cn_topic_0118694335_table20182332"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0118694335_row17966662"><th class="cellrowborder" valign="top" width="24.997500249975%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0118694335_p46013516"><a name="zh-cn_topic_0118694335_p46013516"></a><a name="zh-cn_topic_0118694335_p46013516"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.648235176482352%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0118694335_p36107286"><a name="zh-cn_topic_0118694335_p36107286"></a><a name="zh-cn_topic_0118694335_p36107286"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.648235176482352%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0118694335_p39009036"><a name="zh-cn_topic_0118694335_p39009036"></a><a name="zh-cn_topic_0118694335_p39009036"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="39.70602939706029%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0118694335_p5615384"><a name="zh-cn_topic_0118694335_p5615384"></a><a name="zh-cn_topic_0118694335_p5615384"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0118694335_row66877579"><td class="cellrowborder" valign="top" width="24.997500249975%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0118694335_p48374852"><a name="zh-cn_topic_0118694335_p48374852"></a><a name="zh-cn_topic_0118694335_p48374852"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.648235176482352%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0118694335_p26048945"><a name="zh-cn_topic_0118694335_p26048945"></a><a name="zh-cn_topic_0118694335_p26048945"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.648235176482352%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0118694335_p29589819"><a name="zh-cn_topic_0118694335_p29589819"></a><a name="zh-cn_topic_0118694335_p29589819"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="39.70602939706029%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0118694335_p47965129"><a name="zh-cn_topic_0118694335_p47965129"></a><a name="zh-cn_topic_0118694335_p47965129"></a>应用名</p>
    <p id="p2517164045715"><a name="p2517164045715"></a><a name="p2517164045715"></a>64个字符，只能包含英文字母、下划线和数字。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0118694335_row2861285"><td class="cellrowborder" valign="top" width="24.997500249975%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0118694335_p30437550"><a name="zh-cn_topic_0118694335_p30437550"></a><a name="zh-cn_topic_0118694335_p30437550"></a>platform</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.648235176482352%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0118694335_p49522455"><a name="zh-cn_topic_0118694335_p49522455"></a><a name="zh-cn_topic_0118694335_p49522455"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.648235176482352%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0118694335_p51895880"><a name="zh-cn_topic_0118694335_p51895880"></a><a name="zh-cn_topic_0118694335_p51895880"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="39.70602939706029%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0118694335_p42816746"><a name="zh-cn_topic_0118694335_p42816746"></a><a name="zh-cn_topic_0118694335_p42816746"></a>应用平台</p>
    <p id="p52368466574"><a name="p52368466574"></a><a name="p52368466574"></a>目前仅支持HMS、APNS、APNS_SANDBOX。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0118694335_row7786314"><td class="cellrowborder" valign="top" width="24.997500249975%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0118694335_p26711708"><a name="zh-cn_topic_0118694335_p26711708"></a><a name="zh-cn_topic_0118694335_p26711708"></a>platform_principal</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.648235176482352%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0118694335_p16164763"><a name="zh-cn_topic_0118694335_p16164763"></a><a name="zh-cn_topic_0118694335_p16164763"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.648235176482352%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0118694335_p34277422"><a name="zh-cn_topic_0118694335_p34277422"></a><a name="zh-cn_topic_0118694335_p34277422"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="39.70602939706029%" headers="mcps1.1.5.1.4 "><a name="ul11518185512190"></a><a name="ul11518185512190"></a><ul id="ul11518185512190"><li>对于HMS平台是APP ID，只能包含英文字母和数字，最大20个字符。</li><li>对于苹果APNS、APNS_SandBox平台是推送证书，大小不超过8K，且是Base64编码。</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0118694335_row44188613"><td class="cellrowborder" valign="top" width="24.997500249975%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0118694335_p22507915"><a name="zh-cn_topic_0118694335_p22507915"></a><a name="zh-cn_topic_0118694335_p22507915"></a>platform_credential</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.648235176482352%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0118694335_p11201833"><a name="zh-cn_topic_0118694335_p11201833"></a><a name="zh-cn_topic_0118694335_p11201833"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.648235176482352%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0118694335_p34933320"><a name="zh-cn_topic_0118694335_p34933320"></a><a name="zh-cn_topic_0118694335_p34933320"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="39.70602939706029%" headers="mcps1.1.5.1.4 "><a name="ul1026444616231"></a><a name="ul1026444616231"></a><ul id="ul1026444616231"><li>对于HMS平台是APP SECRET，<p id="p1295075013583"><a name="p1295075013583"></a><a name="p1295075013583"></a>只能包含英文字母和数字，固定32个字符。</p>
    </li><li>对于苹果APNS、APNS_SandBox平台是推送证书的私钥（private key），<p id="p112782583583"><a name="p112782583583"></a><a name="p112782583583"></a>大小不超过8K，且是Base64编码。</p>
    </li></ul>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例

    ```
    POST /v2/{project_id}/notifications/applications 
    {
        "name": "application_name", 
        "platform": "HMS", 
        "platform_principal": "appId", 
        "platform_credential": "appSecret"
    }
    ```


## 响应<a name="zh-cn_topic_0118694335_section11043400"></a>

-   要素说明

    <a name="zh-cn_topic_0118694335_table52510050"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0118694335_row28870051"><th class="cellrowborder" valign="top" width="29.872987298729875%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0118694335_p56772777"><a name="zh-cn_topic_0118694335_p56772777"></a><a name="zh-cn_topic_0118694335_p56772777"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="35.063506350635066%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0118694335_p35192261"><a name="zh-cn_topic_0118694335_p35192261"></a><a name="zh-cn_topic_0118694335_p35192261"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="35.063506350635066%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0118694335_p32000860"><a name="zh-cn_topic_0118694335_p32000860"></a><a name="zh-cn_topic_0118694335_p32000860"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0118694335_row41120801"><td class="cellrowborder" valign="top" width="29.872987298729875%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0118694335_p42450590"><a name="zh-cn_topic_0118694335_p42450590"></a><a name="zh-cn_topic_0118694335_p42450590"></a>request_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0118694335_p15945784"><a name="zh-cn_topic_0118694335_p15945784"></a><a name="zh-cn_topic_0118694335_p15945784"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0118694335_p16540118"><a name="zh-cn_topic_0118694335_p16540118"></a><a name="zh-cn_topic_0118694335_p16540118"></a>请求的唯一标示ID</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0118694335_row45259754"><td class="cellrowborder" valign="top" width="29.872987298729875%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0118694335_p42161475"><a name="zh-cn_topic_0118694335_p42161475"></a><a name="zh-cn_topic_0118694335_p42161475"></a>application_urn</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0118694335_p59636284"><a name="zh-cn_topic_0118694335_p59636284"></a><a name="zh-cn_topic_0118694335_p59636284"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0118694335_p65809661"><a name="zh-cn_topic_0118694335_p65809661"></a><a name="zh-cn_topic_0118694335_p65809661"></a>Application的唯一资源标示</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "request_id": "6a63a18b8bab40ffb71ebd9cb80d0085", 
        "application_urn": "urn:smn:regionId:f96188c7ccaf4ffba0c9aa149ab2bd57:app-HMS-application_name"
    }
    ```


## 返回值<a name="section242171292113"></a>

请参考[返回值](返回值.md)。

## 错误码<a name="section73211020122511"></a>

请参考[错误码说明](错误码说明.md)。

