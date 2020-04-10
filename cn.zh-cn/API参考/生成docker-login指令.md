# 生成docker login指令<a name="swr_02_0052"></a>

## 功能介绍<a name="section14905762191056"></a>

调用该接口，通过获取响应消息头的X-Swr-Dockerlogin的值及响应消息体的host值，可生成docker login指令。

## URI<a name="section10482810165331"></a>

POST /v2/manage/utils/secret?projectname=\{projectname\}&ak=\{ak\}&sk=\{sk\}

参数说明请参见[表1](#table05962819187)。

**表 1**  参数说明

<a name="table05962819187"></a>
<table><thead align="left"><tr id="row18599289181"><th class="cellrowborder" valign="top" width="15.68%" id="mcps1.2.5.1.1"><p id="p145942820183"><a name="p145942820183"></a><a name="p145942820183"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="11.27%" id="mcps1.2.5.1.2"><p id="p1450315424313"><a name="p1450315424313"></a><a name="p1450315424313"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.06%" id="mcps1.2.5.1.3"><p id="p15022419437"><a name="p15022419437"></a><a name="p15022419437"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.989999999999995%" id="mcps1.2.5.1.4"><p id="p205910283185"><a name="p205910283185"></a><a name="p205910283185"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row146018284188"><td class="cellrowborder" valign="top" width="15.68%" headers="mcps1.2.5.1.1 "><p id="p10585203891316"><a name="p10585203891316"></a><a name="p10585203891316"></a>projectname</p>
</td>
<td class="cellrowborder" valign="top" width="11.27%" headers="mcps1.2.5.1.2 "><p id="p198322817174"><a name="p198322817174"></a><a name="p198322817174"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.06%" headers="mcps1.2.5.1.3 "><p id="p19795113419177"><a name="p19795113419177"></a><a name="p19795113419177"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.989999999999995%" headers="mcps1.2.5.1.4 "><p id="p1658514381137"><a name="p1658514381137"></a><a name="p1658514381137"></a>项目名称，缺省值默认为区域名称，例如：cn-north-1。</p>
</td>
</tr>
<tr id="row1160152816186"><td class="cellrowborder" valign="top" width="15.68%" headers="mcps1.2.5.1.1 "><p id="p6585438161310"><a name="p6585438161310"></a><a name="p6585438161310"></a>ak</p>
</td>
<td class="cellrowborder" valign="top" width="11.27%" headers="mcps1.2.5.1.2 "><p id="p81111128181719"><a name="p81111128181719"></a><a name="p81111128181719"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.06%" headers="mcps1.2.5.1.3 "><p id="p1079843413176"><a name="p1079843413176"></a><a name="p1079843413176"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.989999999999995%" headers="mcps1.2.5.1.4 "><p id="p16585203813139"><a name="p16585203813139"></a><a name="p16585203813139"></a>用户AK</p>
</td>
</tr>
<tr id="row7611288187"><td class="cellrowborder" valign="top" width="15.68%" headers="mcps1.2.5.1.1 "><p id="p6585103819131"><a name="p6585103819131"></a><a name="p6585103819131"></a>sk</p>
</td>
<td class="cellrowborder" valign="top" width="11.27%" headers="mcps1.2.5.1.2 "><p id="p11585113871314"><a name="p11585113871314"></a><a name="p11585113871314"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.06%" headers="mcps1.2.5.1.3 "><p id="p1880163431716"><a name="p1880163431716"></a><a name="p1880163431716"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.989999999999995%" headers="mcps1.2.5.1.4 "><p id="p10585133891316"><a name="p10585133891316"></a><a name="p10585133891316"></a>用户SK</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="s8246d3afdd6f44dc817ce0c3f2ac7d53"></a>

N/A

## 响应消息<a name="sab9be5ce850743859bb238e072f8d1f2"></a>

**响应参数**

**表 2**  Response Header参数说明

<a name="table1669936122412"></a>
<table><thead align="left"><tr id="row56991369241"><th class="cellrowborder" valign="top" width="20.89%" id="mcps1.2.4.1.1"><p id="p6699667249"><a name="p6699667249"></a><a name="p6699667249"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20.11%" id="mcps1.2.4.1.2"><p id="p269919620247"><a name="p269919620247"></a><a name="p269919620247"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="59%" id="mcps1.2.4.1.3"><p id="p166992061240"><a name="p166992061240"></a><a name="p166992061240"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row158942365248"><td class="cellrowborder" valign="top" width="20.89%" headers="mcps1.2.4.1.1 "><p id="p1389423616246"><a name="p1389423616246"></a><a name="p1389423616246"></a>X-Swr-Dockerlogin</p>
</td>
<td class="cellrowborder" valign="top" width="20.11%" headers="mcps1.2.4.1.2 "><p id="p195980421242"><a name="p195980421242"></a><a name="p195980421242"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="59%" headers="mcps1.2.4.1.3 "><p id="p759819427240"><a name="p759819427240"></a><a name="p759819427240"></a>docker login登录指令，例如：docker login -u cn-north-1@OW******FPUKBXI -p 6f0779072******863d1ae3ccef921b7f33</p>
</td>
</tr>
</tbody>
</table>

**表 3**  Response Body参数说明

<a name="table34001413863"></a>
<table><thead align="left"><tr id="row17400171319612"><th class="cellrowborder" valign="top" width="20.89%" id="mcps1.2.4.1.1"><p id="p1840015139619"><a name="p1840015139619"></a><a name="p1840015139619"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20.11%" id="mcps1.2.4.1.2"><p id="p24002135620"><a name="p24002135620"></a><a name="p24002135620"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="59%" id="mcps1.2.4.1.3"><p id="p174008131163"><a name="p174008131163"></a><a name="p174008131163"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row11400113668"><td class="cellrowborder" valign="top" width="20.89%" headers="mcps1.2.4.1.1 "><p id="p1348353715289"><a name="p1348353715289"></a><a name="p1348353715289"></a>auths</p>
</td>
<td class="cellrowborder" valign="top" width="20.11%" headers="mcps1.2.4.1.2 "><p id="p114831837142811"><a name="p114831837142811"></a><a name="p114831837142811"></a>Map&lt;String, <a href="#table1787854911167">authInfo</a>&gt;</p>
</td>
<td class="cellrowborder" valign="top" width="59%" headers="mcps1.2.4.1.3 "><p id="p74838372289"><a name="p74838372289"></a><a name="p74838372289"></a>认证信息</p>
</td>
</tr>
</tbody>
</table>

**表 4**  authInfo参数说明

<a name="table1787854911167"></a>
<table><thead align="left"><tr id="row1588184916165"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.4.1.1"><p id="p158847496166"><a name="p158847496166"></a><a name="p158847496166"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p2088624911169"><a name="p2088624911169"></a><a name="p2088624911169"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="59%" id="mcps1.2.4.1.3"><p id="p128875496169"><a name="p128875496169"></a><a name="p128875496169"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row888994917169"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.1 "><p id="p1142716375293"><a name="p1142716375293"></a><a name="p1142716375293"></a>auth</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p642773742911"><a name="p642773742911"></a><a name="p642773742911"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="59%" headers="mcps1.2.4.1.3 "><p id="p194274374297"><a name="p194274374297"></a><a name="p194274374297"></a>Base64加密的认证信息</p>
</td>
</tr>
</tbody>
</table>

**响应示例**

```
{
    "auths": {
        "10.95.181.176:5300": {
            "auth": "Y24tbm9ydGg******hhMTgzMGVmN2RhZjJm"
        }
    }
}
```

通过获取响应消息头的X-Swr-Dockerlogin的值及响应消息体的host值，可生成docker login指令。

例如：上述响应示例中，响应消息头的X-Swr-Dockerlogin的值为“docker login -u cn-north-1@OW\*\*\*\*\*\*FPUKBXI -p 6f0779072\*\*\*\*\*\*863d1ae3ccef921b7f33”，响应消息体的host值为“10.95.181.176:5300”，则生成的docker login指令为 ：

**docker login -u cn-north-1@OW\*\*\*\*\*\*FPUKBXI -p 6f0779072\*\*\*\*\*\*863d1ae3ccef921b7f33 10.95.181.176:5300**

## 状态码<a name="section5365169104253"></a>

状态码如[表5](#table334923162011)所示。

**表 5**  状态码

<a name="table334923162011"></a>
<table><thead align="left"><tr id="row834914392012"><th class="cellrowborder" valign="top" width="17.44%" id="mcps1.2.3.1.1"><p id="p1434911342014"><a name="p1434911342014"></a><a name="p1434911342014"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="82.56%" id="mcps1.2.3.1.2"><p id="p4349430208"><a name="p4349430208"></a><a name="p4349430208"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row5349837207"><td class="cellrowborder" valign="top" width="17.44%" headers="mcps1.2.3.1.1 "><p id="p47673018306"><a name="p47673018306"></a><a name="p47673018306"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="82.56%" headers="mcps1.2.3.1.2 "><p id="p1976173053010"><a name="p1976173053010"></a><a name="p1976173053010"></a>请求成功。</p>
</td>
</tr>
<tr id="row53501322011"><td class="cellrowborder" valign="top" width="17.44%" headers="mcps1.2.3.1.1 "><p id="p2761304301"><a name="p2761304301"></a><a name="p2761304301"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="82.56%" headers="mcps1.2.3.1.2 "><p id="p876530153011"><a name="p876530153011"></a><a name="p876530153011"></a>错误请求，返回错误信息。</p>
</td>
</tr>
<tr id="row187384312201"><td class="cellrowborder" valign="top" width="17.44%" headers="mcps1.2.3.1.1 "><p id="p97613012308"><a name="p97613012308"></a><a name="p97613012308"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="82.56%" headers="mcps1.2.3.1.2 "><p id="p117673023012"><a name="p117673023012"></a><a name="p117673023012"></a>鉴权失败的报错信息。</p>
</td>
</tr>
<tr id="row0350123192020"><td class="cellrowborder" valign="top" width="17.44%" headers="mcps1.2.3.1.1 "><p id="p976113012309"><a name="p976113012309"></a><a name="p976113012309"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="82.56%" headers="mcps1.2.3.1.2 "><p id="p107633093012"><a name="p107633093012"></a><a name="p107633093012"></a>服务器内部错误，返回错误信息。</p>
</td>
</tr>
</tbody>
</table>

