# 查询镜像tag列表<a name="swr_02_0035"></a>

## 功能介绍

查询镜像tag列表

## 接口约束

无

## 调试<a name="atuogenerate_1"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=SWR&api=ListRepositoryTags)中调试该接口，支持自动认证鉴权。API Explorer可以自动生成SDK代码示例，并提供SDK代码示例调试功能。

## URI

GET /v2/manage/namespaces/\{namespace\}/repos/\{repository\}/tags

**表 1**  路径参数

|参数|是否必选|参数类型|描述|
|--|--|--|--|
|namespace|是|String|组织名称。小写字母开头，后面跟小写字母、数字、小数点、下划线或中划线（其中下划线最多允许连续两个，小数点、下划线、中划线不能直接相连），小写字母或数字结尾，1-64个字符。|
|repository|是|String|镜像仓库名称|


**表 2**  Query参数

|参数|是否必选|参数类型|描述|
|--|--|--|--|
|limit|否|String|返回条数。注意：offset和limit参数需要配套使用。|
|offset|否|String|起始索引。注意：offset和limit参数需要配套使用。|
|order_column|否|String|按列排序，可设置为updated_at（按更新时间排序）。注意：order_column和order_type参数需要配套使用。|
|order_type|否|String|排序类型，可设置为desc（降序）、asc（升序）。注意：order_column和order_type参数需要配套使用。|
|tag|否|String|镜像版本名。|
|filter|否|String|应填写 offset::{offset}|limit::{limit}|order_column::{order_column}|order_type::{order_type}|tag::{tag} ,其中{limit}为返回条数,{offset}为起始索引,注意：offset和limit参数需要配套使用。 {order_column}为按列排序，可设置为updated_at（按更新时间排序）,{order_type}为排序类型，可设置为desc（降序）、asc（升序），{tag}为镜像版本名。|


## 请求参数

**表 3**  请求Header参数

|参数|是否必选|参数类型|描述|
|--|--|--|--|
|Content-Type|是|String|消息体的类型（格式），下方类型可任选其一使用： application/json;charset=utf-8 application/json缺省值：**application/json**|
|X-Auth-Token|是|String|用户Token。通过调用IAM服务获取用户Token接口获取（响应消息头中X-Subject-Token的值）。|


## 响应参数

**状态码： 200**

**表 4**  响应Header参数

|参数|参数类型|描述|
|--|--|--|
|Content-Range|String|offset(开始索引)-count(当前页记录条数)/total(总记录条数)|


**表 5**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|[数组元素]|Array of ShowReposTagResp objects|镜像tag列表|


**表 6**  ShowReposTagResp

|参数|参数类型|描述|
|--|--|--|
|id|Long|tag编号|
|repo_id|Long|仓库编号|
|Tag|String|Tag版本名称|
|image_id|String|镜像id|
|manifest|String|镜像manifest|
|digest|String|镜像hash值|
|schema|Long|docker协议版本，值为1或2|
|path|String|镜像pull地址，格式为swr.cn-north-1.myhuaweicloud.com/namespace/repository:tag|
|internal_path|String|cce集群内镜像pull路径，格式为 10.125.0.198:20202/namespace/repository:tag|
|size|Long|镜像大小，0 ~ 9223372036854775807|
|is_trusted|Boolean|默认值为false缺省值：**false**|
|created|String|镜像创建时间，UTC时间格式，时间为UTC标准时间，用户需要根据本地时间计算偏移量；如东8区需要+8:00|
|updated|String|镜像更新时间，UTC时间格式，时间为UTC标准时间，用户需要根据本地时间计算偏移量；如东8区需要+8:00|
|deleted|String|镜像删除时间，UTC时间格式，时间为UTC标准时间，用户需要根据本地时间计算偏移量；如东8区需要+8:00|
|domain_id|String|帐号ID|
|scanned|Boolean|镜像是否被扫描过|
|tag_type|Long|0：manifest类型；1：manifest list类型|


## 请求示例

```
GET https://{endpoint}/v2/manage/namespaces/{namespace}/repos/{repository}/tags
```

## 响应示例

**状态码： 200**

查询镜像列表tag列表成功

```
[ {
  "id" : 0,
  "repo_id" : 0,
  "Tag" : "latest",
  "image_id" : "741f24a795d6d93d7c6edd11780d63c13e16c39615dd9d223378a57a836f2ee6",
  "manifest" : "{\"schemaVersion\":2,\"mediaType\":\"application/vnd.docker.distribution.manifest.v2+json\",\"config\":{\"mediaType\":\"application/vnd.docker.container.image.v1+json\",\"size\":1862,\"digest\":\"sha256:741f24a795d6d93d7c6edd11780d63c13e16c39615dd9d223378a57a836f2ee6\"},\"layers\":[{\"mediaType\":\"application/vnd.docker.image.rootfs.diff.tar.gzip\",\"size\":1292800,\"digest\":\"sha256:8ac8bfaff55af948c796026ee867448c5b5b5d9dd3549f4006d9759b25d4a893\"},{\"mediaType\":\"application/vnd.docker.image.rootfs.diff.tar.gzip\",\"size\":10240,\"digest\":\"sha256:77ddbf3a9fe11e81761a0f9df43a28e3e6f29bbb53c0c8cf71cd7efa69729aed\"}]}",
  "digest" : "sha256:57b605845a6367c34bfb6ea6477f16852f59aa1861a2b51d10ab77ae0a1dc9c3",
  "schema" : 2,
  "path" : "swr.cn-north-1.myhuaweicloud.com/namespace/busybox:latest",
  "internal_path" : "10.125.0.198:20202/namespace/busybox:latest",
  "size" : 1304902,
  "is_trusted" : false,
  "created" : "2018-07-06T06:18:55Z",
  "updated" : "2018-07-06T06:18:55Z",
  "deleted" : null,
  "domain_id" : "0503dda878000fed0f75c0096d70a960",
  "scanned" : false,
  "tag_type" : 0
} ]
```

## 状态码

|状态码|描述|
|--|--|
|200|查询镜像列表tag列表成功|
|400|错误的请求|
|401|鉴权失败|
|404|镜像仓库不存在|
|500|内部错误|


## 错误码

请参见[错误码](错误码.md)。

