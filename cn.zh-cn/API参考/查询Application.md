# 查询Application<a name="ZH-CN_TOPIC_0118712461"></a>

## 功能介绍<a name="zh-cn_topic_0118694338_section3715866"></a>

-   接口名称

    ListApplication

-   功能描述

    查询应用平台列表。


## URI<a name="zh-cn_topic_0118694338_section33442794"></a>

-   URI格式

    GET /v2/\{project\_id\}/notifications/applications?offset=0&limit=100&name=application\_name&platform=APNS

-   参数说明

    <a name="zh-cn_topic_0118694338_table14235214"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0118694338_row63742381"><th class="cellrowborder" valign="top" width="23.61%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0118694338_p62859252"><a name="zh-cn_topic_0118694338_p62859252"></a><a name="zh-cn_topic_0118694338_p62859252"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.28%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0118694338_p58434680"><a name="zh-cn_topic_0118694338_p58434680"></a><a name="zh-cn_topic_0118694338_p58434680"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.28%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0118694338_p35588640"><a name="zh-cn_topic_0118694338_p35588640"></a><a name="zh-cn_topic_0118694338_p35588640"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="45.83%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0118694338_p64107605"><a name="zh-cn_topic_0118694338_p64107605"></a><a name="zh-cn_topic_0118694338_p64107605"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0118694338_row38747780"><td class="cellrowborder" valign="top" width="23.61%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0118694338_p51562446"><a name="zh-cn_topic_0118694338_p51562446"></a><a name="zh-cn_topic_0118694338_p51562446"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.28%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0118694338_p15808580"><a name="zh-cn_topic_0118694338_p15808580"></a><a name="zh-cn_topic_0118694338_p15808580"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.28%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0118694338_p5426640"><a name="zh-cn_topic_0118694338_p5426640"></a><a name="zh-cn_topic_0118694338_p5426640"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="45.83%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0118694338_p36904663"><a name="zh-cn_topic_0118694338_p36904663"></a><a name="zh-cn_topic_0118694338_p36904663"></a>项目ID</p>
    <p id="zh-cn_topic_0118694338_p63706517"><a name="zh-cn_topic_0118694338_p63706517"></a><a name="zh-cn_topic_0118694338_p63706517"></a>获取项目ID请参考<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0118694338_row24458081"><td class="cellrowborder" valign="top" width="23.61%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0118694338_p34947511"><a name="zh-cn_topic_0118694338_p34947511"></a><a name="zh-cn_topic_0118694338_p34947511"></a>offset</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.28%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0118694338_p12176142"><a name="zh-cn_topic_0118694338_p12176142"></a><a name="zh-cn_topic_0118694338_p12176142"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.28%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0118694338_p46743437"><a name="zh-cn_topic_0118694338_p46743437"></a><a name="zh-cn_topic_0118694338_p46743437"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="45.83%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0118694338_p28122077"><a name="zh-cn_topic_0118694338_p28122077"></a><a name="zh-cn_topic_0118694338_p28122077"></a>分页列表的起始页，默认值为0。</p>
    <p id="p19289241909"><a name="p19289241909"></a><a name="p19289241909"></a>offset大于等于0。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0118694338_row32791127"><td class="cellrowborder" valign="top" width="23.61%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0118694338_p38835591"><a name="zh-cn_topic_0118694338_p38835591"></a><a name="zh-cn_topic_0118694338_p38835591"></a>limit</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.28%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0118694338_p58675139"><a name="zh-cn_topic_0118694338_p58675139"></a><a name="zh-cn_topic_0118694338_p58675139"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.28%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0118694338_p55065844"><a name="zh-cn_topic_0118694338_p55065844"></a><a name="zh-cn_topic_0118694338_p55065844"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="45.83%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0118694338_p31148418"><a name="zh-cn_topic_0118694338_p31148418"></a><a name="zh-cn_topic_0118694338_p31148418"></a>一次返回列表的最大条目数 ，默认值为100。</p>
    <p id="p248818131801"><a name="p248818131801"></a><a name="p248818131801"></a>limit大于0且不大于100。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0118694338_row24401147"><td class="cellrowborder" valign="top" width="23.61%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0118694338_p30335854"><a name="zh-cn_topic_0118694338_p30335854"></a><a name="zh-cn_topic_0118694338_p30335854"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.28%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0118694338_p41285147"><a name="zh-cn_topic_0118694338_p41285147"></a><a name="zh-cn_topic_0118694338_p41285147"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.28%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0118694338_p55762600"><a name="zh-cn_topic_0118694338_p55762600"></a><a name="zh-cn_topic_0118694338_p55762600"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="45.83%" headers="mcps1.1.5.1.4 "><p id="p1326911332020"><a name="p1326911332020"></a><a name="p1326911332020"></a>检索应用名称</p>
    <p id="zh-cn_topic_0118694338_p20476733"><a name="zh-cn_topic_0118694338_p20476733"></a><a name="zh-cn_topic_0118694338_p20476733"></a>支持后向模糊匹配，长度不得超过64个字符，只能包含英文字母、下划线和数字。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0118694338_row29371040"><td class="cellrowborder" valign="top" width="23.61%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0118694338_p30244017"><a name="zh-cn_topic_0118694338_p30244017"></a><a name="zh-cn_topic_0118694338_p30244017"></a>platform</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.28%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0118694338_p33846344"><a name="zh-cn_topic_0118694338_p33846344"></a><a name="zh-cn_topic_0118694338_p33846344"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.28%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0118694338_p57199306"><a name="zh-cn_topic_0118694338_p57199306"></a><a name="zh-cn_topic_0118694338_p57199306"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="45.83%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0118694338_p2632225"><a name="zh-cn_topic_0118694338_p2632225"></a><a name="zh-cn_topic_0118694338_p2632225"></a>应用平台</p>
    <p id="p168001951808"><a name="p168001951808"></a><a name="p168001951808"></a>目前仅支持HMS、APNS、APNS_SANDBOX。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求<a name="zh-cn_topic_0118694338_section32549690"></a>

