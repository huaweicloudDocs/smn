# 查询SMN支持的API版本号信息<a name="smn_api_510001"></a>

## 功能介绍<a name="zh-cn_topic_0118694332_section46354700"></a>

-   接口名称

    QueryApiSupportVersions

-   功能描述

    查询SMN开放API支持的版本号。


## URI<a name="zh-cn_topic_0118694332_section14539121"></a>

-   URI格式

    GET /


## 请求消息<a name="zh-cn_topic_0118694332_section63743225"></a>

-   请求样例

    ```
    GET https://{SMN_Endpoint}/
    ```


## 响应消息<a name="zh-cn_topic_0118694332_section36818119"></a>

-   要素说明

    <a name="zh-cn_topic_0118694332_table26328706"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0118694332_row6366124"><th class="cellrowborder" valign="top" width="20%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0118694332_p45894015"><a name="zh-cn_topic_0118694332_p45894015"></a><a name="zh-cn_topic_0118694332_p45894015"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="22%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0118694332_p26427706"><a name="zh-cn_topic_0118694332_p26427706"></a><a name="zh-cn_topic_0118694332_p26427706"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.99999999999999%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0118694332_p60269446"><a name="zh-cn_topic_0118694332_p60269446"></a><a name="zh-cn_topic_0118694332_p60269446"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0118694332_row22411503"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0118694332_p3392477"><a name="zh-cn_topic_0118694332_p3392477"></a><a name="zh-cn_topic_0118694332_p3392477"></a>versions</p>
    </td>
    <td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0118694332_p6355195"><a name="zh-cn_topic_0118694332_p6355195"></a><a name="zh-cn_topic_0118694332_p6355195"></a>Versions结构体数组</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.99999999999999%" headers="mcps1.1.4.1.3 "><p id="p09481736355"><a name="p09481736355"></a><a name="p09481736355"></a>描述version相关对象的列表，结构体说明请参见<a href="#table219819244718">表1</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 1**  Versions结构体

    <a name="table219819244718"></a>
    <table><thead align="left"><tr id="row1526011204718"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.4.1.1"><p id="p182602274711"><a name="p182602274711"></a><a name="p182602274711"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="39%" id="mcps1.2.4.1.2"><p id="p19260192154719"><a name="p19260192154719"></a><a name="p19260192154719"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="40%" id="mcps1.2.4.1.3"><p id="p126017204718"><a name="p126017204718"></a><a name="p126017204718"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row15260132164715"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 "><p id="p8907105518498"><a name="p8907105518498"></a><a name="p8907105518498"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.2 "><p id="p129078554491"><a name="p129078554491"></a><a name="p129078554491"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.4.1.3 "><p id="p88531517575"><a name="p88531517575"></a><a name="p88531517575"></a>版本ID（版本号），如v2</p>
    </td>
    </tr>
    <tr id="row826819249365"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118694332_p9543622"><a name="zh-cn_topic_0118694332_p9543622"></a><a name="zh-cn_topic_0118694332_p9543622"></a>min_version</p>
    </td>
    <td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118694332_p34835893"><a name="zh-cn_topic_0118694332_p34835893"></a><a name="zh-cn_topic_0118694332_p34835893"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.4.1.3 "><p id="p7948334354"><a name="p7948334354"></a><a name="p7948334354"></a>若该版本API支持微版本，则返回支持的最小微版本号；若不支持微版本，则返回空。</p>
    </td>
    </tr>
    <tr id="row972024243711"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 "><p id="p2069817541346"><a name="p2069817541346"></a><a name="p2069817541346"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.2 "><p id="p1698115415341"><a name="p1698115415341"></a><a name="p1698115415341"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.4.1.3 "><p id="p1098793361817"><a name="p1098793361817"></a><a name="p1098793361817"></a>版本状态，为如下3种：</p>
    <a name="ul1496114571817"></a><a name="ul1496114571817"></a><ul id="ul1496114571817"><li>CURRENT：表示该版本为主推版本</li><li>SUPPORTED：表示为老版本，但是现在还继续支持</li><li>DEPRECATED：表示为废弃版本，存在后续删除的可能</li></ul>
    </td>
    </tr>
    <tr id="row79551828143611"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 "><p id="p14902136113515"><a name="p14902136113515"></a><a name="p14902136113515"></a>updated</p>
    </td>
    <td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.2 "><p id="p99021268355"><a name="p99021268355"></a><a name="p99021268355"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.4.1.3 "><p id="p590215614356"><a name="p590215614356"></a><a name="p590215614356"></a>版本发布时间，要求用UTC时间格式表示。如v2发布的时间2014-06-28T12:20:21Z。</p>
    </td>
    </tr>
    <tr id="row17393526173617"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 "><p id="p29120166354"><a name="p29120166354"></a><a name="p29120166354"></a>version</p>
    </td>
    <td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.2 "><p id="p691191611356"><a name="p691191611356"></a><a name="p691191611356"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.4.1.3 "><p id="p209171618355"><a name="p209171618355"></a><a name="p209171618355"></a>若该版本API支持微版本，则返回支持的最大微版本号；若不支持微版本，则返回空。</p>
    </td>
    </tr>
    <tr id="row926062154712"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 "><p id="p1390725544917"><a name="p1390725544917"></a><a name="p1390725544917"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.2 "><p id="p13515150155715"><a name="p13515150155715"></a><a name="p13515150155715"></a>Links结构体数组</p>
    </td>
    <td class="cellrowborder" valign="top" width="40%" headers="mcps1.2.4.1.3 "><p id="p1785191514575"><a name="p1785191514575"></a><a name="p1785191514575"></a>API的URL地址，结构体说明请参见<a href="#table1259118084015">表2</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 2**  Links结构体

    <a name="table1259118084015"></a>
    <table><thead align="left"><tr id="row159118012401"><th class="cellrowborder" valign="top" width="22.772277227722775%" id="mcps1.2.4.1.1"><p id="p115911807403"><a name="p115911807403"></a><a name="p115911807403"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.782178217821784%" id="mcps1.2.4.1.2"><p id="p1459115044014"><a name="p1459115044014"></a><a name="p1459115044014"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="55.44554455445545%" id="mcps1.2.4.1.3"><p id="p1559111015407"><a name="p1559111015407"></a><a name="p1559111015407"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1459113024020"><td class="cellrowborder" valign="top" width="22.772277227722775%" headers="mcps1.2.4.1.1 "><p id="p175910054015"><a name="p175910054015"></a><a name="p175910054015"></a>href</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.782178217821784%" headers="mcps1.2.4.1.2 "><p id="p459614402597"><a name="p459614402597"></a><a name="p459614402597"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.44554455445545%" headers="mcps1.2.4.1.3 "><p id="p2591150144013"><a name="p2591150144013"></a><a name="p2591150144013"></a>对应快捷链接</p>
    </td>
    </tr>
    <tr id="row459130144018"><td class="cellrowborder" valign="top" width="22.772277227722775%" headers="mcps1.2.4.1.1 "><p id="p185911807401"><a name="p185911807401"></a><a name="p185911807401"></a>rel</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.782178217821784%" headers="mcps1.2.4.1.2 "><p id="p856574025910"><a name="p856574025910"></a><a name="p856574025910"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.44554455445545%" headers="mcps1.2.4.1.3 "><p id="p959219013405"><a name="p959219013405"></a><a name="p959219013405"></a>快捷链接标记名称</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "versions": [
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
       ]
    }
    ```


## 返回值<a name="zh-cn_topic_0118694332_section62927619"></a>

请参考[返回值](返回值.md)。

## 错误码<a name="section73211020122511"></a>

请参考[错误码说明](错误码说明.md)。

