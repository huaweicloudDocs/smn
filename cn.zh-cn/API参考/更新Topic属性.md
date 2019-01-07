# 更新Topic属性<a name="ZH-CN_TOPIC_0038364128"></a>

## 功能介绍<a name="section64935954"></a>

-   接口名称

    UpdateTopicAttribute


-   功能描述

    更新Topic的属性。


## URI<a name="section47552675"></a>

-   URI格式

    PUT /v2/\{project\_id\}/notifications/topics/\{topic\_urn\}/attributes/\{name\}


-   参数说明

    <a name="table60453091"></a>
    <table><thead align="left"><tr id="row31471768"><th class="cellrowborder" valign="top" width="24.80751924807519%" id="mcps1.1.5.1.1"><p id="p66185246"><a name="p66185246"></a><a name="p66185246"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="23.227677232276772%" id="mcps1.1.5.1.2"><p id="p59404709"><a name="p59404709"></a><a name="p59404709"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.447855214478555%" id="mcps1.1.5.1.3"><p id="p47052116"><a name="p47052116"></a><a name="p47052116"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="30.516948305169482%" id="mcps1.1.5.1.4"><p id="p53125076"><a name="p53125076"></a><a name="p53125076"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row57297510"><td class="cellrowborder" valign="top" width="24.80751924807519%" headers="mcps1.1.5.1.1 "><p id="p10586695"><a name="p10586695"></a><a name="p10586695"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.227677232276772%" headers="mcps1.1.5.1.2 "><p id="p52215961"><a name="p52215961"></a><a name="p52215961"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.447855214478555%" headers="mcps1.1.5.1.3 "><p id="p1634435"><a name="p1634435"></a><a name="p1634435"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.516948305169482%" headers="mcps1.1.5.1.4 "><p id="p45137179155033"><a name="p45137179155033"></a><a name="p45137179155033"></a>项目ID</p>
    <p id="p65280430"><a name="p65280430"></a><a name="p65280430"></a>获取项目ID请参考<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    <tr id="row9249362"><td class="cellrowborder" valign="top" width="24.80751924807519%" headers="mcps1.1.5.1.1 "><p id="p11000853"><a name="p11000853"></a><a name="p11000853"></a>topic_urn</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.227677232276772%" headers="mcps1.1.5.1.2 "><p id="p18653909"><a name="p18653909"></a><a name="p18653909"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.447855214478555%" headers="mcps1.1.5.1.3 "><p id="p34571641"><a name="p34571641"></a><a name="p34571641"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.516948305169482%" headers="mcps1.1.5.1.4 "><p id="p48839530"><a name="p48839530"></a><a name="p48839530"></a>Topic的唯一的资源标识。</p>
    </td>
    </tr>
    <tr id="row3251307152236"><td class="cellrowborder" valign="top" width="24.80751924807519%" headers="mcps1.1.5.1.1 "><p id="p62029310152236"><a name="p62029310152236"></a><a name="p62029310152236"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.227677232276772%" headers="mcps1.1.5.1.2 "><p id="p58318222152236"><a name="p58318222152236"></a><a name="p58318222152236"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.447855214478555%" headers="mcps1.1.5.1.3 "><p id="p26155522152236"><a name="p26155522152236"></a><a name="p26155522152236"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.516948305169482%" headers="mcps1.1.5.1.4 "><p id="p43921265152316"><a name="p43921265152316"></a><a name="p43921265152316"></a>属性名称。</p>
    <p id="p28391318113116"><a name="p28391318113116"></a><a name="p28391318113116"></a>只支持特定的属性名称，请参见<a href="Topic属性表.md">Topic属性表</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求<a name="section25320898"></a>

