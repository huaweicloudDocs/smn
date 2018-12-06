# 查询Topic属性<a name="ZH-CN_TOPIC_0038364127"></a>

## 功能介绍<a name="section64935954"></a>

-   接口名称

    ListTopicAttributes


-   功能描述

    查询Topic的属性信息。


## URI<a name="section47552675"></a>

-   URI格式

    GET /v2/\{project\_id\}/notifications/topics/\{topic\_urn\}/attributes?name=access\_policy


-   参数说明

    <a name="table60453091"></a>
    <table><thead align="left"><tr id="row31471768"><th class="cellrowborder" valign="top" width="23.69%" id="mcps1.1.5.1.1"><p id="p66185246"><a name="p66185246"></a><a name="p66185246"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.349999999999998%" id="mcps1.1.5.1.2"><p id="p59404709"><a name="p59404709"></a><a name="p59404709"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="24.64%" id="mcps1.1.5.1.3"><p id="p47052116"><a name="p47052116"></a><a name="p47052116"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="30.320000000000004%" id="mcps1.1.5.1.4"><p id="p53125076"><a name="p53125076"></a><a name="p53125076"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row57297510"><td class="cellrowborder" valign="top" width="23.69%" headers="mcps1.1.5.1.1 "><p id="p10586695"><a name="p10586695"></a><a name="p10586695"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.349999999999998%" headers="mcps1.1.5.1.2 "><p id="p52215961"><a name="p52215961"></a><a name="p52215961"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.64%" headers="mcps1.1.5.1.3 "><p id="p1634435"><a name="p1634435"></a><a name="p1634435"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.320000000000004%" headers="mcps1.1.5.1.4 "><p id="p5162792715506"><a name="p5162792715506"></a><a name="p5162792715506"></a>项目ID</p>
    <p id="p65280430"><a name="p65280430"></a><a name="p65280430"></a>获取项目ID请参考<a href="获取项目编号.md">获取项目编号</a>。</p>
    </td>
    </tr>
    <tr id="row9249362"><td class="cellrowborder" valign="top" width="23.69%" headers="mcps1.1.5.1.1 "><p id="p11000853"><a name="p11000853"></a><a name="p11000853"></a>topic_urn</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.349999999999998%" headers="mcps1.1.5.1.2 "><p id="p18653909"><a name="p18653909"></a><a name="p18653909"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.64%" headers="mcps1.1.5.1.3 "><p id="p34571641"><a name="p34571641"></a><a name="p34571641"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.320000000000004%" headers="mcps1.1.5.1.4 "><p id="p48839530"><a name="p48839530"></a><a name="p48839530"></a>Topic的唯一的资源标识。</p>
    </td>
    </tr>
    <tr id="row28333568111935"><td class="cellrowborder" valign="top" width="23.69%" headers="mcps1.1.5.1.1 "><p id="p13317684111935"><a name="p13317684111935"></a><a name="p13317684111935"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.349999999999998%" headers="mcps1.1.5.1.2 "><p id="p4990583111935"><a name="p4990583111935"></a><a name="p4990583111935"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.64%" headers="mcps1.1.5.1.3 "><p id="p1584116111935"><a name="p1584116111935"></a><a name="p1584116111935"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.320000000000004%" headers="mcps1.1.5.1.4 "><p id="p61204561111935"><a name="p61204561111935"></a><a name="p61204561111935"></a>属性名称。</p>
    <p id="p363615525300"><a name="p363615525300"></a><a name="p363615525300"></a>只支持特定的属性名称，请参见<a href="Topic属性表.md">Topic属性表</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >如果查询不带name参数，则查询Topic的所有属性值。目前支持的属性值见[Topic属性表](Topic属性表.md)。  


## 请求<a name="section25320898"></a>

请求样例

```
GET /v2/{project_id}/notifications/topics/urn:smn:regionId:8bad8a40e0f7462f8c1676e3f93a8183:test_create_topic_v2/attributes?name=access_policy
```

## 响应<a name="section26561495"></a>

-   要素说明

    <a name="table38552084"></a>
    <table><thead align="left"><tr id="row10058158"><th class="cellrowborder" valign="top" width="32.20322032203221%" id="mcps1.1.4.1.1"><p id="p9404449"><a name="p9404449"></a><a name="p9404449"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="32.20322032203221%" id="mcps1.1.4.1.2"><p id="p23562876"><a name="p23562876"></a><a name="p23562876"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="35.5935593559356%" id="mcps1.1.4.1.3"><p id="p29544808"><a name="p29544808"></a><a name="p29544808"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row33089041"><td class="cellrowborder" valign="top" width="32.20322032203221%" headers="mcps1.1.4.1.1 "><p id="p62966687"><a name="p62966687"></a><a name="p62966687"></a>request_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.20322032203221%" headers="mcps1.1.4.1.2 "><p id="p27997"><a name="p27997"></a><a name="p27997"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.5935593559356%" headers="mcps1.1.4.1.3 "><p id="p2267763"><a name="p2267763"></a><a name="p2267763"></a>请求的唯一标示ID。</p>
    </td>
    </tr>
    <tr id="row42586845"><td class="cellrowborder" valign="top" width="32.20322032203221%" headers="mcps1.1.4.1.1 "><p id="p266368914302"><a name="p266368914302"></a><a name="p266368914302"></a>attributes</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.20322032203221%" headers="mcps1.1.4.1.2 "><p id="p38092711"><a name="p38092711"></a><a name="p38092711"></a>Map</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.5935593559356%" headers="mcps1.1.4.1.3 "><p id="p65610739"><a name="p65610739"></a><a name="p65610739"></a>属性的键值对。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
       "request_id":"6837531fd3f54550927b930180a706bf",
       "attributes": {
       "access_policy": "{
             "Version": "2016-09-07", 
             "Id": "__default_policy_ID", 
             "Statement": [
                {
                  "Sid": "__user_pub_0",
                  "Effect": "Allow",
                  "Principal": {
                    "CSP": [
                             "urn:csp:iam::93dc1b4697ac493d9b7d089569f86b32:root"
                           ]
                     },
                  "Action": ["SMN:Publish","SMN:QueryTopicDetail"],
                  "Resource": "urn:smn:regionId:8bad8a40e0f7462f8c1676e3f93a8183:aaa"
                  },
                  {
                  "Sid": "__service_pub_0", 
                  "Effect": "Allow",
                  "Principal": {
                     "Service": ["obs"]
                     },
                  "Action": ["SMN:Publish","SMN:QueryTopicDetail"],
                  "Resource": "urn:smn:regionId:8bad8a40e0f7462f8c1676e3f93a8183:aaa"
                  }
                 ]
              }"
           }
      }
    ```

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >“access\_policy”属性的值是一个Json字符串，在使用的过程中需要转义。以上样例为了直观说明未做转义，需做转义才能使用。  


## 返回值<a name="section37726867"></a>

请参考[返回值](返回值.md)。

## 错误码<a name="section73211020122511"></a>

请参考[错误码说明](错误码说明.md)。

