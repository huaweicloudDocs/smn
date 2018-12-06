# 查询SMN支持的API版本号信息<a name="ZH-CN_TOPIC_0133216132"></a>

## 功能介绍<a name="zh-cn_topic_0118694332_section46354700"></a>

-   接口名称

    QueryApiSupportVersions

-   功能描述

    查询SMN开放API支持的版本号。


## URI<a name="zh-cn_topic_0118694332_section14539121"></a>

-   URI格式

    GET /


## 请求<a name="zh-cn_topic_0118694332_section63743225"></a>

-   请求样例

    ```
    GET /
    ```


## 响应<a name="zh-cn_topic_0118694332_section36818119"></a>

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
    <td class="cellrowborder" valign="top" width="57.99999999999999%" headers="mcps1.1.4.1.3 "><p id="p09481736355"><a name="p09481736355"></a><a name="p09481736355"></a>描述version相关对象的列表，结构体说明请参见<a href="Versions结构体.md">Versions结构体</a>。</p>
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

