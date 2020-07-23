# 查询镜像tag列表<a name="swr_02_0035"></a>

## 功能介绍<a name="section14905762191056"></a>

查询某一个镜像的所有镜像版本。

## URI<a name="section10482810165331"></a>

GET /v2/manage/namespaces/\{namespace\}/repos/\{repository\}/tags?filter=offset::\{offset\}|limit::\{limit\}|order\_column::\{order\_column\}|order\_type::\{order\_type\}|tag::\{tag\}

参数说明请参见[表1](#table11843162810214)。

**表 1**  参数说明

<a name="table11843162810214"></a>
<table><thead align="left"><tr id="row20843172818213"><th class="cellrowborder" valign="top" width="15.61%" id="mcps1.2.5.1.1"><p id="p3843528621"><a name="p3843528621"></a><a name="p3843528621"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="11.93%" id="mcps1.2.5.1.2"><p id="p1450315424313"><a name="p1450315424313"></a><a name="p1450315424313"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.22%" id="mcps1.2.5.1.3"><p id="p15022419437"><a name="p15022419437"></a><a name="p15022419437"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="55.24%" id="mcps1.2.5.1.4"><p id="p1584342811211"><a name="p1584342811211"></a><a name="p1584342811211"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1084316281925"><td class="cellrowborder" valign="top" width="15.61%" headers="mcps1.2.5.1.1 "><p id="p6843228526"><a name="p6843228526"></a><a name="p6843228526"></a>namespace</p>
</td>
<td class="cellrowborder" valign="top" width="11.93%" headers="mcps1.2.5.1.2 "><p id="p10507114164313"><a name="p10507114164313"></a><a name="p10507114164313"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.22%" headers="mcps1.2.5.1.3 "><p id="p105058419438"><a name="p105058419438"></a><a name="p105058419438"></a><span>String</span></p>
</td>
<td class="cellrowborder" valign="top" width="55.24%" headers="mcps1.2.5.1.4 "><p id="p85037015469"><a name="p85037015469"></a><a name="p85037015469"></a>组织名称</p>
</td>
</tr>
<tr id="row1319321944420"><td class="cellrowborder" valign="top" width="15.61%" headers="mcps1.2.5.1.1 "><p id="p919315194441"><a name="p919315194441"></a><a name="p919315194441"></a>repository</p>
</td>
<td class="cellrowborder" valign="top" width="11.93%" headers="mcps1.2.5.1.2 "><p id="p15466162817454"><a name="p15466162817454"></a><a name="p15466162817454"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.22%" headers="mcps1.2.5.1.3 "><p id="p546292854514"><a name="p546292854514"></a><a name="p546292854514"></a><span>String</span></p>
</td>
<td class="cellrowborder" valign="top" width="55.24%" headers="mcps1.2.5.1.4 "><p id="p13193201924411"><a name="p13193201924411"></a><a name="p13193201924411"></a>镜像仓库名称</p>
</td>
</tr>
<tr id="row64791218462"><td class="cellrowborder" valign="top" width="15.61%" headers="mcps1.2.5.1.1 "><p id="p06735284118"><a name="p06735284118"></a><a name="p06735284118"></a>offset</p>
</td>
<td class="cellrowborder" valign="top" width="11.93%" headers="mcps1.2.5.1.2 "><p id="p2673928141118"><a name="p2673928141118"></a><a name="p2673928141118"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.22%" headers="mcps1.2.5.1.3 "><p id="p86731328171117"><a name="p86731328171117"></a><a name="p86731328171117"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="55.24%" headers="mcps1.2.5.1.4 "><p id="p4673102861117"><a name="p4673102861117"></a><a name="p4673102861117"></a>起始索引</p>
</td>
</tr>
<tr id="row12480192174619"><td class="cellrowborder" valign="top" width="15.61%" headers="mcps1.2.5.1.1 "><p id="p18996138161115"><a name="p18996138161115"></a><a name="p18996138161115"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="11.93%" headers="mcps1.2.5.1.2 "><p id="p2099715389119"><a name="p2099715389119"></a><a name="p2099715389119"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.22%" headers="mcps1.2.5.1.3 "><p id="p1599653891110"><a name="p1599653891110"></a><a name="p1599653891110"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="55.24%" headers="mcps1.2.5.1.4 "><p id="p149971438121120"><a name="p149971438121120"></a><a name="p149971438121120"></a>返回的条数</p>
</td>
</tr>
<tr id="row74701012184713"><td class="cellrowborder" valign="top" width="15.61%" headers="mcps1.2.5.1.1 "><p id="p17470141274715"><a name="p17470141274715"></a><a name="p17470141274715"></a>order_column</p>
</td>
<td class="cellrowborder" valign="top" width="11.93%" headers="mcps1.2.5.1.2 "><p id="p11298142374713"><a name="p11298142374713"></a><a name="p11298142374713"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.22%" headers="mcps1.2.5.1.3 "><p id="p179431748184713"><a name="p179431748184713"></a><a name="p179431748184713"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.24%" headers="mcps1.2.5.1.4 "><p id="p1847081212472"><a name="p1847081212472"></a><a name="p1847081212472"></a>按列排序，可设置为updated_at（按更新时间排序）。</p>
</td>
</tr>
<tr id="row16470161294710"><td class="cellrowborder" valign="top" width="15.61%" headers="mcps1.2.5.1.1 "><p id="p1547061274718"><a name="p1547061274718"></a><a name="p1547061274718"></a>order_type</p>
</td>
<td class="cellrowborder" valign="top" width="11.93%" headers="mcps1.2.5.1.2 "><p id="p1430232320475"><a name="p1430232320475"></a><a name="p1430232320475"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.22%" headers="mcps1.2.5.1.3 "><p id="p394854824714"><a name="p394854824714"></a><a name="p394854824714"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.24%" headers="mcps1.2.5.1.4 "><p id="p12470131294710"><a name="p12470131294710"></a><a name="p12470131294710"></a>排序类型，可设置为desc（降序）、asc（升序）。</p>
</td>
</tr>
<tr id="row32671234114610"><td class="cellrowborder" valign="top" width="15.61%" headers="mcps1.2.5.1.1 "><p id="p16267173416465"><a name="p16267173416465"></a><a name="p16267173416465"></a>tag</p>
</td>
<td class="cellrowborder" valign="top" width="11.93%" headers="mcps1.2.5.1.2 "><p id="p13267103454614"><a name="p13267103454614"></a><a name="p13267103454614"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.22%" headers="mcps1.2.5.1.3 "><p id="p1026733434618"><a name="p1026733434618"></a><a name="p1026733434618"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.24%" headers="mcps1.2.5.1.4 "><p id="p9267334124613"><a name="p9267334124613"></a><a name="p9267334124613"></a>镜像版本名</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section3270966102931"></a>

N/A

## 响应消息<a name="section1262713444552"></a>

**响应参数**

**表 2**  Response Body参数说明

<a name="table45446245174724"></a>
<table><thead align="left"><tr id="row1412623174724"><th class="cellrowborder" valign="top" width="21.03789621037896%" id="mcps1.2.4.1.1"><p id="p47313663174724"><a name="p47313663174724"></a><a name="p47313663174724"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20.157984201579843%" id="mcps1.2.4.1.2"><p id="p7201512174724"><a name="p7201512174724"></a><a name="p7201512174724"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="58.80411958804119%" id="mcps1.2.4.1.3"><p id="p4480706174724"><a name="p4480706174724"></a><a name="p4480706174724"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row23391130131913"><td class="cellrowborder" valign="top" width="21.03789621037896%" headers="mcps1.2.4.1.1 "><p id="p43401630141910"><a name="p43401630141910"></a><a name="p43401630141910"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.2.4.1.2 "><p id="p1224112114332"><a name="p1224112114332"></a><a name="p1224112114332"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="58.80411958804119%" headers="mcps1.2.4.1.3 "><p id="p20340730191918"><a name="p20340730191918"></a><a name="p20340730191918"></a>编号</p>
</td>
</tr>
<tr id="row697982791918"><td class="cellrowborder" valign="top" width="21.03789621037896%" headers="mcps1.2.4.1.1 "><p id="p10980112717192"><a name="p10980112717192"></a><a name="p10980112717192"></a>repo_id</p>
</td>
<td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.2.4.1.2 "><p id="p20980132718193"><a name="p20980132718193"></a><a name="p20980132718193"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="58.80411958804119%" headers="mcps1.2.4.1.3 "><p id="p14980192714197"><a name="p14980192714197"></a><a name="p14980192714197"></a>仓库编号</p>
</td>
</tr>
<tr id="row17668249354"><td class="cellrowborder" valign="top" width="21.03789621037896%" headers="mcps1.2.4.1.1 "><p id="p3602231570"><a name="p3602231570"></a><a name="p3602231570"></a>Tag</p>
</td>
<td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.2.4.1.2 "><p id="p360215315712"><a name="p360215315712"></a><a name="p360215315712"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.80411958804119%" headers="mcps1.2.4.1.3 "><p id="p206025311878"><a name="p206025311878"></a><a name="p206025311878"></a>Tag版本名称</p>
</td>
</tr>
<tr id="row176816213207"><td class="cellrowborder" valign="top" width="21.03789621037896%" headers="mcps1.2.4.1.1 "><p id="p1568212212204"><a name="p1568212212204"></a><a name="p1568212212204"></a>image_id</p>
</td>
<td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.2.4.1.2 "><p id="p1568252172015"><a name="p1568252172015"></a><a name="p1568252172015"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.80411958804119%" headers="mcps1.2.4.1.3 "><p id="p1968202192013"><a name="p1968202192013"></a><a name="p1968202192013"></a>镜像id</p>
</td>
</tr>
<tr id="row2590104211156"><td class="cellrowborder" valign="top" width="21.03789621037896%" headers="mcps1.2.4.1.1 "><p id="p1592204251517"><a name="p1592204251517"></a><a name="p1592204251517"></a>manifest</p>
</td>
<td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.2.4.1.2 "><p id="p95921422152"><a name="p95921422152"></a><a name="p95921422152"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.80411958804119%" headers="mcps1.2.4.1.3 "><p id="p145923427155"><a name="p145923427155"></a><a name="p145923427155"></a>镜像manifest</p>
</td>
</tr>
<tr id="row411720412429"><td class="cellrowborder" valign="top" width="21.03789621037896%" headers="mcps1.2.4.1.1 "><p id="p8361449104214"><a name="p8361449104214"></a><a name="p8361449104214"></a>digest</p>
</td>
<td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.2.4.1.2 "><p id="p103631149164219"><a name="p103631149164219"></a><a name="p103631149164219"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.80411958804119%" headers="mcps1.2.4.1.3 "><p id="p33651491427"><a name="p33651491427"></a><a name="p33651491427"></a>镜像sha值</p>
</td>
</tr>
<tr id="row19747155313423"><td class="cellrowborder" valign="top" width="21.03789621037896%" headers="mcps1.2.4.1.1 "><p id="p55111044437"><a name="p55111044437"></a><a name="p55111044437"></a>schema</p>
</td>
<td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.2.4.1.2 "><p id="p65137412431"><a name="p65137412431"></a><a name="p65137412431"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="58.80411958804119%" headers="mcps1.2.4.1.3 "><p id="p05141147434"><a name="p05141147434"></a><a name="p05141147434"></a>docker协议版本，值为1或2。</p>
</td>
</tr>
<tr id="row27392900174724"><td class="cellrowborder" valign="top" width="21.03789621037896%" headers="mcps1.2.4.1.1 "><p id="p66029311173"><a name="p66029311173"></a><a name="p66029311173"></a>path</p>
</td>
<td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.2.4.1.2 "><p id="p460211311279"><a name="p460211311279"></a><a name="p460211311279"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.80411958804119%" headers="mcps1.2.4.1.3 "><p id="p9603163112712"><a name="p9603163112712"></a><a name="p9603163112712"></a>镜像pull地址，格式为</p>
<p id="p8659141362"><a name="p8659141362"></a><a name="p8659141362"></a>swr.cn-north-1.myhuaweicloud.com/namespace/repository:tag。</p>
</td>
</tr>
<tr id="row207081451715"><td class="cellrowborder" valign="top" width="21.03789621037896%" headers="mcps1.2.4.1.1 "><p id="p1701714191712"><a name="p1701714191712"></a><a name="p1701714191712"></a>internal_path</p>
</td>
<td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.2.4.1.2 "><p id="p470314161716"><a name="p470314161716"></a><a name="p470314161716"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.80411958804119%" headers="mcps1.2.4.1.3 "><p id="p07051481718"><a name="p07051481718"></a><a name="p07051481718"></a>cce集群内镜像pull路径，格式为 10.125.0.198:20202/namespace/repository:tag</p>
</td>
</tr>
<tr id="row12917712114013"><td class="cellrowborder" valign="top" width="21.03789621037896%" headers="mcps1.2.4.1.1 "><p id="p15603531879"><a name="p15603531879"></a><a name="p15603531879"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.2.4.1.2 "><p id="p1760318310710"><a name="p1760318310710"></a><a name="p1760318310710"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="58.80411958804119%" headers="mcps1.2.4.1.3 "><p id="p136038314714"><a name="p136038314714"></a><a name="p136038314714"></a>镜像大小，0 ~ 9223372036854775807。</p>
</td>
</tr>
<tr id="row6189161112289"><td class="cellrowborder" valign="top" width="21.03789621037896%" headers="mcps1.2.4.1.1 "><p id="p519041132810"><a name="p519041132810"></a><a name="p519041132810"></a>is_trusted</p>
</td>
<td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.2.4.1.2 "><p id="p1119014117288"><a name="p1119014117288"></a><a name="p1119014117288"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="58.80411958804119%" headers="mcps1.2.4.1.3 "><p id="p13191811182818"><a name="p13191811182818"></a><a name="p13191811182818"></a>默认值为false</p>
</td>
</tr>
<tr id="row24091911193911"><td class="cellrowborder" valign="top" width="21.03789621037896%" headers="mcps1.2.4.1.1 "><p id="p13603531378"><a name="p13603531378"></a><a name="p13603531378"></a>created</p>
</td>
<td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.2.4.1.2 "><p id="p660333115711"><a name="p660333115711"></a><a name="p660333115711"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.80411958804119%" headers="mcps1.2.4.1.3 "><p id="p760315313710"><a name="p760315313710"></a><a name="p760315313710"></a>镜像创建时间，UTC时间格式，时间为UTC标准时间，用户需要根据本地时间计算偏移量；如东8区需要+8:00。</p>
</td>
</tr>
<tr id="row10790853193918"><td class="cellrowborder" valign="top" width="21.03789621037896%" headers="mcps1.2.4.1.1 "><p id="p14603631778"><a name="p14603631778"></a><a name="p14603631778"></a>updated</p>
</td>
<td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.2.4.1.2 "><p id="p3603203112717"><a name="p3603203112717"></a><a name="p3603203112717"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.80411958804119%" headers="mcps1.2.4.1.3 "><p id="p1360316317716"><a name="p1360316317716"></a><a name="p1360316317716"></a>镜像更新时间，UTC时间格式，时间为UTC标准时间，用户需要根据本地时间计算偏移量；如东8区需要+8:00。</p>
</td>
</tr>
<tr id="row1627112185506"><td class="cellrowborder" valign="top" width="21.03789621037896%" headers="mcps1.2.4.1.1 "><p id="p427119188502"><a name="p427119188502"></a><a name="p427119188502"></a>deleted</p>
</td>
<td class="cellrowborder" valign="top" width="20.157984201579843%" headers="mcps1.2.4.1.2 "><p id="p142711318125017"><a name="p142711318125017"></a><a name="p142711318125017"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.80411958804119%" headers="mcps1.2.4.1.3 "><p id="p1327116186505"><a name="p1327116186505"></a><a name="p1327116186505"></a>镜像删除时间</p>
</td>
</tr>
</tbody>
</table>

**响应示例**

```
[
    {
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
    }
]
```

## 状态码<a name="section5365169104253"></a>

状态码如[表3](#table1984564864716)所示。

**表 3**  状态码

<a name="table1984564864716"></a>
<table><thead align="left"><tr id="row1984554824718"><th class="cellrowborder" valign="top" width="16.99%" id="mcps1.2.3.1.1"><p id="p4846548124714"><a name="p4846548124714"></a><a name="p4846548124714"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="83.00999999999999%" id="mcps1.2.3.1.2"><p id="p984612486479"><a name="p984612486479"></a><a name="p984612486479"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1484619482477"><td class="cellrowborder" valign="top" width="16.99%" headers="mcps1.2.3.1.1 "><p id="p88461948154710"><a name="p88461948154710"></a><a name="p88461948154710"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="83.00999999999999%" headers="mcps1.2.3.1.2 "><p id="p13846748154710"><a name="p13846748154710"></a><a name="p13846748154710"></a>成功查询镜像仓库的所有tag。</p>
</td>
</tr>
<tr id="row98468489472"><td class="cellrowborder" valign="top" width="16.99%" headers="mcps1.2.3.1.1 "><p id="p14846134812476"><a name="p14846134812476"></a><a name="p14846134812476"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="83.00999999999999%" headers="mcps1.2.3.1.2 "><p id="p08461448114716"><a name="p08461448114716"></a><a name="p08461448114716"></a>错误请求，返回错误信息。</p>
</td>
</tr>
<tr id="row631310443579"><td class="cellrowborder" valign="top" width="16.99%" headers="mcps1.2.3.1.1 "><p id="p12314164419574"><a name="p12314164419574"></a><a name="p12314164419574"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="83.00999999999999%" headers="mcps1.2.3.1.2 "><p id="p93141244155715"><a name="p93141244155715"></a><a name="p93141244155715"></a>鉴权失败。</p>
</td>
</tr>
<tr id="row9846114818471"><td class="cellrowborder" valign="top" width="16.99%" headers="mcps1.2.3.1.1 "><p id="p188468486471"><a name="p188468486471"></a><a name="p188468486471"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="83.00999999999999%" headers="mcps1.2.3.1.2 "><p id="p11846134819473"><a name="p11846134819473"></a><a name="p11846134819473"></a>repository不存在。</p>
</td>
</tr>
<tr id="row16846248114719"><td class="cellrowborder" valign="top" width="16.99%" headers="mcps1.2.3.1.1 "><p id="p2846248184714"><a name="p2846248184714"></a><a name="p2846248184714"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="83.00999999999999%" headers="mcps1.2.3.1.2 "><p id="p5846154810474"><a name="p5846154810474"></a><a name="p5846154810474"></a>服务器内部错误，返回错误信息。</p>
</td>
</tr>
</tbody>
</table>

