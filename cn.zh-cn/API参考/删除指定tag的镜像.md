# 删除指定tag的镜像<a name="swr_02_0036"></a>

## 功能介绍<a name="section14905762191056"></a>

删除镜像仓库中指定tag的镜像。

## 调试<a name="section85822133314"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=SWR&api=DeleteRepoTag)中直接运行调试该接口。

## URI<a name="section10482810165331"></a>

DELETE /v2/manage/namespaces/\{namespace\}/repos/\{repository\}/tags/\{tag\}

参数说明请参见[表1](#table05962819187)。

**表 1**  参数说明

<a name="table05962819187"></a>
<table><thead align="left"><tr id="row18599289181"><th class="cellrowborder" valign="top" width="18.92%" id="mcps1.2.5.1.1"><p id="p145942820183"><a name="p145942820183"></a><a name="p145942820183"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="16.150000000000002%" id="mcps1.2.5.1.2"><p id="p1450315424313"><a name="p1450315424313"></a><a name="p1450315424313"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.75%" id="mcps1.2.5.1.3"><p id="p15022419437"><a name="p15022419437"></a><a name="p15022419437"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="47.18%" id="mcps1.2.5.1.4"><p id="p205910283185"><a name="p205910283185"></a><a name="p205910283185"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row146018284188"><td class="cellrowborder" valign="top" width="18.92%" headers="mcps1.2.5.1.1 "><p id="p0601928131816"><a name="p0601928131816"></a><a name="p0601928131816"></a>namespace</p>
</td>
<td class="cellrowborder" valign="top" width="16.150000000000002%" headers="mcps1.2.5.1.2 "><p id="p10507114164313"><a name="p10507114164313"></a><a name="p10507114164313"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.75%" headers="mcps1.2.5.1.3 "><p id="p105058419438"><a name="p105058419438"></a><a name="p105058419438"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.18%" headers="mcps1.2.5.1.4 "><p id="p11460935127"><a name="p11460935127"></a><a name="p11460935127"></a>组织名称</p>
</td>
</tr>
<tr id="row1160152816186"><td class="cellrowborder" valign="top" width="18.92%" headers="mcps1.2.5.1.1 "><p id="p206018288188"><a name="p206018288188"></a><a name="p206018288188"></a>repository</p>
</td>
<td class="cellrowborder" valign="top" width="16.150000000000002%" headers="mcps1.2.5.1.2 "><p id="p18920840134520"><a name="p18920840134520"></a><a name="p18920840134520"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.75%" headers="mcps1.2.5.1.3 "><p id="p391915406456"><a name="p391915406456"></a><a name="p391915406456"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.18%" headers="mcps1.2.5.1.4 "><p id="p1871615462812"><a name="p1871615462812"></a><a name="p1871615462812"></a>镜像仓库名称</p>
</td>
</tr>
<tr id="row7611288187"><td class="cellrowborder" valign="top" width="18.92%" headers="mcps1.2.5.1.1 "><p id="p761728131819"><a name="p761728131819"></a><a name="p761728131819"></a>tag</p>
</td>
<td class="cellrowborder" valign="top" width="16.150000000000002%" headers="mcps1.2.5.1.2 "><p id="p923624264510"><a name="p923624264510"></a><a name="p923624264510"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.75%" headers="mcps1.2.5.1.3 "><p id="p623464254512"><a name="p623464254512"></a><a name="p623464254512"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.18%" headers="mcps1.2.5.1.4 "><p id="p371619413280"><a name="p371619413280"></a><a name="p371619413280"></a>镜像版本名称</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section3270966102931"></a>

-   请求参数

    无

-   请求样例

    ```
    DELETE https://{Endpoint}/v2/manage/namespaces/group/repos/busybox/tags/v1
    ```


## 响应消息<a name="section46271297104114"></a>

N/A

## 状态码<a name="section5365169104253"></a>

<a name="table334923162011"></a>
<table><thead align="left"><tr id="row834914392012"><th class="cellrowborder" valign="top" width="17.44%" id="mcps1.1.3.1.1"><p id="p1434911342014"><a name="p1434911342014"></a><a name="p1434911342014"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="82.56%" id="mcps1.1.3.1.2"><p id="p4349430208"><a name="p4349430208"></a><a name="p4349430208"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row5349837207"><td class="cellrowborder" valign="top" width="17.44%" headers="mcps1.1.3.1.1 "><p id="p834920312011"><a name="p834920312011"></a><a name="p834920312011"></a>204</p>
</td>
<td class="cellrowborder" valign="top" width="82.56%" headers="mcps1.1.3.1.2 "><p id="p4349113182014"><a name="p4349113182014"></a><a name="p4349113182014"></a>成功删除指定tag的镜像</p>
</td>
</tr>
<tr id="row53501322011"><td class="cellrowborder" valign="top" width="17.44%" headers="mcps1.1.3.1.1 "><p id="p23509352013"><a name="p23509352013"></a><a name="p23509352013"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="82.56%" headers="mcps1.1.3.1.2 "><p id="p83505352020"><a name="p83505352020"></a><a name="p83505352020"></a>错误请求，返回错误信息。</p>
</td>
</tr>
<tr id="row147214765819"><td class="cellrowborder" valign="top" width="17.44%" headers="mcps1.1.3.1.1 "><p id="p12314164419574"><a name="p12314164419574"></a><a name="p12314164419574"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="82.56%" headers="mcps1.1.3.1.2 "><p id="p93141244155715"><a name="p93141244155715"></a><a name="p93141244155715"></a>鉴权失败</p>
</td>
</tr>
<tr id="row187384312201"><td class="cellrowborder" valign="top" width="17.44%" headers="mcps1.1.3.1.1 "><p id="p11739731182020"><a name="p11739731182020"></a><a name="p11739731182020"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="82.56%" headers="mcps1.1.3.1.2 "><p id="p137391931122010"><a name="p137391931122010"></a><a name="p137391931122010"></a>repository不存在或指定的tag不存在</p>
</td>
</tr>
<tr id="row0350123192020"><td class="cellrowborder" valign="top" width="17.44%" headers="mcps1.1.3.1.1 "><p id="p335019311201"><a name="p335019311201"></a><a name="p335019311201"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="82.56%" headers="mcps1.1.3.1.2 "><p id="p43509342017"><a name="p43509342017"></a><a name="p43509342017"></a>服务器内部错误，返回错误信息。</p>
</td>
</tr>
</tbody>
</table>

