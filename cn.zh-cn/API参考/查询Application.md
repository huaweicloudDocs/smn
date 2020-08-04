# 查询Application<a name="smn_api_57004"></a>

## 功能介绍<a name="zh-cn_topic_0118694338_section3715866"></a>

-   接口名称

    ListApplication

-   功能描述

    查询应用平台列表。


## URI<a name="zh-cn_topic_0118694338_section33442794"></a>

-   URI格式

    GET /v2/\{project\_id\}/notifications/applications?offset=\{offset\}&limit=\{limit\}&name=\{name\}&platform=\{platform\}

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
    <td class="cellrowborder" valign="top" width="15.28%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0118694338_p46743437"><a name="zh-cn_topic_0118694338_p46743437"></a><a name="zh-cn_topic_0118694338_p46743437"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="45.83%" headers="mcps1.1.5.1.4 "><p id="p146581828102110"><a name="p146581828102110"></a><a name="p146581828102110"></a>偏移量</p>
    <p id="p21821344207"><a name="p21821344207"></a><a name="p21821344207"></a>偏移量为一个大于0小于资源总个数的整数，表示查询该偏移量后面的所有的资源数，默认值为0。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0118694338_row32791127"><td class="cellrowborder" valign="top" width="23.61%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0118694338_p38835591"><a name="zh-cn_topic_0118694338_p38835591"></a><a name="zh-cn_topic_0118694338_p38835591"></a>limit</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.28%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0118694338_p58675139"><a name="zh-cn_topic_0118694338_p58675139"></a><a name="zh-cn_topic_0118694338_p58675139"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.28%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0118694338_p55065844"><a name="zh-cn_topic_0118694338_p55065844"></a><a name="zh-cn_topic_0118694338_p55065844"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="45.83%" headers="mcps1.1.5.1.4 "><a name="ul38160342182720"></a><a name="ul38160342182720"></a><ul id="ul38160342182720"><li>取值范围：0~100<p id="p3980022182720"><a name="p3980022182720"></a><a name="p3980022182720"></a>取值一般为10，20，50</p>
    </li><li>功能说明：每页返回的资源个数。</li></ul>
    <p id="p5184153012911"><a name="p5184153012911"></a><a name="p5184153012911"></a>默认值为100。</p>
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
    <p id="p13766536143619"><a name="p13766536143619"></a><a name="p13766536143619"></a>HMS是为开发者提供的消息推送平台。</p>
    <p id="p15471145103612"><a name="p15471145103612"></a><a name="p15471145103612"></a>APNS和APNS_SANDBOX是用于推送iOS消息的服务平台。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="zh-cn_topic_0118694338_section32549690"></a>

-   请求样例

    ```
    GET https://{SMN_Endpoint}/v2/{project_id}/notifications/applications?offset=0&limit=100&name=application_name&platform=APNS
    ```


