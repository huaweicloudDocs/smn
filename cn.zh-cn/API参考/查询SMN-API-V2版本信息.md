# 查询SMN API V2版本信息<a name="ZH-CN_TOPIC_0133216133"></a>

## 功能介绍<a name="zh-cn_topic_0118694332_section46354700"></a>

-   接口名称

    QueryV2ApiInfo

-   功能描述

    查询SMN开放v2版本API信息。


## URI<a name="zh-cn_topic_0118694332_section14539121"></a>

-   URI格式

    GET /\{api\_version\}

-   参数说明

    <a name="table1952532171110"></a>
    <table><thead align="left"><tr id="row12952113251110"><th class="cellrowborder" valign="top" width="22%" id="mcps1.1.5.1.1"><p id="p13952193220115"><a name="p13952193220115"></a><a name="p13952193220115"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="16%" id="mcps1.1.5.1.2"><p id="p18427194911117"><a name="p18427194911117"></a><a name="p18427194911117"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="23%" id="mcps1.1.5.1.3"><p id="p122611473812"><a name="p122611473812"></a><a name="p122611473812"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="39%" id="mcps1.1.5.1.4"><p id="p795243271111"><a name="p795243271111"></a><a name="p795243271111"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1095203271110"><td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.1 "><p id="p1395203213111"><a name="p1395203213111"></a><a name="p1395203213111"></a>api_version</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.2 "><p id="p3427164911115"><a name="p3427164911115"></a><a name="p3427164911115"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="23%" headers="mcps1.1.5.1.3 "><p id="p12611713812"><a name="p12611713812"></a><a name="p12611713812"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="39%" headers="mcps1.1.5.1.4 "><p id="p695233216116"><a name="p695233216116"></a><a name="p695233216116"></a>待查询版本号。</p>
    <div class="note" id="note6856165481210"><a name="note6856165481210"></a><a name="note6856165481210"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p8856145451214"><a name="p8856145451214"></a><a name="p8856145451214"></a>目前仅支持v2。</p>
    </div></div>
    </td>
    </tr>
    </tbody>
    </table>


## 请求<a name="zh-cn_topic_0118694332_section63743225"></a>

-   请求样例

    ```
    GET /v2
    ```


## 响应<a name="zh-cn_topic_0118694332_section36818119"></a>

