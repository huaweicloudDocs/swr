# 查询所有API版本信息<a name="swr_02_0080"></a>

## 功能介绍

查询所有API版本信息

## 接口约束

无

## 调试<a name="atuogenerate_1"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=SWR&api=ListApiVersions)中调试该接口，支持自动认证鉴权。API Explorer可以自动生成SDK代码示例，并提供SDK代码示例调试功能。

## URI

GET /

## 请求参数

**表 1**  请求Header参数

|参数|是否必选|参数类型|描述|
|--|--|--|--|
|Content-Type|是|String|消息体的类型（格式），下方类型可任选其一使用： application/json;charset=utf-8 application/json缺省值：**application/json**|
|X-Auth-Token|是|String|用户Token。通过调用IAM服务获取用户Token接口获取（响应消息头中X-Subject-Token的值）。|


## 响应参数

**状态码： 200**

**表 2**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|versions|Array of VersionDetail objects|描述version相关对象的列表|


**表 3**  VersionDetail

|参数|参数类型|描述|
|--|--|--|
|id|String|版本ID（版本号)。|
|links|Link object|API的URL地址|
|version|String|若该版本API支持微版本，则填支持的最大微版本号，如果不支持微版本，则填空。|
|status|String|版本状态，为如下3种：CURRENT：表示该版本为主推版本；SUPPORTED：表示为老版本，但是现在还继续支持；DEPRECATED：表示为废弃版本，存在后续删除的可能。|
|updated|String|版本发布时间，要求用UTC时间表示。如v1发布的时间2014-06-28T12:20:21Z。|
|min_version|String|若该版本API 支持微版本，则填支持的最小微版本号， 如果不支持微版本，则填空。|


**表 4**  Link

|参数|参数类型|描述|
|--|--|--|
|href|String|链接|
|rel|String|描述|


## 请求示例

```
GET https://{endpoint}
```

## 响应示例

**状态码： 200**

查询成功

```
{
  "versions" : [ {
    "id" : "v2",
    "links" : {
      "href" : "https://swr-api.xxxx.myhuaweicloud.com/v2/",
      "rel" : "self"
    },
    "min_version" : "2.0",
    "status" : "CURRENT",
    "updated" : "2020-07-09T00:00:00Z",
    "version" : "2.26"
  } ]
}
```

## 状态码

|状态码|描述|
|--|--|
|200|查询成功|
|500|内部错误|


## 错误码

请参见[错误码](错误码.md)。