## 响应消息<a name="zh-cn_topic_0118694338_section24511755"></a>

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
    <td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0118694338_p54650299"><a name="zh-cn_topic_0118694338_p54650299"></a><a name="zh-cn_topic_0118694338_p54650299"></a>请求的唯一标识ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0118694338_row44511700"><td class="cellrowborder" valign="top" width="29.872987298729875%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0118694338_p48677920"><a name="zh-cn_topic_0118694338_p48677920"></a><a name="zh-cn_topic_0118694338_p48677920"></a>application_count</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0118694338_p50597473"><a name="zh-cn_topic_0118694338_p50597473"></a><a name="zh-cn_topic_0118694338_p50597473"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0118694338_p4754687"><a name="zh-cn_topic_0118694338_p4754687"></a><a name="zh-cn_topic_0118694338_p4754687"></a>返回的Application个数。</p>
    <div class="note" id="note48698383125"><a name="note48698383125"></a><a name="note48698383125"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p452954191219"><a name="p452954191219"></a><a name="p452954191219"></a>该参数不受offset和limit影响，即返回的是您账户下所有的Application个数。</p>
    </div></div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0118694338_row43615216"><td class="cellrowborder" valign="top" width="29.872987298729875%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0118694338_p43171571"><a name="zh-cn_topic_0118694338_p43171571"></a><a name="zh-cn_topic_0118694338_p43171571"></a>applications</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0118694338_p7236400"><a name="zh-cn_topic_0118694338_p7236400"></a><a name="zh-cn_topic_0118694338_p7236400"></a>Application结构体数组</p>
    </td>
    <td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0118694338_p49277517"><a name="zh-cn_topic_0118694338_p49277517"></a><a name="zh-cn_topic_0118694338_p49277517"></a>请参见<a href="#table1818919447461">表1</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 1**  Application结构体

    <a name="table1818919447461"></a>
    <table><thead align="left"><tr id="row19313104494614"><th class="cellrowborder" valign="top" width="37%" id="mcps1.2.4.1.1"><p id="p163137442461"><a name="p163137442461"></a><a name="p163137442461"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p1331310442465"><a name="p1331310442465"></a><a name="p1331310442465"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="43%" id="mcps1.2.4.1.3"><p id="p131344414469"><a name="p131344414469"></a><a name="p131344414469"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row831311441463"><td class="cellrowborder" valign="top" width="37%" headers="mcps1.2.4.1.1 "><p id="p5313164484617"><a name="p5313164484617"></a><a name="p5313164484617"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p83134441465"><a name="p83134441465"></a><a name="p83134441465"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.3 "><p id="p331384434618"><a name="p331384434618"></a><a name="p331384434618"></a>创建application的名字</p>
    </td>
    </tr>
    <tr id="row2313444194610"><td class="cellrowborder" valign="top" width="37%" headers="mcps1.2.4.1.1 "><p id="p1231324416469"><a name="p1231324416469"></a><a name="p1231324416469"></a>platform</p>
    </td>
    <td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p531316443465"><a name="p531316443465"></a><a name="p531316443465"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.3 "><p id="p1531312448463"><a name="p1531312448463"></a><a name="p1531312448463"></a>应用平台</p>
    </td>
    </tr>
    <tr id="row4313184413460"><td class="cellrowborder" valign="top" width="37%" headers="mcps1.2.4.1.1 "><p id="p12313114464614"><a name="p12313114464614"></a><a name="p12313114464614"></a>create_time</p>
    </td>
    <td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p231314474610"><a name="p231314474610"></a><a name="p231314474610"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.3 "><p id="p7313154484612"><a name="p7313154484612"></a><a name="p7313154484612"></a>创建application的时间</p>
    <p id="p119351732132717"><a name="p119351732132717"></a><a name="p119351732132717"></a>时间格式为UTC时间，YYYY-MM-DDTHH:MM:SSZ</p>
    </td>
    </tr>
    <tr id="row43132445462"><td class="cellrowborder" valign="top" width="37%" headers="mcps1.2.4.1.1 "><p id="p13131442464"><a name="p13131442464"></a><a name="p13131442464"></a>application_urn</p>
    </td>
    <td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p131334434614"><a name="p131334434614"></a><a name="p131334434614"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.3 "><p id="p173133443463"><a name="p173133443463"></a><a name="p173133443463"></a>Application的唯一资源标识</p>
    </td>
    </tr>
    <tr id="row289343131615"><td class="cellrowborder" valign="top" width="37%" headers="mcps1.2.4.1.1 "><p id="p2089333115161"><a name="p2089333115161"></a><a name="p2089333115161"></a>application_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1889393110168"><a name="p1889393110168"></a><a name="p1889393110168"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.3 "><p id="p16893123191610"><a name="p16893123191610"></a><a name="p16893123191610"></a>Application的唯一标识ID</p>
    </td>
    </tr>
    <tr id="row1831315443466"><td class="cellrowborder" valign="top" width="37%" headers="mcps1.2.4.1.1 "><p id="p131313444465"><a name="p131313444465"></a><a name="p131313444465"></a>enabled</p>
    </td>
    <td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p7313174410466"><a name="p7313174410466"></a><a name="p7313174410466"></a>boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.3 "><p id="p103131744204619"><a name="p103131744204619"></a><a name="p103131744204619"></a>应用平台是否启用</p>
    </td>
    </tr>
    <tr id="row831324418465"><td class="cellrowborder" valign="top" width="37%" headers="mcps1.2.4.1.1 "><p id="p11313044104612"><a name="p11313044104612"></a><a name="p11313044104612"></a>apple_certificate_expiration_date</p>
    </td>
    <td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p331317449461"><a name="p331317449461"></a><a name="p331317449461"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="43%" headers="mcps1.2.4.1.3 "><p id="p1331374494615"><a name="p1331374494615"></a><a name="p1331374494615"></a>苹果证书过期时间</p>
    <p id="p3129141254019"><a name="p3129141254019"></a><a name="p3129141254019"></a>APNS、APNS_SANDBOX平台特有属性</p>
    <p id="p151901011102817"><a name="p151901011102817"></a><a name="p151901011102817"></a>时间格式为UTC时间，YYYY-MM-DDTHH:MM:SSZ</p>
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
            "application_id": "b1b8643dc12b4g77ad6e35a16003119b"
        },
        {
            "create_time": "2018-01-11T12:58:58Z",
            "apple_certificate_expiration_date": "2018-03-09T12:21:40Z",
            "name": "application_name002",
            "platform": "APNS",
            "enabled": "true",
            "application_urn": "urn:smn:regionId:429ffced18074da0938112f2c362b935:app-APNS-application_name002",
            "application_id": "a3a4643dc12b4g77ad6e35a16002558c"
        }]
    }
    ```


## 返回值<a name="section242171292113"></a>

请参考[返回值](返回值.md)。

## 错误码<a name="section73211020122511"></a>

请参考[错误码说明](错误码说明.md)。

