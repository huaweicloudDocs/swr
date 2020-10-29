# 查询所有API版本信息<a name="swr_02_0080"></a>

## 功能介绍<a name="se03aae4436e64394a95dc13b6f233898"></a>

查询容器镜像服务所有可用的API版本信息列表。

## URI<a name="s476df674307e4b04b9545f9575dde042"></a>

GET /

## 请求消息<a name="s8246d3afdd6f44dc817ce0c3f2ac7d53"></a>

N/A

## 响应消息<a name="sab9be5ce850743859bb238e072f8d1f2"></a>

**响应参数**

**表 1**  Response Body参数说明

<a name="table1585555623716"></a>
<table><thead align="left"><tr id="row18561356203713"><th class="cellrowborder" valign="top" width="21.52215221522152%" id="mcps1.2.4.1.1"><p id="p20856135619375"><a name="p20856135619375"></a><a name="p20856135619375"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="19.65196519651965%" id="mcps1.2.4.1.2"><p id="p3856105610372"><a name="p3856105610372"></a><a name="p3856105610372"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="58.825882588258814%" id="mcps1.2.4.1.3"><p id="p6856956203719"><a name="p6856956203719"></a><a name="p6856956203719"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row18561356173718"><td class="cellrowborder" valign="top" width="21.52215221522152%" headers="mcps1.2.4.1.1 "><p id="p1985685653718"><a name="p1985685653718"></a><a name="p1985685653718"></a>versions</p>
</td>
<td class="cellrowborder" valign="top" width="19.65196519651965%" headers="mcps1.2.4.1.2 "><p id="p585645612379"><a name="p585645612379"></a><a name="p585645612379"></a>Array of objects</p>
</td>
<td class="cellrowborder" valign="top" width="58.825882588258814%" headers="mcps1.2.4.1.3 "><p id="p28568564370"><a name="p28568564370"></a><a name="p28568564370"></a><span>描述</span><span>version</span><span>相关对象的列表，详情请参见</span><a href="#table45446245174724">表2</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 2**  versions参数说明

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
<td class="cellrowborder" valign="top" width="58.825882588258814%" headers="mcps1.2.4.1.3 "><p id="p15406115518308"><a name="p15406115518308"></a><a name="p15406115518308"></a><span>版本</span>ID<span>（版本号），如</span><span>v2</span>。</p>
</td>
</tr>
<tr id="row3367184810392"><td class="cellrowborder" valign="top" width="21.52215221522152%" headers="mcps1.2.4.1.1 "><p id="p14406755103013"><a name="p14406755103013"></a><a name="p14406755103013"></a>links</p>
</td>
<td class="cellrowborder" valign="top" width="19.65196519651965%" headers="mcps1.2.4.1.2 "><p id="p17406855153012"><a name="p17406855153012"></a><a name="p17406855153012"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.825882588258814%" headers="mcps1.2.4.1.3 "><p id="p13406195533010"><a name="p13406195533010"></a><a name="p13406195533010"></a>API<span>的</span>URL<span>地址</span>，详情请参见<a href="#table453717423323">表3</a>。</p>
</td>
</tr>
<tr id="row626682835815"><td class="cellrowborder" valign="top" width="21.52215221522152%" headers="mcps1.2.4.1.1 "><p id="p1891845543117"><a name="p1891845543117"></a><a name="p1891845543117"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="19.65196519651965%" headers="mcps1.2.4.1.2 "><p id="p1491805516316"><a name="p1491805516316"></a><a name="p1491805516316"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.825882588258814%" headers="mcps1.2.4.1.3 "><p id="p59181855123117"><a name="p59181855123117"></a><a name="p59181855123117"></a><span>若该版本</span>API<span>支持微版本，则填支持的最大微版本号，如果不支持微版本，则填空</span>。</p>
</td>
</tr>
<tr id="row1272510338318"><td class="cellrowborder" valign="top" width="21.52215221522152%" headers="mcps1.2.4.1.1 "><p id="p69181655183119"><a name="p69181655183119"></a><a name="p69181655183119"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="19.65196519651965%" headers="mcps1.2.4.1.2 "><p id="p191855553110"><a name="p191855553110"></a><a name="p191855553110"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.825882588258814%" headers="mcps1.2.4.1.3 "><p id="p791815513111"><a name="p791815513111"></a><a name="p791815513111"></a><span>版本状态，为如下</span><span>3</span><span>种：</span></p>
<p id="p14919135517310"><a name="p14919135517310"></a><a name="p14919135517310"></a><span>CURRENT</span><span>：表示该版本为主推版本</span>；</p>
<p id="p169191555103116"><a name="p169191555103116"></a><a name="p169191555103116"></a><span>SUPPORTED</span><span>：表示为老版本，但是现在还继续支持</span>；</p>
<p id="p149191355173117"><a name="p149191355173117"></a><a name="p149191355173117"></a><span>DEPRECATED</span><span>：表示为废弃版本，存在后续删除的可能</span>。</p>
</td>
</tr>
<tr id="row11746173743119"><td class="cellrowborder" valign="top" width="21.52215221522152%" headers="mcps1.2.4.1.1 "><p id="p15919145533117"><a name="p15919145533117"></a><a name="p15919145533117"></a>updated</p>
</td>
<td class="cellrowborder" valign="top" width="19.65196519651965%" headers="mcps1.2.4.1.2 "><p id="p791917552312"><a name="p791917552312"></a><a name="p791917552312"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.825882588258814%" headers="mcps1.2.4.1.3 "><p id="p7919195503119"><a name="p7919195503119"></a><a name="p7919195503119"></a><span>版本发布时间，要求用</span><span>UTC</span><span>时间表示。</span>如v1发布的时间2014-06-28T12:20:21Z。</p>
</td>
</tr>
<tr id="row14580164713313"><td class="cellrowborder" valign="top" width="21.52215221522152%" headers="mcps1.2.4.1.1 "><p id="p791995515312"><a name="p791995515312"></a><a name="p791995515312"></a>min_version</p>
</td>
<td class="cellrowborder" valign="top" width="19.65196519651965%" headers="mcps1.2.4.1.2 "><p id="p18919155511315"><a name="p18919155511315"></a><a name="p18919155511315"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.825882588258814%" headers="mcps1.2.4.1.3 "><p id="p6919195518313"><a name="p6919195518313"></a><a name="p6919195518313"></a><span>若该版本</span>API <span>支持微版本，则填支持的最小微版本号，</span> <span>如果不支持微版本，则填空</span>。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  links参数说明