-   参数说明

    <a name="table16833793185146"></a>
    <table><thead align="left"><tr id="row46280455185146"><th class="cellrowborder" valign="top" width="17.65%" id="mcps1.1.5.1.1"><p id="p57729347185146"><a name="p57729347185146"></a><a name="p57729347185146"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.06%" id="mcps1.1.5.1.2"><p id="p45565556185146"><a name="p45565556185146"></a><a name="p45565556185146"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="25.22%" id="mcps1.1.5.1.3"><p id="p66931458185146"><a name="p66931458185146"></a><a name="p66931458185146"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="35.07%" id="mcps1.1.5.1.4"><p id="p52739028185146"><a name="p52739028185146"></a><a name="p52739028185146"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row7465062185146"><td class="cellrowborder" valign="top" width="17.65%" headers="mcps1.1.5.1.1 "><p id="p690294185146"><a name="p690294185146"></a><a name="p690294185146"></a>value</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.06%" headers="mcps1.1.5.1.2 "><p id="p55913834185146"><a name="p55913834185146"></a><a name="p55913834185146"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.22%" headers="mcps1.1.5.1.3 "><p id="p32726699185146"><a name="p32726699185146"></a><a name="p32726699185146"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.07%" headers="mcps1.1.5.1.4 "><p id="p33616928185146"><a name="p33616928185146"></a><a name="p33616928185146"></a>Topic的属性值。</p>
    <p id="p5140847203117"><a name="p5140847203117"></a><a name="p5140847203117"></a>最大支持30KB。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例

    ```
    PUT /v2/{project_id}/notifications/topics/{topic_urn}/attributes/access_policy
    ```

    ```
    {
       "value": "{
             \"Version\": \"2016-09-07\", 
             \"Id\": \"__default_policy_ID\", 
             \"Statement\": [
                {
                  \"Sid\": \"__user_pub_0\",
                  \"Effect\": \"Allow\",
                  \"Principal\": {
                    \"CSP\": [
                            \"urn:csp:iam::{domainID}:root\"
                           ]
                     },
                  \"Action\": [\"SMN:Publish\",\"SMN:QueryTopicDetail\"],
                  \"Resource\": \"{topic_urn}\"
                  },
                  {
                  \"Sid\": \"__service_pub_0\", 
                  \"Effect\": \"Allow\",
                  \"Principal\": {
                     \"Service\": [\"obs\"]
                     },
                  \"Action\": [\"SMN:Publish\",\"SMN:QueryTopicDetail\"],
                  \"Resource\": \"{topic_urn}\"
                  }
                 ]
              }"
      }
    ```

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >-   在使用以上样例时，斜体的_\{project\_id\}、__\{domainID\}_和_\{topic\_urn\}_需替换为实际值。  
    >    其中，domainID是用户的账号ID，获取方法为：登录消息通知服务控制台，单击右上角用户名下的“我的凭证”，查看“账号ID”。  
    >-   “access\_policy”属性的值是一个Json字符串，在使用的过程中需要转义。以上样例为了直观说明未做转义，需做转义才能使用。  


## 响应<a name="section26561495"></a>

-   要素说明

    <a name="table38552084"></a>
    <table><thead align="left"><tr id="row10058158"><th class="cellrowborder" valign="top" width="30.04%" id="mcps1.1.4.1.1"><p id="p9404449"><a name="p9404449"></a><a name="p9404449"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="31.380000000000003%" id="mcps1.1.4.1.2"><p id="p23562876"><a name="p23562876"></a><a name="p23562876"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="38.58%" id="mcps1.1.4.1.3"><p id="p29544808"><a name="p29544808"></a><a name="p29544808"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row33089041"><td class="cellrowborder" valign="top" width="30.04%" headers="mcps1.1.4.1.1 "><p id="p62966687"><a name="p62966687"></a><a name="p62966687"></a>request_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="31.380000000000003%" headers="mcps1.1.4.1.2 "><p id="p27997"><a name="p27997"></a><a name="p27997"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.58%" headers="mcps1.1.4.1.3 "><p id="p2267763"><a name="p2267763"></a><a name="p2267763"></a>请求的唯一标示ID。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "request_id":"6837531fd3f54550927b930180a706bf"
    }
    ```


## 返回值<a name="section37726867"></a>

请参考[返回值](返回值.md)。

## 错误码<a name="section73211020122511"></a>

请参考[错误码说明](错误码说明.md)。

