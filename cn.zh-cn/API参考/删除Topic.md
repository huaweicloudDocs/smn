# 删除Topic<a name="ZH-CN_TOPIC_0036016754"></a>

## 功能介绍<a name="zh-cn_topic_0025373766"></a>

-   接口名称

    DeleteTopic


-   功能描述

    删除一个Topic以及它的所有订阅者。删除Topic操作会导致未推送的消息无法再推送给该Topic的订阅者。


## URI<a name="section6556909"></a>

-   URI格式

    DELETE /v2/\{project\_id\}/notifications/topics/\{topic\_urn\}


-   参数说明

    <a name="table36893359"></a>
    <table><thead align="left"><tr id="row46277382"><th class="cellrowborder" valign="top" width="21.862186218621858%" id="mcps1.1.5.1.1"><p id="p57480441"><a name="p57480441"></a><a name="p57480441"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.122212221222124%" id="mcps1.1.5.1.2"><p id="p25404116"><a name="p25404116"></a><a name="p25404116"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.122212221222124%" id="mcps1.1.5.1.3"><p id="p44467520"><a name="p44467520"></a><a name="p44467520"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.89338933893389%" id="mcps1.1.5.1.4"><p id="p45099364"><a name="p45099364"></a><a name="p45099364"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row13951479"><td class="cellrowborder" valign="top" width="21.862186218621858%" headers="mcps1.1.5.1.1 "><p id="p56327989"><a name="p56327989"></a><a name="p56327989"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.122212221222124%" headers="mcps1.1.5.1.2 "><p id="p66273227"><a name="p66273227"></a><a name="p66273227"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.122212221222124%" headers="mcps1.1.5.1.3 "><p id="p66531170"><a name="p66531170"></a><a name="p66531170"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.89338933893389%" headers="mcps1.1.5.1.4 "><p id="p12084664154931"><a name="p12084664154931"></a><a name="p12084664154931"></a>项目ID</p>
    <p id="p20315681"><a name="p20315681"></a><a name="p20315681"></a>获取项目ID请参考<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    <tr id="row46181951"><td class="cellrowborder" valign="top" width="21.862186218621858%" headers="mcps1.1.5.1.1 "><p id="p49750539"><a name="p49750539"></a><a name="p49750539"></a>topic_urn</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.122212221222124%" headers="mcps1.1.5.1.2 "><p id="p3261819"><a name="p3261819"></a><a name="p3261819"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.122212221222124%" headers="mcps1.1.5.1.3 "><p id="p62880759"><a name="p62880759"></a><a name="p62880759"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.89338933893389%" headers="mcps1.1.5.1.4 "><p id="p60176744"><a name="p60176744"></a><a name="p60176744"></a>Topic的唯一的资源标识，可通过<a href="查询Topic列表.md">查询Topic列表</a>获取该标识。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求<a name="section59012183"></a>

请求样例

```
DELETE https://{SMN_Endpoint}/v2/{project_id}/notifications/topics/urn:smn:regionId:f96188c7ccaf4ffba0c9aa149ab2bd57:test_topic_v2
```

## 响应<a name="section61347601"></a>

-   要素说明

    <a name="table9967070"></a>
    <table><thead align="left"><tr id="row65063572"><th class="cellrowborder" valign="top" width="31.443144314431443%" id="mcps1.1.4.1.1"><p id="p35658012"><a name="p35658012"></a><a name="p35658012"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="31.443144314431443%" id="mcps1.1.4.1.2"><p id="p2617844"><a name="p2617844"></a><a name="p2617844"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="37.11371137113711%" id="mcps1.1.4.1.3"><p id="p10718788"><a name="p10718788"></a><a name="p10718788"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row62991470"><td class="cellrowborder" valign="top" width="31.443144314431443%" headers="mcps1.1.4.1.1 "><p id="p2035480"><a name="p2035480"></a><a name="p2035480"></a>request_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="31.443144314431443%" headers="mcps1.1.4.1.2 "><p id="p30656219"><a name="p30656219"></a><a name="p30656219"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.11371137113711%" headers="mcps1.1.4.1.3 "><p id="p125790"><a name="p125790"></a><a name="p125790"></a>请求的唯一标识ID。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    { 
         "request_id": " 5fcba32bd2814ea39431829c22bda94b", 
    }
    ```


## 返回值<a name="section15257500"></a>

请参考[返回值](返回值.md)。

## 错误码<a name="section73211020122511"></a>

请参考[错误码说明](错误码说明.md)。

