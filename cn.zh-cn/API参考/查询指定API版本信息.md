# 查询指定API版本信息<a name="swr_02_0081"></a>

## 功能介绍<a name="se03aae4436e64394a95dc13b6f233898"></a>

查询容器镜像服务指定API版本信息列表。

## URI<a name="s476df674307e4b04b9545f9575dde042"></a>

GET /\{api\_version\}

参数说明请参见[表1](#tae82a09e27434bef9a38b734d798ae6c)。

**表 1**  参数说明

<a name="tae82a09e27434bef9a38b734d798ae6c"></a>
<table><thead align="left"><tr id="r2c22eba22439445680961f8c447f8756"><th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.1"><p id="a4276374f4f884a1a8ff6eabdab4da030"><a name="a4276374f4f884a1a8ff6eabdab4da030"></a><a name="a4276374f4f884a1a8ff6eabdab4da030"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="p2011016570315"><a name="p2011016570315"></a><a name="p2011016570315"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="16%" id="mcps1.2.5.1.3"><p id="p537522204217"><a name="p537522204217"></a><a name="p537522204217"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0060210625_p192541611508"><a name="zh-cn_topic_0060210625_p192541611508"></a><a name="zh-cn_topic_0060210625_p192541611508"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row4140165617213"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.1 "><p id="p520212400161"><a name="p520212400161"></a><a name="p520212400161"></a>api_version</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p15117857734"><a name="p15117857734"></a><a name="p15117857734"></a><span>String</span></p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.3 "><p id="p20379152154213"><a name="p20379152154213"></a><a name="p20379152154213"></a><span>是</span></p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p219804051612"><a name="p219804051612"></a><a name="p219804051612"></a>API版本号。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息.<a name="s8246d3afdd6f44dc817ce0c3f2ac7d53"></a>

N/A

## 响应消息<a name="sab9be5ce850743859bb238e072f8d1f2"></a>

**响应参数**

**表 2**  Response Body参数说明

<a name="table183801055203619"></a>
<table><thead align="left"><tr id="row5381195513365"><th class="cellrowborder" valign="top" width="21.52215221522152%" id="mcps1.2.4.1.1"><p id="p1938145519369"><a name="p1938145519369"></a><a name="p1938145519369"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="19.65196519651965%" id="mcps1.2.4.1.2"><p id="p6381185513616"><a name="p6381185513616"></a><a name="p6381185513616"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="58.825882588258814%" id="mcps1.2.4.1.3"><p id="p93815559368"><a name="p93815559368"></a><a name="p93815559368"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row338165511364"><td class="cellrowborder" valign="top" width="21.52215221522152%" headers="mcps1.2.4.1.1 "><p id="p1838117551367"><a name="p1838117551367"></a><a name="p1838117551367"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="19.65196519651965%" headers="mcps1.2.4.1.2 "><p id="p1438112559365"><a name="p1438112559365"></a><a name="p1438112559365"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="58.825882588258814%" headers="mcps1.2.4.1.3 "><p id="p4381755113616"><a name="p4381755113616"></a><a name="p4381755113616"></a><span>描述</span><span>versio</span><span>n相关对象，详情请参见</span><a href="#table45446245174724">表3</a><span>。</span></p>
</td>
</tr>
</tbody>
</table>

**表 3**  version参数说明

<a name="table45446245174724"></a>
<table><thead align="left"><tr id="row1412623174724"><th class="cellrowborder" valign="top" width="21.52215221522152%" id="mcps1.2.4.1.1"><p id="p47313663174724"><a name="p47313663174724"></a><a name="p47313663174724"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="19.65196519651965%" id="mcps1.2.4.1.2"><p id="p7201512174724"><a name="p7201512174724"></a><a name="p7201512174724"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="58.825882588258814%" id="mcps1.2.4.1.3"><p id="p4480706174724"><a name="p4480706174724"></a><a name="p4480706174724"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row98876365819"><td class="cellrowborder" valign="top" width="21.52215221522152%" headers="mcps1.2.4.1.1 "><p id="p1440645517302"><a name="p1440645517302"></a><a name="p1440645517302"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="19.65196519651965%" headers="mcps1.2.4.1.2 "><p id="p540675519302"><a name="p540675519302"></a><a name="p540675519302"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.825882588258814%" headers="mcps1.2.4.1.3 "><p id="p15406115518308"><a name="p15406115518308"></a><a name="p15406115518308"></a>版本ID（版本号），如v2。</p>
</td>
</tr>
<tr id="row3367184810392"><td class="cellrowborder" valign="top" width="21.52215221522152%" headers="mcps1.2.4.1.1 "><p id="p14406755103013"><a name="p14406755103013"></a><a name="p14406755103013"></a>links</p>
</td>
<td class="cellrowborder" valign="top" width="19.65196519651965%" headers="mcps1.2.4.1.2 "><p id="p17406855153012"><a name="p17406855153012"></a><a name="p17406855153012"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.825882588258814%" headers="mcps1.2.4.1.3 "><p id="p13406195533010"><a name="p13406195533010"></a><a name="p13406195533010"></a>API的URL地址。</p>
</td>
</tr>
<tr id="row626682835815"><td class="cellrowborder" valign="top" width="21.52215221522152%" headers="mcps1.2.4.1.1 "><p id="p1891845543117"><a name="p1891845543117"></a><a name="p1891845543117"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="19.65196519651965%" headers="mcps1.2.4.1.2 "><p id="p1491805516316"><a name="p1491805516316"></a><a name="p1491805516316"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.825882588258814%" headers="mcps1.2.4.1.3 "><p id="p59181855123117"><a name="p59181855123117"></a><a name="p59181855123117"></a>若该版本API支持微版本，则填支持的最大微版本号，如果不支持微版本，则填空。</p>
</td>
</tr>
<tr id="row1272510338318"><td class="cellrowborder" valign="top" width="21.52215221522152%" headers="mcps1.2.4.1.1 "><p id="p69181655183119"><a name="p69181655183119"></a><a name="p69181655183119"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="19.65196519651965%" headers="mcps1.2.4.1.2 "><p id="p191855553110"><a name="p191855553110"></a><a name="p191855553110"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.825882588258814%" headers="mcps1.2.4.1.3 "><p id="p791815513111"><a name="p791815513111"></a><a name="p791815513111"></a>版本状态，为如下3种：</p>
<p id="p14919135517310"><a name="p14919135517310"></a><a name="p14919135517310"></a>CURRENT：表示该版本为主推版本；</p>
<p id="p169191555103116"><a name="p169191555103116"></a><a name="p169191555103116"></a>SUPPORTED：表示为老版本，但是现在还继续支持；</p>
<p id="p149191355173117"><a name="p149191355173117"></a><a name="p149191355173117"></a>DEPRECATED：表示为废弃版本，存在后续删除的可能。</p>
</td>
</tr>
<tr id="row11746173743119"><td class="cellrowborder" valign="top" width="21.52215221522152%" headers="mcps1.2.4.1.1 "><p id="p15919145533117"><a name="p15919145533117"></a><a name="p15919145533117"></a>updated</p>
</td>
<td class="cellrowborder" valign="top" width="19.65196519651965%" headers="mcps1.2.4.1.2 "><p id="p791917552312"><a name="p791917552312"></a><a name="p791917552312"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.825882588258814%" headers="mcps1.2.4.1.3 "><p id="p7919195503119"><a name="p7919195503119"></a><a name="p7919195503119"></a>版本发布时间，要求用UTC时间表示。如v1发布的时间2014-06-28T12:20:21Z。</p>
</td>
</tr>
<tr id="row14580164713313"><td class="cellrowborder" valign="top" width="21.52215221522152%" headers="mcps1.2.4.1.1 "><p id="p791995515312"><a name="p791995515312"></a><a name="p791995515312"></a>min_version</p>
</td>
<td class="cellrowborder" valign="top" width="19.65196519651965%" headers="mcps1.2.4.1.2 "><p id="p18919155511315"><a name="p18919155511315"></a><a name="p18919155511315"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.825882588258814%" headers="mcps1.2.4.1.3 "><p id="p6919195518313"><a name="p6919195518313"></a><a name="p6919195518313"></a>若该版本API 支持微版本，则填支持的最小微版本号， 如果不支持微版本，则填空。</p>
</td>
</tr>
</tbody>
</table>

**响应示例**

```
{
    "version": {
        "id": "v2",
        "links": [
            {
                "href": "https://swr-api.xxxx.myhuaweicloud.com/v2/",
                "rel": "self"
            }
        ],
        "min_version": "2.0",
        "status": "CURRENT",
        "updated": "2017-12-09T00:00:00Z",
        "version": "2.26"
    }
}
```

## 状态码<a name="s336c1dbc7af446a1b3cc077ea3f82fc9"></a>

状态码如[表4](#t33d02fa79e8443868a71c99f411610a5)所示。

**表 4**  状态码

<a name="t33d02fa79e8443868a71c99f411610a5"></a>
<table><thead align="left"><tr id="r9eb80d64e8f34d0db940daa95fc929dd"><th class="cellrowborder" valign="top" width="16.439999999999998%" id="mcps1.2.3.1.1"><p id="a7e51ed73a71e4dc29d0dd4aae3016632"><a name="a7e51ed73a71e4dc29d0dd4aae3016632"></a><a name="a7e51ed73a71e4dc29d0dd4aae3016632"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="83.56%" id="mcps1.2.3.1.2"><p id="aa802d02e21c944f1863435a0d11c7ec1"><a name="aa802d02e21c944f1863435a0d11c7ec1"></a><a name="aa802d02e21c944f1863435a0d11c7ec1"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="r1cc0192c651444db882dde750b14be23"><td class="cellrowborder" valign="top" width="16.439999999999998%" headers="mcps1.2.3.1.1 "><p id="a6a3639a3cb154e17b95c5076c8036471"><a name="a6a3639a3cb154e17b95c5076c8036471"></a><a name="a6a3639a3cb154e17b95c5076c8036471"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="83.56%" headers="mcps1.2.3.1.2 "><p id="p14504142233912"><a name="p14504142233912"></a><a name="p14504142233912"></a>请求成功</p>
</td>
</tr>
<tr id="r19bdef782c164c93917f897241e521f8"><td class="cellrowborder" valign="top" width="16.439999999999998%" headers="mcps1.2.3.1.1 "><p id="a7da68e311c0f4267bacf3cbdb71d1ead"><a name="a7da68e311c0f4267bacf3cbdb71d1ead"></a><a name="a7da68e311c0f4267bacf3cbdb71d1ead"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="83.56%" headers="mcps1.2.3.1.2 "><p id="aa6fd12cedd8841e29eeeca27c1bdea1a"><a name="aa6fd12cedd8841e29eeeca27c1bdea1a"></a><a name="aa6fd12cedd8841e29eeeca27c1bdea1a"></a>内部错误</p>
</td>
</tr>
</tbody>
</table>

