# REST API介绍<a name="swr_02_0006"></a>

公有云API符合RESTful API的设计理论。

REST从资源的角度来观察整个网络，提供创建、查询、更新、删掉等方法访问服务的资源。

REST API请求/响应对可以分为如下部分：

-   请求URI
-   请求方法
-   请求消息头
-   请求消息体
-   响应消息头
-   响应消息体

## 请求URI<a name="section1849899574"></a>

请求URI由如下部分组成。

**\{URI-scheme\} :// \{**Endpoint**\} / \{resource-path\} ? \{query-string\}**

尽管请求URI包含在请求消息头中，但大多数语言或框架都要求您从请求消息中单独传递它，所有在此单独拿出来强调。

**表 1**  URI中的参数说明

<a name="t1797260c744a4e1a85d354f259cae55a"></a>
<table><thead align="left"><tr id="r6dceed05bcc649d2b032accbb2980a31"><th class="cellrowborder" valign="top" width="24.529999999999998%" id="mcps1.2.3.1.1"><p id="a3446b6b785cb432bae9f45aef9177041"><a name="a3446b6b785cb432bae9f45aef9177041"></a><a name="a3446b6b785cb432bae9f45aef9177041"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="75.47%" id="mcps1.2.3.1.2"><p id="abe71244a12ac45308e99d4bbf975a9f8"><a name="abe71244a12ac45308e99d4bbf975a9f8"></a><a name="abe71244a12ac45308e99d4bbf975a9f8"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row106982018513"><td class="cellrowborder" valign="top" width="24.529999999999998%" headers="mcps1.2.3.1.1 "><p id="p136991001517"><a name="p136991001517"></a><a name="p136991001517"></a>URI-scheme</p>
</td>
<td class="cellrowborder" valign="top" width="75.47%" headers="mcps1.2.3.1.2 "><p id="p56992017520"><a name="p56992017520"></a><a name="p56992017520"></a>表示用于传输请求的协议。</p>
</td>
</tr>
<tr id="rb217758afff146a1b40b0dcbb28a4ae1"><td class="cellrowborder" valign="top" width="24.529999999999998%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0035614179_p480227019422"><a name="zh-cn_topic_0035614179_p480227019422"></a><a name="zh-cn_topic_0035614179_p480227019422"></a>Endpoint</p>
</td>
<td class="cellrowborder" valign="top" width="75.47%" headers="mcps1.2.3.1.2 "><p id="ad82b3484a1be43ddadf436efbe15285e"><a name="ad82b3484a1be43ddadf436efbe15285e"></a><a name="ad82b3484a1be43ddadf436efbe15285e"></a>指定承载REST服务端点的服务器域名或IP，从<a href="http://developer-intl.huaweicloud.com/zh-cn/endpoint.html" target="_blank" rel="noopener noreferrer">地区和终端节点</a><a href="http://developer.huaweicloud.com/dev/endpoint" target="_blank" rel="noopener noreferrer">地区和终端节点</a>中获取。</p>
</td>
</tr>
<tr id="refeed61892004ea682639be281a1a707"><td class="cellrowborder" valign="top" width="24.529999999999998%" headers="mcps1.2.3.1.1 "><p id="p1797614317513"><a name="p1797614317513"></a><a name="p1797614317513"></a>resource-path</p>
</td>
<td class="cellrowborder" valign="top" width="75.47%" headers="mcps1.2.3.1.2 "><p id="a90409cbb8b1c49c4ad4d3cfee16f475e"><a name="a90409cbb8b1c49c4ad4d3cfee16f475e"></a><a name="a90409cbb8b1c49c4ad4d3cfee16f475e"></a>资源路径，也即API访问路径。从具体接口的URI模块获取，例如“v3/auth/tokens”。</p>
</td>
</tr>
<tr id="row19939365518"><td class="cellrowborder" valign="top" width="24.529999999999998%" headers="mcps1.2.3.1.1 "><p id="p393966455"><a name="p393966455"></a><a name="p393966455"></a>Query string</p>
</td>
<td class="cellrowborder" valign="top" width="75.47%" headers="mcps1.2.3.1.2 "><p id="p159401867517"><a name="p159401867517"></a><a name="p159401867517"></a>可选参数，例如API版本或资源选择标准。</p>
</td>
</tr>
</tbody>
</table>

## 请求方法<a name="section580035055419"></a>

HTTP方法（也称为操作或动词），它告诉服务你正在请求什么类型的操作。

**表 2**  HTTP方法

