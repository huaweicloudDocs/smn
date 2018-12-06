# 更新Topic<a name="ZH-CN_TOPIC_0036017301"></a>

## 功能介绍<a name="section37714282185146"></a>

-   接口名称

    UpdateTopic


-   功能描述

    更新显示名。


## URI<a name="section46186214185146"></a>

-   URI格式

    PUT /v2/\{project\_id\}/notifications/topics/\{topic\_urn\}


-   参数说明

    <a name="table20000134185146"></a>
    <table><thead align="left"><tr id="row37235592185146"><th class="cellrowborder" valign="top" width="22.887711228877112%" id="mcps1.1.5.1.1"><p id="p63292990185146"><a name="p63292990185146"></a><a name="p63292990185146"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="24.047595240475953%" id="mcps1.1.5.1.2"><p id="p26458572185146"><a name="p26458572185146"></a><a name="p26458572185146"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="26.957304269573047%" id="mcps1.1.5.1.3"><p id="p62769627185146"><a name="p62769627185146"></a><a name="p62769627185146"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="26.107389261073894%" id="mcps1.1.5.1.4"><p id="p51175059185146"><a name="p51175059185146"></a><a name="p51175059185146"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row13917467185146"><td class="cellrowborder" valign="top" width="22.887711228877112%" headers="mcps1.1.5.1.1 "><p id="p53573052185146"><a name="p53573052185146"></a><a name="p53573052185146"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.047595240475953%" headers="mcps1.1.5.1.2 "><p id="p44449957185146"><a name="p44449957185146"></a><a name="p44449957185146"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.957304269573047%" headers="mcps1.1.5.1.3 "><p id="p43676799185146"><a name="p43676799185146"></a><a name="p43676799185146"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.107389261073894%" headers="mcps1.1.5.1.4 "><p id="p60845278154921"><a name="p60845278154921"></a><a name="p60845278154921"></a>项目ID</p>
    <p id="p48159858185146"><a name="p48159858185146"></a><a name="p48159858185146"></a>获取项目ID请参考<a href="获取项目编号.md">获取项目编号</a>。</p>
    </td>
    </tr>
    <tr id="row10600782185146"><td class="cellrowborder" valign="top" width="22.887711228877112%" headers="mcps1.1.5.1.1 "><p id="p53356996185146"><a name="p53356996185146"></a><a name="p53356996185146"></a>topic_urn</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.047595240475953%" headers="mcps1.1.5.1.2 "><p id="p26949456185146"><a name="p26949456185146"></a><a name="p26949456185146"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.957304269573047%" headers="mcps1.1.5.1.3 "><p id="p35422295185146"><a name="p35422295185146"></a><a name="p35422295185146"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.107389261073894%" headers="mcps1.1.5.1.4 "><p id="p50633667185146"><a name="p50633667185146"></a><a name="p50633667185146"></a>Topic的唯一的资源标识。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求<a name="section18618345185146"></a>

-   参数说明

    <a name="table16833793185146"></a>
    <table><thead align="left"><tr id="row46280455185146"><th class="cellrowborder" valign="top" width="24.55754424557544%" id="mcps1.1.5.1.1"><p id="p57729347185146"><a name="p57729347185146"></a><a name="p57729347185146"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="20.537946205379455%" id="mcps1.1.5.1.2"><p id="p45565556185146"><a name="p45565556185146"></a><a name="p45565556185146"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.15788421157884%" id="mcps1.1.5.1.3"><p id="p66931458185146"><a name="p66931458185146"></a><a name="p66931458185146"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.74662533746625%" id="mcps1.1.5.1.4"><p id="p52739028185146"><a name="p52739028185146"></a><a name="p52739028185146"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row7465062185146"><td class="cellrowborder" valign="top" width="24.55754424557544%" headers="mcps1.1.5.1.1 "><p id="p690294185146"><a name="p690294185146"></a><a name="p690294185146"></a>display_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.537946205379455%" headers="mcps1.1.5.1.2 "><p id="p55913834185146"><a name="p55913834185146"></a><a name="p55913834185146"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.15788421157884%" headers="mcps1.1.5.1.3 "><p id="p32726699185146"><a name="p32726699185146"></a><a name="p32726699185146"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.74662533746625%" headers="mcps1.1.5.1.4 "><p id="p17720185311254"><a name="p17720185311254"></a><a name="p17720185311254"></a>Topic的显示名，推送邮件消息时，作为邮件发件人显示。</p>
    <p id="p57656838184157"><a name="p57656838184157"></a><a name="p57656838184157"></a>显示名的长度为192byte或64个中文。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例

    ```
    PUT /v2/{project_id}/notifications/topics/urn:smn:regionId:f96188c7ccaf4ffba0c9aa149ab2bd57:test_topic_v2
    ```

    ```
    { 
        "display_name":"testtest222"
    }
    ```


## 响应<a name="section11007541185146"></a>

-   要素说明

    <a name="table11342130185146"></a>
    <table><thead align="left"><tr id="row63969717185146"><th class="cellrowborder" valign="top" width="17.349999999999998%" id="mcps1.1.5.1.1"><p id="p14164593185146"><a name="p14164593185146"></a><a name="p14164593185146"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.310000000000002%" id="mcps1.1.5.1.2"><p id="p6481381185146"><a name="p6481381185146"></a><a name="p6481381185146"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.67%" id="mcps1.1.5.1.3"><p id="p55229882185146"><a name="p55229882185146"></a><a name="p55229882185146"></a>说明</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.67%" id="mcps1.1.5.1.4"><p id="p44435480185146"><a name="p44435480185146"></a><a name="p44435480185146"></a>约束</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row42504102185146"><td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.1.5.1.1 "><p id="p20280204185146"><a name="p20280204185146"></a><a name="p20280204185146"></a>request_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.310000000000002%" headers="mcps1.1.5.1.2 "><p id="p32083827185146"><a name="p32083827185146"></a><a name="p32083827185146"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.67%" headers="mcps1.1.5.1.3 "><p id="p48653186185146"><a name="p48653186185146"></a><a name="p48653186185146"></a>请求的唯一标示ID。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.67%" headers="mcps1.1.5.1.4 "><p id="p48594018185146"><a name="p48594018185146"></a><a name="p48594018185146"></a>-</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "request_id": "6a63a18b8bab40ffb71ebd9cb80d0085"
    }
    ```


## 返回值<a name="section26976275185146"></a>

请参考[返回值](返回值.md)。

## 错误码<a name="section73211020122511"></a>

请参考[错误码说明](错误码说明.md)。