-   请求样例

    ```
    GET /v2/{project_id}/notifications/applications?offset=0&limit=100&name=application_name&platform=APNS
    ```


## 响应<a name="zh-cn_topic_0118694338_section24511755"></a>

-   要素说明

    <a name="zh-cn_topic_0118694338_table21510401"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0118694338_row56111205"><th class="cellrowborder" valign="top" width="29.872987298729875%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0118694338_p48713786"><a name="zh-cn_topic_0118694338_p48713786"></a><a name="zh-cn_topic_0118694338_p48713786"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="35.063506350635066%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0118694338_p53502616"><a name="zh-cn_topic_0118694338_p53502616"></a><a name="zh-cn_topic_0118694338_p53502616"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="35.063506350635066%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0118694338_p38744614"><a name="zh-cn_topic_0118694338_p38744614"></a><a name="zh-cn_topic_0118694338_p38744614"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0118694338_row62145011"><td class="cellrowborder" valign="top" width="29.872987298729875%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0118694338_p581122"><a name="zh-cn_topic_0118694338_p581122"></a><a name="zh-cn_topic_0118694338_p581122"></a>request_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0118694338_p47070946"><a name="zh-cn_topic_0118694338_p47070946"></a><a name="zh-cn_topic_0118694338_p47070946"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0118694338_p54650299"><a name="zh-cn_topic_0118694338_p54650299"></a><a name="zh-cn_topic_0118694338_p54650299"></a>请求的唯一标示ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0118694338_row44511700"><td class="cellrowborder" valign="top" width="29.872987298729875%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0118694338_p48677920"><a name="zh-cn_topic_0118694338_p48677920"></a><a name="zh-cn_topic_0118694338_p48677920"></a>application_count</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0118694338_p50597473"><a name="zh-cn_topic_0118694338_p50597473"></a><a name="zh-cn_topic_0118694338_p50597473"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0118694338_p4754687"><a name="zh-cn_topic_0118694338_p4754687"></a><a name="zh-cn_topic_0118694338_p4754687"></a>返回的Application个数。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0118694338_row43615216"><td class="cellrowborder" valign="top" width="29.872987298729875%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0118694338_p43171571"><a name="zh-cn_topic_0118694338_p43171571"></a><a name="zh-cn_topic_0118694338_p43171571"></a>applications</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0118694338_p7236400"><a name="zh-cn_topic_0118694338_p7236400"></a><a name="zh-cn_topic_0118694338_p7236400"></a>Application结构体数组</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0118694338_p49277517"><a name="zh-cn_topic_0118694338_p49277517"></a><a name="zh-cn_topic_0118694338_p49277517"></a>请参见<a href="Application结构体.md">Application结构体</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "request_id": "1ba562636055494980c4bc896e4a6960",
        "application_count": 2,
        "applications": [{
            "create_time": "2018-02-08T08:30:16Z",
            "apple_certificate_expiration_date": "2018-03-09T12:21:40Z",
            "name": "application_name001",
            "platform": "APNS",
            "enabled": "true",
            "application_urn": "urn:smn:regionId:429ffced18074da0938112f2c362b935:app-APNS-application_name001",
            "application_id":"b1b8643dc12b4g77ad6e35a16003119b"
        },
        {
            "create_time": "2018-01-11T12:58:58Z",
            "apple_certificate_expiration_date": "2018-03-09T12:21:40Z",
            "name": "application_name002",
            "platform": "APNS",
            "enabled": "true",
            "application_urn": "urn:smn:regionId:429ffced18074da0938112f2c362b935:app-APNS-application_name002",
            "application_id":"a3a4643dc12b4g77ad6e35a16002558c"
        }]
    }
    ```


## 返回值<a name="section242171292113"></a>

请参考[返回值](返回值.md)。

## 错误码<a name="section73211020122511"></a>

请参考[错误码说明](错误码说明.md)。