<a name="table26515221161"></a>
<table><thead align="left"><tr id="row10728192251616"><th class="cellrowborder" valign="top" width="18%" id="mcps1.2.3.1.1"><p id="p157281422201616"><a name="p157281422201616"></a><a name="p157281422201616"></a>方法</p>
</th>
<th class="cellrowborder" valign="top" width="82%" id="mcps1.2.3.1.2"><p id="p672872219161"><a name="p672872219161"></a><a name="p672872219161"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1394642154919"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.3.1.1 "><p id="p13848247114919"><a name="p13848247114919"></a><a name="p13848247114919"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="82%" headers="mcps1.2.3.1.2 "><p id="p2850147164917"><a name="p2850147164917"></a><a name="p2850147164917"></a>请求服务器返回指定资源。</p>
</td>
</tr>
<tr id="row5728322121617"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.3.1.1 "><p id="p97281922111616"><a name="p97281922111616"></a><a name="p97281922111616"></a>PUT</p>
</td>
<td class="cellrowborder" valign="top" width="82%" headers="mcps1.2.3.1.2 "><p id="p1572882241617"><a name="p1572882241617"></a><a name="p1572882241617"></a>请求服务器更新指定资源。</p>
</td>
</tr>
<tr id="row172872211168"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.3.1.1 "><p id="p472820225166"><a name="p472820225166"></a><a name="p472820225166"></a>POST</p>
</td>
<td class="cellrowborder" valign="top" width="82%" headers="mcps1.2.3.1.2 "><p id="p272812212161"><a name="p272812212161"></a><a name="p272812212161"></a>请求服务器新增资源或执行特殊操作。</p>
</td>
</tr>
<tr id="row8728132231620"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.3.1.1 "><p id="p16729422151616"><a name="p16729422151616"></a><a name="p16729422151616"></a>DELETE</p>
</td>
<td class="cellrowborder" valign="top" width="82%" headers="mcps1.2.3.1.2 "><p id="p10729122261616"><a name="p10729122261616"></a><a name="p10729122261616"></a>请求服务器删除指定资源，如删除对象等。</p>
</td>
</tr>
<tr id="row2157183019175"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.3.1.1 "><p id="p15159030201715"><a name="p15159030201715"></a><a name="p15159030201715"></a>HEAD</p>
</td>
<td class="cellrowborder" valign="top" width="82%" headers="mcps1.2.3.1.2 "><p id="p42261787492"><a name="p42261787492"></a><a name="p42261787492"></a>请求服务器资源头部。</p>
</td>
</tr>
<tr id="row16729182210163"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.3.1.1 "><p id="p1772932218162"><a name="p1772932218162"></a><a name="p1772932218162"></a>PATCH</p>
</td>
<td class="cellrowborder" valign="top" width="82%" headers="mcps1.2.3.1.2 "><p id="p13729192251620"><a name="p13729192251620"></a><a name="p13729192251620"></a>请求服务器更新资源的部分内容。</p>
<p id="p0729142221616"><a name="p0729142221616"></a><a name="p0729142221616"></a>当资源不存在的时候，PATCH可能会去创建一个新的资源。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息头<a name="section1454211155819"></a>

请求消息头由若干头域构成，每个头域由一个域名，冒号\(: \)和域值组成。

可选的附加请求头字段，如指定的URI和HTTP方法所要求的字段。详细的公共请求消息头字段请参见[表1](公共请求参数.md#table64174151155930)，其中请求认证信息请参见[获取请求认证](获取请求认证.md)。

## 请求消息体（可选）<a name="section14612192315587"></a>

请求消息体通常以JSON格式封装，基本语法是嵌套式的key:value形式。HTTP请求的正文针对不同的URI对象有不同的必须字段和可选字段。

## 响应消息头<a name="section7804143005810"></a>

响应的消息报头在大多数情况下含如所[表1](公共响应参数.md#table431633395935)的响应报头。

## 响应消息体（可选）<a name="section034615592583"></a>

响应消息体通常是JSON格式的文本，当接口调用出现错误时会返回错误码及描述。

## 发起请求<a name="section140743661613"></a>

共有三种方式可以基于已构建好的请求消息发起请求，分别为：

-   cURL

    cURL是一个命令行工具，用来执行各种URL操作和信息传输。cURL充当的是HTTP客户端，可以发送HTTP请求给服务端，并接收响应消息。cURL适用于接口调试。关于cURL详细信息请参见[https://curl.haxx.se/](https://curl.haxx.se/)。

-   编码

    通过编码调用接口，组装请求消息，并发送处理请求消息。

-   REST客户端

    Mozilla、Google都为REST提供了图形化的浏览器插件，发送处理请求消息。针对Firefox，请参见[Firefox REST Client](https://addons.mozilla.org/en-US/firefox/addon/restclient/)。针对Chrome，请参见[Postman](https://chrome.google.com/webstore/detail/postman/fhbjgbiflinjbdggehcddcbncdddomop)。


