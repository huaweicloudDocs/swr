# API概览<a name="swr_02_0065"></a>

通过使用容器镜像服务提供的接口，您可以实现对组织、镜像仓库、镜像信息的查询，也可以实现对组织、镜像仓库、镜像的管理操作。

**表 1**  接口说明

<a name="table88711342351"></a>
<table><thead align="left"><tr id="row88716427513"><th class="cellrowborder" valign="top" width="32%" id="mcps1.2.3.1.1"><p id="p1871442156"><a name="p1871442156"></a><a name="p1871442156"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="68%" id="mcps1.2.3.1.2"><p id="p12871194215516"><a name="p12871194215516"></a><a name="p12871194215516"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1145120310497"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p3451113194913"><a name="p3451113194913"></a><a name="p3451113194913"></a><a href="创建组织.md">创建组织</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p7451153154910"><a name="p7451153154910"></a><a name="p7451153154910"></a>创建组织。</p>
</td>
</tr>
<tr id="row1345119354918"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p7451153204913"><a name="p7451153204913"></a><a name="p7451153204913"></a><a href="删除组织.md">删除组织</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p1145183194916"><a name="p1145183194916"></a><a name="p1145183194916"></a>删除组织。</p>
</td>
</tr>
<tr id="row14515315491"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p124513314916"><a name="p124513314916"></a><a name="p124513314916"></a><a href="查询组织列表.md">查询组织列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p745113184912"><a name="p745113184912"></a><a name="p745113184912"></a>查询组织列表。</p>
</td>
</tr>
<tr id="row139966563480"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p2099612562482"><a name="p2099612562482"></a><a name="p2099612562482"></a><a href="查询组织详情.md">查询组织详情</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p7996155618489"><a name="p7996155618489"></a><a name="p7996155618489"></a>查询某个组织的详情信息，包括组织id、组织名称、创建者和用户权限。</p>
</td>
</tr>
<tr id="row193875553480"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p16387155134819"><a name="p16387155134819"></a><a name="p16387155134819"></a><a href="创建镜像仓库.md">创建镜像仓库</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p173871455144811"><a name="p173871455144811"></a><a name="p173871455144811"></a>在组织下创建镜像仓库。</p>
</td>
</tr>
<tr id="row76419536489"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p3643453174816"><a name="p3643453174816"></a><a name="p3643453174816"></a><a href="删除镜像仓库.md">删除镜像仓库</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p0643175315481"><a name="p0643175315481"></a><a name="p0643175315481"></a>删除组织下的镜像仓库。</p>
</td>
</tr>
<tr id="row08723421515"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p207961550184814"><a name="p207961550184814"></a><a name="p207961550184814"></a><a href="更新镜像仓库的概要信息.md">更新镜像的概要信息</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p121701508378"><a name="p121701508378"></a><a name="p121701508378"></a>更新账号组织下的镜像概要信息，包括镜像类型、是否公有、描述信息。</p>
</td>
</tr>
<tr id="row1187211423510"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p9795250174816"><a name="p9795250174816"></a><a name="p9795250174816"></a><a href="查询镜像仓库概要信息.md">查询镜像概要信息</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p61691806371"><a name="p61691806371"></a><a name="p61691806371"></a>查询账号组织下镜像的概要信息，包括仓库id、组织id、仓库名称、<span>仓库描述信息</span>、<span>仓库创建者</span>、仓库大小、<span>镜像pull路径</span>等。</p>
</td>
</tr>
<tr id="row2087254219512"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p0795050194818"><a name="p0795050194818"></a><a name="p0795050194818"></a><a href="查询镜像列表.md">查询镜像列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p161673011371"><a name="p161673011371"></a><a name="p161673011371"></a>查询镜像列表。</p>
</td>
</tr>
<tr id="row1387219421653"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p2794125004815"><a name="p2794125004815"></a><a name="p2794125004815"></a><a href="查询镜像tag列表.md">查询镜像tag列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p21651406373"><a name="p21651406373"></a><a name="p21651406373"></a>获取镜像的tag的列表。</p>
</td>
</tr>
<tr id="row20873042758"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p6793450104811"><a name="p6793450104811"></a><a name="p6793450104811"></a><a href="删除指定tag的镜像.md">删除指定tag的镜像</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p8165140173719"><a name="p8165140173719"></a><a name="p8165140173719"></a>删除镜像仓库中指定tag的镜像。</p>
</td>
</tr>
<tr id="row1996444614579"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p18964164619574"><a name="p18964164619574"></a><a name="p18964164619574"></a><a href="查询官方镜像列表.md">查询官方镜像列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p10964114655716"><a name="p10964114655716"></a><a name="p10964114655716"></a>查询官方镜像列表。容器镜像服务为您提供大量的公有镜像资源检索，包括docker官方镜像资源。您可以收藏这些镜像并推送到自己的仓库之中，方便使用。</p>
</td>
</tr>
<tr id="row27545115719"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p675125113575"><a name="p675125113575"></a><a name="p675125113575"></a><a href="查询官方镜像详情.md">查询官方镜像详情</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p1075165111571"><a name="p1075165111571"></a><a name="p1075165111571"></a>查询官方镜像详情。</p>
</td>
</tr>
<tr id="row14834124815572"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p15834164815579"><a name="p15834164815579"></a><a name="p15834164815579"></a><a href="查询官方镜像版本列表.md">查询官方镜像版本列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p1583464835719"><a name="p1583464835719"></a><a name="p1583464835719"></a>查询官方镜像版本列表。</p>
</td>
</tr>
<tr id="row191740203579"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p1617512015712"><a name="p1617512015712"></a><a name="p1617512015712"></a><a href="创建共享账号.md">创建共享账号</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p13176220165710"><a name="p13176220165710"></a><a name="p13176220165710"></a>创建共享账号。镜像上传后，您可以共享<span class="keyword" id="keyword149651164212"><a name="keyword149651164212"></a><a name="keyword149651164212"></a>私有镜像</span>给其他账号，并授予下载该镜像的权限。</p>
</td>
</tr>
<tr id="row0364155612568"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p736595615610"><a name="p736595615610"></a><a name="p736595615610"></a><a href="删除共享账号.md">删除共享账号</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p129123259110"><a name="p129123259110"></a><a name="p129123259110"></a>删除共享账号。</p>
</td>
</tr>
<tr id="row941674820567"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p18418134820563"><a name="p18418134820563"></a><a name="p18418134820563"></a><a href="更新共享账号.md">更新共享账号</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p103461628015"><a name="p103461628015"></a><a name="p103461628015"></a>更新共享账号。</p>
</td>
</tr>
<tr id="row71481415924"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p514917153219"><a name="p514917153219"></a><a name="p514917153219"></a><a href="判断共享帐号是否存在.md">判断共享账号是否存在</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p51499156219"><a name="p51499156219"></a><a name="p51499156219"></a>判断共享账号是否存在。</p>
</td>
</tr>
<tr id="row207281881322"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p1731148728"><a name="p1731148728"></a><a name="p1731148728"></a><a href="获取共享帐号列表.md">获取共享账号列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p47313817219"><a name="p47313817219"></a><a name="p47313817219"></a>获取共享账号列表。</p>
</td>
</tr>
<tr id="row1295416574198"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p45251171204"><a name="p45251171204"></a><a name="p45251171204"></a><a href="查看共享镜像列表.md">查看共享镜像列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p11525197112013"><a name="p11525197112013"></a><a name="p11525197112013"></a>查看共享镜像列表。</p>
</td>
</tr>
<tr id="row109551357181911"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p95265792016"><a name="p95265792016"></a><a name="p95265792016"></a><a href="查询所有API版本信息.md">查询所有API版本信息</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p195261076209"><a name="p195261076209"></a><a name="p195261076209"></a>查询<span>容器镜像</span>服务所有可用的API版本信息列表。</p>
</td>
</tr>
<tr id="row1295535710193"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p05261876202"><a name="p05261876202"></a><a name="p05261876202"></a><a href="查询指定API版本信息.md">查询指定API版本信息</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p155261579206"><a name="p155261579206"></a><a name="p155261579206"></a>查询<span>容器镜像</span>服务指定API版本信息列表。</p>
</td>
</tr>
<tr id="row7955105731915"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p1552677112018"><a name="p1552677112018"></a><a name="p1552677112018"></a><a href="获取镜像中心下载次数统计.md">获取镜像中心下载次数统计</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p4526107132018"><a name="p4526107132018"></a><a name="p4526107132018"></a>获取镜像中心下载次数统计。</p>
</td>
</tr>
<tr id="row181264548191"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p1852677112013"><a name="p1852677112013"></a><a name="p1852677112013"></a><a href="获取镜像加速器地址.md">获取镜像加速器地址</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p20526774204"><a name="p20526774204"></a><a name="p20526774204"></a>获取镜像加速器地址。</p>
</td>
</tr>
<tr id="row1681441205812"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p5814416584"><a name="p5814416584"></a><a name="p5814416584"></a><a href="创建组织权限.md">创建组织权限</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p781417135817"><a name="p781417135817"></a><a name="p781417135817"></a>创建组织权限。</p>
</td>
</tr>
<tr id="row281418165819"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p481431145812"><a name="p481431145812"></a><a name="p481431145812"></a><a href="删除组织权限.md">删除组织权限</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p1681441175818"><a name="p1681441175818"></a><a name="p1681441175818"></a>删除组织权限。</p>
</td>
</tr>
<tr id="row12814917588"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p18147113583"><a name="p18147113583"></a><a name="p18147113583"></a><a href="更新组织权限.md">更新组织权限</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p1081410110585"><a name="p1081410110585"></a><a name="p1081410110585"></a>更新组织权限。</p>
</td>
</tr>
<tr id="row15903376582"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p89031771584"><a name="p89031771584"></a><a name="p89031771584"></a><a href="查询组织权限.md">查询组织权限</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p17903278585"><a name="p17903278585"></a><a name="p17903278585"></a>查询组织权限。</p>
</td>
</tr>
</tbody>
</table>