<a name="table453717423323"></a>
<table><thead align="left"><tr id="row1553720421323"><th class="cellrowborder" valign="top" width="21.52215221522152%" id="mcps1.2.4.1.1"><p id="p1553744263216"><a name="p1553744263216"></a><a name="p1553744263216"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="19.65196519651965%" id="mcps1.2.4.1.2"><p id="p15379427326"><a name="p15379427326"></a><a name="p15379427326"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="58.825882588258814%" id="mcps1.2.4.1.3"><p id="p10537134212325"><a name="p10537134212325"></a><a name="p10537134212325"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row45372426327"><td class="cellrowborder" valign="top" width="21.52215221522152%" headers="mcps1.2.4.1.1 "><p id="p9537194253219"><a name="p9537194253219"></a><a name="p9537194253219"></a>href</p>
</td>
<td class="cellrowborder" valign="top" width="19.65196519651965%" headers="mcps1.2.4.1.2 "><p id="p1753864273219"><a name="p1753864273219"></a><a name="p1753864273219"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.825882588258814%" headers="mcps1.2.4.1.3 "><p id="p2053834210320"><a name="p2053834210320"></a><a name="p2053834210320"></a>链接</p>
</td>
</tr>
<tr id="row125383424322"><td class="cellrowborder" valign="top" width="21.52215221522152%" headers="mcps1.2.4.1.1 "><p id="p15387424321"><a name="p15387424321"></a><a name="p15387424321"></a>rel</p>
</td>
<td class="cellrowborder" valign="top" width="19.65196519651965%" headers="mcps1.2.4.1.2 "><p id="p05381842163219"><a name="p05381842163219"></a><a name="p05381842163219"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.825882588258814%" headers="mcps1.2.4.1.3 "><p id="p5538144212329"><a name="p5538144212329"></a><a name="p5538144212329"></a>描述</p>
</td>
</tr>
</tbody>
</table>

**响应示例**

```
{ 
   "versions": [
        {
            "id": "v2",
            "links": 
                {
                    "href": "https://swr-api.xxxx.myhuaweicloud.com/v2/",
                    "rel": "self"
                }
            "min_version": "2.0",
            "status": "CURRENT",
            "updated": "2020-07-09T00:00:00Z",
            "version": "2.26",
        }
    ]

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

