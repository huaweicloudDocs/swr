# 删除指定tag的镜像<a name="swr_02_0036"></a>

## 功能介绍<a name="section14905762191056"></a>

删除镜像仓库中指定tag的镜像。

## URI<a name="section10482810165331"></a>

DELETE /v2/manage/namespaces/\{namespace\}/repos/\{repository\}/tags/\{tag\}

参数说明请参见[表1](#table05962819187)。

**表 1**  参数说明

<a name="table05962819187"></a>
<table><thead align="left"><tr id="row18599289181"><th class="cellrowborder" valign="top" width="32.29%" id="mcps1.2.4.1.1"><p id="p145942820183"><a name="p145942820183"></a><a name="p145942820183"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="24.14%" id="mcps1.2.4.1.2"><p id="p2412385190"><a name="p2412385190"></a><a name="p2412385190"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="43.57%" id="mcps1.2.4.1.3"><p id="p205910283185"><a name="p205910283185"></a><a name="p205910283185"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row146018284188"><td class="cellrowborder" valign="top" width="32.29%" headers="mcps1.2.4.1.1 "><p id="p0601928131816"><a name="p0601928131816"></a><a name="p0601928131816"></a>namespace</p>
</td>
<td class="cellrowborder" valign="top" width="24.14%" headers="mcps1.2.4.1.2 "><p id="p1541218191918"><a name="p1541218191918"></a><a name="p1541218191918"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="43.57%" headers="mcps1.2.4.1.3 "><p id="p1960112891813"><a name="p1960112891813"></a><a name="p1960112891813"></a>命名空间名称，只支持大小写字母开头，后面跟大小写字母、数字、下划线或横线，1-255个字符</p>
</td>
</tr>
<tr id="row1160152816186"><td class="cellrowborder" valign="top" width="32.29%" headers="mcps1.2.4.1.1 "><p id="p206018288188"><a name="p206018288188"></a><a name="p206018288188"></a>repository</p>
</td>
<td class="cellrowborder" valign="top" width="24.14%" headers="mcps1.2.4.1.2 "><p id="p5412986190"><a name="p5412986190"></a><a name="p5412986190"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="43.57%" headers="mcps1.2.4.1.3 "><p id="p11611528111811"><a name="p11611528111811"></a><a name="p11611528111811"></a>repository名称，仅支持大小写字母或数字开头，后面跟大小写字母、数字、下划线或横线，1-255个字符</p>
</td>
</tr>
<tr id="row7611288187"><td class="cellrowborder" valign="top" width="32.29%" headers="mcps1.2.4.1.1 "><p id="p761728131819"><a name="p761728131819"></a><a name="p761728131819"></a>tag</p>
</td>
<td class="cellrowborder" valign="top" width="24.14%" headers="mcps1.2.4.1.2 "><p id="p441212891913"><a name="p441212891913"></a><a name="p441212891913"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="43.57%" headers="mcps1.2.4.1.3 "><p id="p261202814184"><a name="p261202814184"></a><a name="p261202814184"></a>数字、字母或下划线开头，后面跟数字、字母、下划线、点、短横线，最长128个字符</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section3270966102931"></a>

N/A。

## 响应消息<a name="section46271297104114"></a>

N/A。

## 状态码<a name="section5365169104253"></a>

状态码如[表2](#table334923162011)所示。

**表 2**  状态码

<a name="table334923162011"></a>
<table><thead align="left"><tr id="row834914392012"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="p1434911342014"><a name="p1434911342014"></a><a name="p1434911342014"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="p4349430208"><a name="p4349430208"></a><a name="p4349430208"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row5349837207"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p834920312011"><a name="p834920312011"></a><a name="p834920312011"></a>204</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p4349113182014"><a name="p4349113182014"></a><a name="p4349113182014"></a>成功删除tag指定的镜像。</p>
</td>
</tr>
<tr id="row53501322011"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p23509352013"><a name="p23509352013"></a><a name="p23509352013"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p83505352020"><a name="p83505352020"></a><a name="p83505352020"></a>错误请求，返回错误信息。</p>
</td>
</tr>
<tr id="row187384312201"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p11739731182020"><a name="p11739731182020"></a><a name="p11739731182020"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p137391931122010"><a name="p137391931122010"></a><a name="p137391931122010"></a>repository不存在或指定的tag不存在。</p>
</td>
</tr>
<tr id="row0350123192020"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p335019311201"><a name="p335019311201"></a><a name="p335019311201"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p43509342017"><a name="p43509342017"></a><a name="p43509342017"></a>服务器内部错误，返回错误信息。</p>
</td>
</tr>
</tbody>
</table>

