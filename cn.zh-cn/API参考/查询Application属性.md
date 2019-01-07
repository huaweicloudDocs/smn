# 查询Application属性<a name="ZH-CN_TOPIC_0118712462"></a>

## 功能介绍<a name="zh-cn_topic_0118694339_section19819501"></a>

-   接口名称

    GetApplicationAttributes

-   功能描述

    获取应用平台属性。


## URI<a name="zh-cn_topic_0118694339_section44157788"></a>

-   URI格式

    GET /v2/\{project\_id\}/notifications/applications/\{application\_urn\}

-   参数说明

    <a name="zh-cn_topic_0118694339_table33304091"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0118694339_row53503647"><th class="cellrowborder" valign="top" width="20.990000000000002%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0118694339_p38828151"><a name="zh-cn_topic_0118694339_p38828151"></a><a name="zh-cn_topic_0118694339_p38828151"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.75%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0118694339_p58072540"><a name="zh-cn_topic_0118694339_p58072540"></a><a name="zh-cn_topic_0118694339_p58072540"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="20.990000000000002%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0118694339_p6255285"><a name="zh-cn_topic_0118694339_p6255285"></a><a name="zh-cn_topic_0118694339_p6255285"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="38.269999999999996%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0118694339_p36916075"><a name="zh-cn_topic_0118694339_p36916075"></a><a name="zh-cn_topic_0118694339_p36916075"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0118694339_row10478731"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0118694339_p43470919"><a name="zh-cn_topic_0118694339_p43470919"></a><a name="zh-cn_topic_0118694339_p43470919"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.75%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0118694339_p31483518"><a name="zh-cn_topic_0118694339_p31483518"></a><a name="zh-cn_topic_0118694339_p31483518"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0118694339_p28186"><a name="zh-cn_topic_0118694339_p28186"></a><a name="zh-cn_topic_0118694339_p28186"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.269999999999996%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0118694339_p2283139"><a name="zh-cn_topic_0118694339_p2283139"></a><a name="zh-cn_topic_0118694339_p2283139"></a>项目ID</p>
    <p id="zh-cn_topic_0118694339_p20548256"><a name="zh-cn_topic_0118694339_p20548256"></a><a name="zh-cn_topic_0118694339_p20548256"></a>获取项目ID请参考<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0118694339_row62509229"><td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0118694339_p30082780"><a name="zh-cn_topic_0118694339_p30082780"></a><a name="zh-cn_topic_0118694339_p30082780"></a>application_urn</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.75%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0118694339_p20786140"><a name="zh-cn_topic_0118694339_p20786140"></a><a name="zh-cn_topic_0118694339_p20786140"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0118694339_p5955797"><a name="zh-cn_topic_0118694339_p5955797"></a><a name="zh-cn_topic_0118694339_p5955797"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.269999999999996%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0118694339_p12657518"><a name="zh-cn_topic_0118694339_p12657518"></a><a name="zh-cn_topic_0118694339_p12657518"></a>Application的唯一资源标示</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求<a name="zh-cn_topic_0118694339_section61875774"></a>

-   请求样例

    ```
    GET /v2/{project_id}/notifications/applications/{application_urn}
    ```


## 响应<a name="zh-cn_topic_0118694339_section20011062"></a>

-   要素说明

    <a name="zh-cn_topic_0118694339_table65541146"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0118694339_row64426188"><th class="cellrowborder" valign="top" width="29.872987298729875%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0118694339_p51138754"><a name="zh-cn_topic_0118694339_p51138754"></a><a name="zh-cn_topic_0118694339_p51138754"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="35.063506350635066%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0118694339_p48598416"><a name="zh-cn_topic_0118694339_p48598416"></a><a name="zh-cn_topic_0118694339_p48598416"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="35.063506350635066%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0118694339_p44157663"><a name="zh-cn_topic_0118694339_p44157663"></a><a name="zh-cn_topic_0118694339_p44157663"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0118694339_row9466911"><td class="cellrowborder" valign="top" width="29.872987298729875%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0118694339_p28622303"><a name="zh-cn_topic_0118694339_p28622303"></a><a name="zh-cn_topic_0118694339_p28622303"></a>request_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0118694339_p36705216"><a name="zh-cn_topic_0118694339_p36705216"></a><a name="zh-cn_topic_0118694339_p36705216"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0118694339_p20332521"><a name="zh-cn_topic_0118694339_p20332521"></a><a name="zh-cn_topic_0118694339_p20332521"></a>请求的唯一标示ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0118694339_row58458402"><td class="cellrowborder" valign="top" width="29.872987298729875%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0118694339_p37510120"><a name="zh-cn_topic_0118694339_p37510120"></a><a name="zh-cn_topic_0118694339_p37510120"></a>attributes</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0118694339_p18420850"><a name="zh-cn_topic_0118694339_p18420850"></a><a name="zh-cn_topic_0118694339_p18420850"></a>Application_attributes结构体</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0118694339_p15693864"><a name="zh-cn_topic_0118694339_p15693864"></a><a name="zh-cn_topic_0118694339_p15693864"></a>请参见<a href="Application_attributes结构体.md">Application_attributes结构体</a></p>
    </td>
    </tr>
    <tr id="row1348515372063"><td class="cellrowborder" valign="top" width="29.872987298729875%" headers="mcps1.1.4.1.1 "><p id="p248515379613"><a name="p248515379613"></a><a name="p248515379613"></a>application_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.2 "><p id="p0485113713614"><a name="p0485113713614"></a><a name="p0485113713614"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.3 "><p id="p1148517371764"><a name="p1148517371764"></a><a name="p1148517371764"></a>Application的唯一标示ID。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   响应样例

    ```
    {
        "request_id": "c2b8643dc12b5e77ad6e35a16003229b", 
        "application_id":"b1b8643dc12b4g77ad6e35a16003119b",
        "attributes": {
            "enabled": "true", 
            "apple_certificate_expiration_date": "2018-03-09T12:21:40Z"
        }
    }
    ```


## 返回值<a name="section242171292113"></a>

请参考[返回值](返回值.md)。

## 错误码<a name="section73211020122511"></a>

请参考[错误码说明](错误码说明.md)。

