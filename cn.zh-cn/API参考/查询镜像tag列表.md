# 查询镜像tag列表<a name="swr_02_0035"></a>

## 功能介绍<a name="section14905762191056"></a>

获取镜像的tag的列表。

## URI<a name="section10482810165331"></a>

GET /v2/manage/namespaces/\{namespace\}/repos/\{repository\}/tags

参数说明请参见[表1](#table11843162810214)。

**表 1**  参数说明

<a name="table11843162810214"></a>
<table><thead align="left"><tr id="row20843172818213"><th class="cellrowborder" valign="top" width="30.61%" id="mcps1.2.4.1.1"><p id="p3843528621"><a name="p3843528621"></a><a name="p3843528621"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="33.4%" id="mcps1.2.4.1.2"><p id="p1384319283210"><a name="p1384319283210"></a><a name="p1384319283210"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="35.99%" id="mcps1.2.4.1.3"><p id="p1584342811211"><a name="p1584342811211"></a><a name="p1584342811211"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1084316281925"><td class="cellrowborder" valign="top" width="30.61%" headers="mcps1.2.4.1.1 "><p id="p6843228526"><a name="p6843228526"></a><a name="p6843228526"></a>namespace</p>
</td>
<td class="cellrowborder" valign="top" width="33.4%" headers="mcps1.2.4.1.2 "><p id="p284310281826"><a name="p284310281826"></a><a name="p284310281826"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="35.99%" headers="mcps1.2.4.1.3 "><p id="p85037015469"><a name="p85037015469"></a><a name="p85037015469"></a>组织名称</p>
</td>
</tr>
<tr id="row1319321944420"><td class="cellrowborder" valign="top" width="30.61%" headers="mcps1.2.4.1.1 "><p id="p919315194441"><a name="p919315194441"></a><a name="p919315194441"></a>repository</p>
</td>
<td class="cellrowborder" valign="top" width="33.4%" headers="mcps1.2.4.1.2 "><p id="p17193161964410"><a name="p17193161964410"></a><a name="p17193161964410"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="35.99%" headers="mcps1.2.4.1.3 "><p id="p13193201924411"><a name="p13193201924411"></a><a name="p13193201924411"></a>镜像仓库名称</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section3270966102931"></a>

N/A。

## 响应消息<a name="section1262713444552"></a>

**响应参数**

响应参数如[表2](#table45446245174724)所示。

**表 2**  响应参数

<a name="table45446245174724"></a>
<table><thead align="left"><tr id="row1412623174724"><th class="cellrowborder" valign="top" width="34.616538346165385%" id="mcps1.2.4.1.1"><p id="p47313663174724"><a name="p47313663174724"></a><a name="p47313663174724"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="30.76692330766923%" id="mcps1.2.4.1.2"><p id="p7201512174724"><a name="p7201512174724"></a><a name="p7201512174724"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="34.616538346165385%" id="mcps1.2.4.1.3"><p id="p4480706174724"><a name="p4480706174724"></a><a name="p4480706174724"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row23391130131913"><td class="cellrowborder" valign="top" width="34.616538346165385%" headers="mcps1.2.4.1.1 "><p id="p43401630141910"><a name="p43401630141910"></a><a name="p43401630141910"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="30.76692330766923%" headers="mcps1.2.4.1.2 "><p id="p203401530111912"><a name="p203401530111912"></a><a name="p203401530111912"></a>int64</p>
</td>
<td class="cellrowborder" valign="top" width="34.616538346165385%" headers="mcps1.2.4.1.3 "><p id="p20340730191918"><a name="p20340730191918"></a><a name="p20340730191918"></a>编号</p>
</td>
</tr>
<tr id="row697982791918"><td class="cellrowborder" valign="top" width="34.616538346165385%" headers="mcps1.2.4.1.1 "><p id="p10980112717192"><a name="p10980112717192"></a><a name="p10980112717192"></a>repo_id</p>
</td>
<td class="cellrowborder" valign="top" width="30.76692330766923%" headers="mcps1.2.4.1.2 "><p id="p20980132718193"><a name="p20980132718193"></a><a name="p20980132718193"></a>int64</p>
</td>
<td class="cellrowborder" valign="top" width="34.616538346165385%" headers="mcps1.2.4.1.3 "><p id="p14980192714197"><a name="p14980192714197"></a><a name="p14980192714197"></a>仓库编号</p>
</td>
</tr>
<tr id="row17668249354"><td class="cellrowborder" valign="top" width="34.616538346165385%" headers="mcps1.2.4.1.1 "><p id="p3602231570"><a name="p3602231570"></a><a name="p3602231570"></a>Tag</p>
</td>
<td class="cellrowborder" valign="top" width="30.76692330766923%" headers="mcps1.2.4.1.2 "><p id="p360215315712"><a name="p360215315712"></a><a name="p360215315712"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="34.616538346165385%" headers="mcps1.2.4.1.3 "><p id="p206025311878"><a name="p206025311878"></a><a name="p206025311878"></a>Tag版本名称。</p>
</td>
</tr>
<tr id="row176816213207"><td class="cellrowborder" valign="top" width="34.616538346165385%" headers="mcps1.2.4.1.1 "><p id="p1568212212204"><a name="p1568212212204"></a><a name="p1568212212204"></a>image_id</p>
</td>
<td class="cellrowborder" valign="top" width="30.76692330766923%" headers="mcps1.2.4.1.2 "><p id="p1568252172015"><a name="p1568252172015"></a><a name="p1568252172015"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="34.616538346165385%" headers="mcps1.2.4.1.3 "><p id="p1968202192013"><a name="p1968202192013"></a><a name="p1968202192013"></a>镜像id</p>
</td>
</tr>
<tr id="row2590104211156"><td class="cellrowborder" valign="top" width="34.616538346165385%" headers="mcps1.2.4.1.1 "><p id="p1592204251517"><a name="p1592204251517"></a><a name="p1592204251517"></a>manifest</p>
</td>
<td class="cellrowborder" valign="top" width="30.76692330766923%" headers="mcps1.2.4.1.2 "><p id="p95921422152"><a name="p95921422152"></a><a name="p95921422152"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="34.616538346165385%" headers="mcps1.2.4.1.3 "><p id="p145923427155"><a name="p145923427155"></a><a name="p145923427155"></a>镜像manifest</p>
</td>
</tr>
<tr id="row411720412429"><td class="cellrowborder" valign="top" width="34.616538346165385%" headers="mcps1.2.4.1.1 "><p id="p8361449104214"><a name="p8361449104214"></a><a name="p8361449104214"></a>digest</p>
</td>
<td class="cellrowborder" valign="top" width="30.76692330766923%" headers="mcps1.2.4.1.2 "><p id="p103631149164219"><a name="p103631149164219"></a><a name="p103631149164219"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="34.616538346165385%" headers="mcps1.2.4.1.3 "><p id="p33651491427"><a name="p33651491427"></a><a name="p33651491427"></a>镜像hash值</p>
</td>
</tr>
<tr id="row19747155313423"><td class="cellrowborder" valign="top" width="34.616538346165385%" headers="mcps1.2.4.1.1 "><p id="p55111044437"><a name="p55111044437"></a><a name="p55111044437"></a>schema</p>
</td>
<td class="cellrowborder" valign="top" width="30.76692330766923%" headers="mcps1.2.4.1.2 "><p id="p65137412431"><a name="p65137412431"></a><a name="p65137412431"></a>int64</p>
</td>
<td class="cellrowborder" valign="top" width="34.616538346165385%" headers="mcps1.2.4.1.3 "><p id="p05141147434"><a name="p05141147434"></a><a name="p05141147434"></a>docker协议版本，值为1或2。</p>
</td>
</tr>
<tr id="row27392900174724"><td class="cellrowborder" valign="top" width="34.616538346165385%" headers="mcps1.2.4.1.1 "><p id="p66029311173"><a name="p66029311173"></a><a name="p66029311173"></a>path</p>
</td>
<td class="cellrowborder" valign="top" width="30.76692330766923%" headers="mcps1.2.4.1.2 "><p id="p460211311279"><a name="p460211311279"></a><a name="p460211311279"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="34.616538346165385%" headers="mcps1.2.4.1.3 "><p id="p9603163112712"><a name="p9603163112712"></a><a name="p9603163112712"></a>镜像pull地址，格式为</p>
<p id="p8659141362"><a name="p8659141362"></a><a name="p8659141362"></a>swr.cn-north-1.myhuaweicloud.com/namespace/repository:tag。</p>
</td>
</tr>
<tr id="row207081451715"><td class="cellrowborder" valign="top" width="34.616538346165385%" headers="mcps1.2.4.1.1 "><p id="p1701714191712"><a name="p1701714191712"></a><a name="p1701714191712"></a>internal_path</p>
</td>
<td class="cellrowborder" valign="top" width="30.76692330766923%" headers="mcps1.2.4.1.2 "><p id="p470314161716"><a name="p470314161716"></a><a name="p470314161716"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="34.616538346165385%" headers="mcps1.2.4.1.3 "><p id="p07051481718"><a name="p07051481718"></a><a name="p07051481718"></a>cce集群内镜像pull路径，格式为 10.125.0.198:20202/namespace/repository:tag</p>
</td>
</tr>
<tr id="row12917712114013"><td class="cellrowborder" valign="top" width="34.616538346165385%" headers="mcps1.2.4.1.1 "><p id="p15603531879"><a name="p15603531879"></a><a name="p15603531879"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="30.76692330766923%" headers="mcps1.2.4.1.2 "><p id="p1760318310710"><a name="p1760318310710"></a><a name="p1760318310710"></a>int64</p>
</td>
<td class="cellrowborder" valign="top" width="34.616538346165385%" headers="mcps1.2.4.1.3 "><p id="p136038314714"><a name="p136038314714"></a><a name="p136038314714"></a>镜像大小，0 ~ 9223372036854775807。</p>
</td>
</tr>
<tr id="row6189161112289"><td class="cellrowborder" valign="top" width="34.616538346165385%" headers="mcps1.2.4.1.1 "><p id="p519041132810"><a name="p519041132810"></a><a name="p519041132810"></a>is_trusted</p>
</td>
<td class="cellrowborder" valign="top" width="30.76692330766923%" headers="mcps1.2.4.1.2 "><p id="p1119014117288"><a name="p1119014117288"></a><a name="p1119014117288"></a>bool</p>
</td>
<td class="cellrowborder" valign="top" width="34.616538346165385%" headers="mcps1.2.4.1.3 "><p id="p13191811182818"><a name="p13191811182818"></a><a name="p13191811182818"></a>默认值为false</p>
</td>
</tr>
<tr id="row24091911193911"><td class="cellrowborder" valign="top" width="34.616538346165385%" headers="mcps1.2.4.1.1 "><p id="p13603531378"><a name="p13603531378"></a><a name="p13603531378"></a>created</p>
</td>
<td class="cellrowborder" valign="top" width="30.76692330766923%" headers="mcps1.2.4.1.2 "><p id="p660333115711"><a name="p660333115711"></a><a name="p660333115711"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="34.616538346165385%" headers="mcps1.2.4.1.3 "><p id="p760315313710"><a name="p760315313710"></a><a name="p760315313710"></a>镜像创建时间，UTC时间格式，时间为UTC标准时间，用户需要根据本地时间计算偏移量；如东8区需要+8:00</p>
</td>
</tr>
<tr id="row10790853193918"><td class="cellrowborder" valign="top" width="34.616538346165385%" headers="mcps1.2.4.1.1 "><p id="p14603631778"><a name="p14603631778"></a><a name="p14603631778"></a>updated</p>
</td>
<td class="cellrowborder" valign="top" width="30.76692330766923%" headers="mcps1.2.4.1.2 "><p id="p3603203112717"><a name="p3603203112717"></a><a name="p3603203112717"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="34.616538346165385%" headers="mcps1.2.4.1.3 "><p id="p1360316317716"><a name="p1360316317716"></a><a name="p1360316317716"></a>镜像更新时间，UTC时间格式，时间为UTC标准时间，用户需要根据本地时间计算偏移量；如东8区需要+8:00</p>
</td>
</tr>
<tr id="row1627112185506"><td class="cellrowborder" valign="top" width="34.616538346165385%" headers="mcps1.2.4.1.1 "><p id="p427119188502"><a name="p427119188502"></a><a name="p427119188502"></a>deleted</p>
</td>
<td class="cellrowborder" valign="top" width="30.76692330766923%" headers="mcps1.2.4.1.2 "><p id="p142711318125017"><a name="p142711318125017"></a><a name="p142711318125017"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="34.616538346165385%" headers="mcps1.2.4.1.3 "><p id="p1327116186505"><a name="p1327116186505"></a><a name="p1327116186505"></a>镜像删除时间</p>
</td>
</tr>
</tbody>
</table>

**响应示例**

```


[{

    "id": 0,
    "repo_id": 0,
    "Tag": "latest",
    "image_id": "741f24a795d6d93d7c6edd11780d63c13e16c39615dd9d223378a57a836f2ee6",
    "manifest": "{\"schemaVersion\":2,\"mediaType\":\"application/vnd.docker.distribution.manifest.v2+json\",\"config\":{\"mediaType\":\"application/vnd.docker.container.image.v1+json\",\"size\":1862,\"digest\":\"sha256:741f24a795d6d93d7c6edd11780d63c13e16c39615dd9d223378a57a836f2ee6\"},\"layers\":[{\"mediaType\":\"application/vnd.docker.image.rootfs.diff.tar.gzip\",\"size\":1292800,\"digest\":\"sha256:8ac8bfaff55af948c796026ee867448c5b5b5d9dd3549f4006d9759b25d4a893\"},{\"mediaType\":\"application/vnd.docker.image.rootfs.diff.tar.gzip\",\"size\":10240,\"digest\":\"sha256:77ddbf3a9fe11e81761a0f9df43a28e3e6f29bbb53c0c8cf71cd7efa69729aed\"}]}",
    "digest": "sha256:57b605845a6367c34bfb6ea6477f16852f59aa1861a2b51d10ab77ae0a1dc9c3",
    "schema": 2,
    "path": "swr.cn-north-1.myhuaweicloud.com/namespace/busybox:latest",
    "internal_path": "10.125.0.198:20202/namespace/busybox:latest",
    "size": 1304902,
    "is_trusted": false,
    "created": "2018-07-06T06:18:55Z",
    "updated": "2018-07-06T06:18:55Z",
    "deleted": null
}]

```

## 状态码<a name="section5365169104253"></a>

状态码如[表3](#table1984564864716)所示。

**表 3**  状态码

<a name="table1984564864716"></a>
<table><thead align="left"><tr id="row1984554824718"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="p4846548124714"><a name="p4846548124714"></a><a name="p4846548124714"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="p984612486479"><a name="p984612486479"></a><a name="p984612486479"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1484619482477"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p88461948154710"><a name="p88461948154710"></a><a name="p88461948154710"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p13846748154710"><a name="p13846748154710"></a><a name="p13846748154710"></a>成功查询镜像仓库的所有tag。</p>
</td>
</tr>
<tr id="row98468489472"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p14846134812476"><a name="p14846134812476"></a><a name="p14846134812476"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p08461448114716"><a name="p08461448114716"></a><a name="p08461448114716"></a>错误请求，返回错误信息。</p>
</td>
</tr>
<tr id="row9846114818471"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p188468486471"><a name="p188468486471"></a><a name="p188468486471"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p11846134819473"><a name="p11846134819473"></a><a name="p11846134819473"></a>repository不存在。</p>
</td>
</tr>
<tr id="row16846248114719"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p2846248184714"><a name="p2846248184714"></a><a name="p2846248184714"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p5846154810474"><a name="p5846154810474"></a><a name="p5846154810474"></a>服务器内部错误，返回错误信息。</p>
</td>
</tr>
</tbody>
</table>