-   要素说明

    **表 1**  响应样例要素说明

    <a name="zh-cn_topic_0118694332_table26328706"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0118694332_row6366124"><th class="cellrowborder" valign="top" width="17.82178217821782%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118694332_p45894015"><a name="zh-cn_topic_0118694332_p45894015"></a><a name="zh-cn_topic_0118694332_p45894015"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="23.762376237623762%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118694332_p26427706"><a name="zh-cn_topic_0118694332_p26427706"></a><a name="zh-cn_topic_0118694332_p26427706"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="58.415841584158414%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118694332_p60269446"><a name="zh-cn_topic_0118694332_p60269446"></a><a name="zh-cn_topic_0118694332_p60269446"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0118694332_row22411503"><td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118694332_p3392477"><a name="zh-cn_topic_0118694332_p3392477"></a><a name="zh-cn_topic_0118694332_p3392477"></a>version</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.762376237623762%" headers="mcps1.2.4.1.2 "><p id="p125256566512"><a name="p125256566512"></a><a name="p125256566512"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="p09481736355"><a name="p09481736355"></a><a name="p09481736355"></a>描述version相关对象的列表</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 2**  version字段说明

    <a name="table219819244718"></a>
    <table><thead align="left"><tr id="row1526011204718"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p182602274711"><a name="p182602274711"></a><a name="p182602274711"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="28.000000000000004%" id="mcps1.2.4.1.2"><p id="p19260192154719"><a name="p19260192154719"></a><a name="p19260192154719"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="52%" id="mcps1.2.4.1.3"><p id="p126017204718"><a name="p126017204718"></a><a name="p126017204718"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row15260132164715"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p8907105518498"><a name="p8907105518498"></a><a name="p8907105518498"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.2.4.1.2 "><p id="p129078554491"><a name="p129078554491"></a><a name="p129078554491"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="52%" headers="mcps1.2.4.1.3 "><p id="p88531517575"><a name="p88531517575"></a><a name="p88531517575"></a>版本ID（版本号），如v2</p>
    </td>
    </tr>
    <tr id="row1766313211514"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1390725544917"><a name="p1390725544917"></a><a name="p1390725544917"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.2.4.1.2 "><p id="p13515150155715"><a name="p13515150155715"></a><a name="p13515150155715"></a>Links结构体数组，结构体说明请参见<a href="Links结构体.md">Links结构体</a>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="52%" headers="mcps1.2.4.1.3 "><p id="p1785191514575"><a name="p1785191514575"></a><a name="p1785191514575"></a>API的URL地址</p>
    </td>
    </tr>
    <tr id="row826819249365"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118694332_p9543622"><a name="zh-cn_topic_0118694332_p9543622"></a><a name="zh-cn_topic_0118694332_p9543622"></a>min_version</p>
    </td>
    <td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118694332_p34835893"><a name="zh-cn_topic_0118694332_p34835893"></a><a name="zh-cn_topic_0118694332_p34835893"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="52%" headers="mcps1.2.4.1.3 "><p id="p7948334354"><a name="p7948334354"></a><a name="p7948334354"></a>若该版本API支持微版本，则填支持的最小微版本号；若不支持微版本，则填空。</p>
    </td>
    </tr>
    <tr id="row972024243711"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p2069817541346"><a name="p2069817541346"></a><a name="p2069817541346"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.2.4.1.2 "><p id="p1698115415341"><a name="p1698115415341"></a><a name="p1698115415341"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="52%" headers="mcps1.2.4.1.3 "><p id="p1098793361817"><a name="p1098793361817"></a><a name="p1098793361817"></a>版本状态，为如下3种：</p>
    <a name="ul1496114571817"></a><a name="ul1496114571817"></a><ul id="ul1496114571817"><li>CURRENT：表示该版本为主推版本</li><li>SUPPORTED：表示为老版本，但是现在还继续支持</li><li>DEPRECATED：表示为废弃版本，存在后续删除的可能</li></ul>
    </td>
    </tr>
    <tr id="row79551828143611"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p14902136113515"><a name="p14902136113515"></a><a name="p14902136113515"></a>updated</p>
    </td>
    <td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.2.4.1.2 "><p id="p99021268355"><a name="p99021268355"></a><a name="p99021268355"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="52%" headers="mcps1.2.4.1.3 "><p id="p590215614356"><a name="p590215614356"></a><a name="p590215614356"></a>版本发布时间，要求用UTC时间表示。如v2发布的时间2014-06-28T12:20:21Z。</p>
    </td>
    </tr>
    <tr id="row17393526173617"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p29120166354"><a name="p29120166354"></a><a name="p29120166354"></a>version</p>
    </td>
    <td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.2.4.1.2 "><p id="p691191611356"><a name="p691191611356"></a><a name="p691191611356"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="52%" headers="mcps1.2.4.1.3 "><p id="p209171618355"><a name="p209171618355"></a><a name="p209171618355"></a>若该版本API支持微版本，则填支持的最大微版本号；若不支持微版本，则填空。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "version": 
            {
                "id": "v2",
                "links": [
                    {
                        "href": "https://127.0.0.1/v2",
                        "rel": "self"
                    }
                ],
                "min_version": "",
                "status": "CURRENT",
                "updated": "2018-09-19T00:00:00Z",
                "version": ""
            }
    }
    ```


## 返回值<a name="zh-cn_topic_0118694332_section62927619"></a>

请参考[返回值](返回值.md)。

## 错误码<a name="section73211020122511"></a>

请参考[错误码说明](错误码说明.md)。

