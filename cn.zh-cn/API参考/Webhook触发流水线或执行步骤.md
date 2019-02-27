# Webhook触发流水线或执行步骤<a name="swr_02_0090"></a>

## 功能介绍<a name="section163491716123910"></a>

通过流水线或执行步骤前置操作中webhook类型的url触发流水线或stage。

## URI<a name="section16349101618390"></a>

**URI格式**

POST /v2/manage/webhooks/\{webhook\_id\}?\{param1\}=\{paramvalue1\}&\{params2\}= \{paramvalue2\}…

POST /v3/manage/webhooks/\{webhook\_id\}?\{param1\}=\{paramvalue1\}&\{params2\}= \{paramvalue2\}…

**表 1**  参数说明

<a name="table33491916143913"></a>
<table><thead align="left"><tr id="row17411918103917"><th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.1"><p id="p1241218203910"><a name="p1241218203910"></a><a name="p1241218203910"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="p17411918203911"><a name="p17411918203911"></a><a name="p17411918203911"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="16%" id="mcps1.2.5.1.3"><p id="p441111813399"><a name="p441111813399"></a><a name="p441111813399"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="p204171810395"><a name="p204171810395"></a><a name="p204171810395"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row7411918173919"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="p5418189392"><a name="p5418189392"></a><a name="p5418189392"></a>webhook_id</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p1841121818398"><a name="p1841121818398"></a><a name="p1841121818398"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.3 "><p id="p11418185397"><a name="p11418185397"></a><a name="p11418185397"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p14151817396"><a name="p14151817396"></a><a name="p14151817396"></a>通过流水线详情接口的url获取</p>
</td>
</tr>
<tr id="row3415187393"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="p5417185392"><a name="p5417185392"></a><a name="p5417185392"></a>param1</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p24171814392"><a name="p24171814392"></a><a name="p24171814392"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.3 "><p id="p134212181396"><a name="p134212181396"></a><a name="p134212181396"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p64291823910"><a name="p64291823910"></a><a name="p64291823910"></a>触发参数，在webhook trigger的触发参数定义</p>
</td>
</tr>
<tr id="row19421189395"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="p17421418123915"><a name="p17421418123915"></a><a name="p17421418123915"></a>paramvalue1</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p1642161819390"><a name="p1642161819390"></a><a name="p1642161819390"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.3 "><p id="p242101883914"><a name="p242101883914"></a><a name="p242101883914"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p1742218153916"><a name="p1742218153916"></a><a name="p1742218153916"></a>触发参数param1对应的值</p>
</td>
</tr>
<tr id="row1342418113910"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="p6421818203914"><a name="p6421818203914"></a><a name="p6421818203914"></a>…</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p5434185393"><a name="p5434185393"></a><a name="p5434185393"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.3 "><p id="p343161810393"><a name="p343161810393"></a><a name="p343161810393"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p84321863918"><a name="p84321863918"></a><a name="p84321863918"></a>-</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section15365116193914"></a>

**请求参数**

**表 2**  Request Header参数说明

<a name="table133654162399"></a>
<table><thead align="left"><tr id="row164541810394"><th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.1"><p id="p545111843917"><a name="p545111843917"></a><a name="p545111843917"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="p8455185392"><a name="p8455185392"></a><a name="p8455185392"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="16%" id="mcps1.2.5.1.3"><p id="p20451718173917"><a name="p20451718173917"></a><a name="p20451718173917"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="p164561843914"><a name="p164561843914"></a><a name="p164561843914"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row7455186392"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="p04514182394"><a name="p04514182394"></a><a name="p04514182394"></a>X-Auth-Token</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p184531853917"><a name="p184531853917"></a><a name="p184531853917"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.3 "><p id="p19451318183916"><a name="p19451318183916"></a><a name="p19451318183916"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p045618113914"><a name="p045618113914"></a><a name="p045618113914"></a>用户Token，需从华为云IAM服务获取。</p>
</td>
</tr>
</tbody>
</table>

**请求示例**

```
N/A
```

## 响应消息<a name="section3369516103914"></a>

**响应示例**

```
{}
```

## 状态码<a name="section1037041673916"></a>

**表 3**  状态码

<a name="table937041613394"></a>
<table><thead align="left"><tr id="row11503184398"><th class="cellrowborder" valign="top" width="16.16%" id="mcps1.2.3.1.1"><p id="p1250118103916"><a name="p1250118103916"></a><a name="p1250118103916"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="83.84%" id="mcps1.2.3.1.2"><p id="p17503188398"><a name="p17503188398"></a><a name="p17503188398"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row115071823910"><td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.3.1.1 "><p id="p850131853916"><a name="p850131853916"></a><a name="p850131853916"></a>201</p>
</td>
<td class="cellrowborder" valign="top" width="83.84%" headers="mcps1.2.3.1.2 "><p id="p250151817393"><a name="p250151817393"></a><a name="p250151817393"></a>触发成功</p>
</td>
</tr>
<tr id="row145011181395"><td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.3.1.1 "><p id="p1650151810394"><a name="p1650151810394"></a><a name="p1650151810394"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="83.84%" headers="mcps1.2.3.1.2 "><p id="p1750181812394"><a name="p1750181812394"></a><a name="p1750181812394"></a>错误的请求</p>
</td>
</tr>
<tr id="row4501818193910"><td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.3.1.1 "><p id="p115011813398"><a name="p115011813398"></a><a name="p115011813398"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="83.84%" headers="mcps1.2.3.1.2 "><p id="p75041863916"><a name="p75041863916"></a><a name="p75041863916"></a>鉴权失败</p>
</td>
</tr>
<tr id="row15013188399"><td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.3.1.1 "><p id="p19501218143913"><a name="p19501218143913"></a><a name="p19501218143913"></a>409</p>
</td>
<td class="cellrowborder" valign="top" width="83.84%" headers="mcps1.2.3.1.2 "><p id="p750121817399"><a name="p750121817399"></a><a name="p750121817399"></a>已存在或超出每组户下可创建最大组织数</p>
</td>
</tr>
<tr id="row1950418133918"><td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.3.1.1 "><p id="p1550118103913"><a name="p1550118103913"></a><a name="p1550118103913"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="83.84%" headers="mcps1.2.3.1.2 "><p id="p1450111817392"><a name="p1450111817392"></a><a name="p1450111817392"></a>内部错误</p>
</td>
</tr>
</tbody>
</table>

