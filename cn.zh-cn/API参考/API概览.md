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
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p7996155618489"><a name="p7996155618489"></a><a name="p7996155618489"></a>查询某个组织的详细信息，包括组织ID、组织名称、创建者和用户权限。</p>
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
<tr id="row08723421515"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p207961550184814"><a name="p207961550184814"></a><a name="p207961550184814"></a><a href="更新镜像仓库的概要信息.md">更新镜像仓库的概要信息</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p121701508378"><a name="p121701508378"></a><a name="p121701508378"></a>更新组织下的镜像仓库概要信息，包括镜像类型、是否公有、描述信息。</p>
</td>
</tr>
<tr id="row1187211423510"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p9795250174816"><a name="p9795250174816"></a><a name="p9795250174816"></a><a href="查询镜像仓库概要信息.md">查询镜像仓库概要信息</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p61691806371"><a name="p61691806371"></a><a name="p61691806371"></a>查询组织下镜像仓库的概要信息，包括仓库ID、组织ID、仓库名称、仓库描述信息、仓库创建者、仓库大小、镜像pull路径等。</p>
</td>
</tr>
<tr id="row2087254219512"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p0795050194818"><a name="p0795050194818"></a><a name="p0795050194818"></a><a href="查询镜像仓库列表.md">查询镜像仓库列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p161673011371"><a name="p161673011371"></a><a name="p161673011371"></a>查询镜像仓库列表。</p>
</td>
</tr>
<tr id="row1387219421653"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p2794125004815"><a name="p2794125004815"></a><a name="p2794125004815"></a><a href="查询镜像仓库tag列表.md">查询镜像仓库tag列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p21651406373"><a name="p21651406373"></a><a name="p21651406373"></a>查询某一个镜像仓库的所有镜像版本。</p>
</td>
</tr>
<tr id="row20873042758"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p6793450104811"><a name="p6793450104811"></a><a name="p6793450104811"></a><a href="删除指定tag的镜像.md">删除指定tag的镜像</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p8165140173719"><a name="p8165140173719"></a><a name="p8165140173719"></a>删除镜像仓库中指定tag的镜像。</p>
</td>
</tr>
<tr id="row16259104105216"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p122608416524"><a name="p122608416524"></a><a name="p122608416524"></a><a href="生成临时登录指令.md">生成临时登录指令</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p64081653142219"><a name="p64081653142219"></a><a name="p64081653142219"></a>通过获取响应消息头的X-Swr-Dockerlogin的值及响应消息体的host值，可生成临时登录指令。</p>
</td>
</tr>
<tr id="row191740203579"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p1617512015712"><a name="p1617512015712"></a><a name="p1617512015712"></a><a href="创建共享帐号.md">创建共享帐号</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p13176220165710"><a name="p13176220165710"></a><a name="p13176220165710"></a>创建共享帐号。镜像上传后，您可以共享<span class="keyword" id="keyword149651164212"><a name="keyword149651164212"></a><a name="keyword149651164212"></a>私有镜像</span>给其他帐号，并授予下载该镜像的权限。</p>
</td>
</tr>
<tr id="row0364155612568"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p736595615610"><a name="p736595615610"></a><a name="p736595615610"></a><a href="删除共享帐号.md">删除共享帐号</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p129123259110"><a name="p129123259110"></a><a name="p129123259110"></a>删除共享帐号。</p>
</td>
</tr>
<tr id="row941674820567"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p18418134820563"><a name="p18418134820563"></a><a name="p18418134820563"></a><a href="更新共享帐号.md">更新共享帐号</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p103461628015"><a name="p103461628015"></a><a name="p103461628015"></a>更新共享帐号。</p>
</td>
</tr>
<tr id="row71481415924"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p514917153219"><a name="p514917153219"></a><a name="p514917153219"></a><a href="判断共享帐号是否存在.md">判断共享帐号是否存在</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p51499156219"><a name="p51499156219"></a><a name="p51499156219"></a>判断共享帐号是否存在。</p>
</td>
</tr>
<tr id="row207281881322"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p1731148728"><a name="p1731148728"></a><a name="p1731148728"></a><a href="获取共享帐号列表.md">获取共享帐号列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p47313817219"><a name="p47313817219"></a><a name="p47313817219"></a>获取共享帐号列表。</p>
</td>
</tr>
<tr id="row1295416574198"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p45251171204"><a name="p45251171204"></a><a name="p45251171204"></a><a href="查看共享镜像列表.md">查看共享镜像列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p11525197112013"><a name="p11525197112013"></a><a name="p11525197112013"></a>查看共享镜像列表。</p>
</td>
</tr>
<tr id="row109551357181911"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p95265792016"><a name="p95265792016"></a><a name="p95265792016"></a><a href="查询所有API版本信息.md">查询所有API版本信息</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p195261076209"><a name="p195261076209"></a><a name="p195261076209"></a>查询容器镜像服务所有可用的API版本信息列表。</p>
</td>
</tr>
<tr id="row1295535710193"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p05261876202"><a name="p05261876202"></a><a name="p05261876202"></a><a href="查询指定API版本信息.md">查询指定API版本信息</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p155261579206"><a name="p155261579206"></a><a name="p155261579206"></a>查询容器镜像服务指定API版本信息列表。</p>
</td>
</tr>
<tr id="row1681441205812"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p5814416584"><a name="p5814416584"></a><a name="p5814416584"></a><a href="创建组织权限.md">创建组织权限</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p781417135817"><a name="p781417135817"></a><a name="p781417135817"></a>为组织添加授权，使某些用户可以管理/编辑/读取该组织下的镜像。</p>
</td>
</tr>
<tr id="row281418165819"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p481431145812"><a name="p481431145812"></a><a name="p481431145812"></a><a href="删除组织权限.md">删除组织权限</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p1681441175818"><a name="p1681441175818"></a><a name="p1681441175818"></a>删除某些用户对组织的操作权限。</p>
</td>
</tr>
<tr id="row12814917588"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p18147113583"><a name="p18147113583"></a><a name="p18147113583"></a><a href="更新组织权限.md">更新组织权限</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p1081410110585"><a name="p1081410110585"></a><a name="p1081410110585"></a>更新某些用户对组织的操作权限类型。</p>
</td>
</tr>
<tr id="row15903376582"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p89031771584"><a name="p89031771584"></a><a name="p89031771584"></a><a href="查询组织权限.md">查询组织权限</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p17903278585"><a name="p17903278585"></a><a name="p17903278585"></a>查询组织权限。</p>
</td>
</tr>
<tr id="row69032715819"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p179032715816"><a name="p179032715816"></a><a name="p179032715816"></a><a href="创建镜像权限.md">创建镜像权限</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p109031473587"><a name="p109031473587"></a><a name="p109031473587"></a>为镜像授权，使某些用户可以管理/编辑/读取该镜像。</p>
</td>
</tr>
<tr id="row209039711585"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p19039795810"><a name="p19039795810"></a><a name="p19039795810"></a><a href="删除镜像权限.md">删除镜像权限</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p159037715814"><a name="p159037715814"></a><a name="p159037715814"></a>删除某些用户对镜像的操作权限。</p>
</td>
</tr>
<tr id="row1290317712583"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p89031175588"><a name="p89031175588"></a><a name="p89031175588"></a><a href="更新镜像权限.md">更新镜像权限</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="a7005bd3228d34f8ea0fb7b75b17cfbb2"><a name="a7005bd3228d34f8ea0fb7b75b17cfbb2"></a><a name="a7005bd3228d34f8ea0fb7b75b17cfbb2"></a>更新某些用户对镜像的操作权限类型。</p>
</td>
</tr>
<tr id="row20903127145810"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p08621419155915"><a name="p08621419155915"></a><a name="p08621419155915"></a><a href="查询镜像权限.md">查询镜像权限</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p1790314710582"><a name="p1790314710582"></a><a name="p1790314710582"></a>查询镜像的权限。</p>
</td>
</tr>
<tr id="row97891428362"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p2790184223616"><a name="p2790184223616"></a><a name="p2790184223616"></a><a href="获取镜像同步任务信息.md">获取镜像同步任务信息</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p19790184263613"><a name="p19790184263613"></a><a name="p19790184263613"></a>获取镜像同步任务信息。</p>
</td>
</tr>
<tr id="row637353143615"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p12379531361"><a name="p12379531361"></a><a name="p12379531361"></a><a href="获取镜像自动同步任务列表.md">获取镜像自动同步任务列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p438195383614"><a name="p438195383614"></a><a name="p438195383614"></a>获取镜像自动同步任务列表。</p>
</td>
</tr>
<tr id="row198006556361"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p1801155519361"><a name="p1801155519361"></a><a name="p1801155519361"></a><a href="创建镜像自动同步任务.md">创建镜像自动同步任务</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p8765363429"><a name="p8765363429"></a><a name="p8765363429"></a>创建镜像自动同步任务。</p>
</td>
</tr>
<tr id="row1434194512361"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p1434174511366"><a name="p1434174511366"></a><a name="p1434174511366"></a><a href="删除镜像自动同步任务.md">删除镜像自动同步任务</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p834154518363"><a name="p834154518363"></a><a name="p834154518363"></a>删除镜像自动同步任务。</p>
</td>
</tr>
<tr id="row194571823372"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p1345719223710"><a name="p1345719223710"></a><a name="p1345719223710"></a><a href="手动同步镜像.md">手动同步镜像</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p5458202113718"><a name="p5458202113718"></a><a name="p5458202113718"></a>手动触发镜像同步。</p>
</td>
</tr>
<tr id="row845815210377"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p114583293710"><a name="p114583293710"></a><a name="p114583293710"></a><a href="创建触发器.md">创建触发器</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p7458525372"><a name="p7458525372"></a><a name="p7458525372"></a>创建触发器。</p>
</td>
</tr>
<tr id="row1645810203713"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p445819211372"><a name="p445819211372"></a><a name="p445819211372"></a><a href="获取镜像仓库下的触发器列表.md">获取镜像仓库下的触发器列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p4902125214424"><a name="p4902125214424"></a><a name="p4902125214424"></a>获取镜像仓库下的触发器列表。</p>
</td>
</tr>
<tr id="row94584253711"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p124587233718"><a name="p124587233718"></a><a name="p124587233718"></a><a href="删除触发器.md">删除触发器</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p1651217572423"><a name="p1651217572423"></a><a name="p1651217572423"></a>删除触发器。</p>
</td>
</tr>
<tr id="row5525168103710"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p052568133719"><a name="p052568133719"></a><a name="p052568133719"></a><a href="获取触发器详情.md">获取触发器详情</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p18525108193718"><a name="p18525108193718"></a><a name="p18525108193718"></a>获取触发器详情。</p>
</td>
</tr>
<tr id="row952538183716"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p115254811377"><a name="p115254811377"></a><a name="p115254811377"></a><a href="更新触发器配置.md">更新触发器配置</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p9526687370"><a name="p9526687370"></a><a name="p9526687370"></a>更新触发器的状态。</p>
</td>
</tr>
<tr id="row195267883718"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p752648113717"><a name="p752648113717"></a><a name="p752648113717"></a><a href="创建镜像老化规则.md">创建镜像老化规则</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p4526582372"><a name="p4526582372"></a><a name="p4526582372"></a>创建镜像老化规则。</p>
</td>
</tr>
<tr id="row1652620843713"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p1752613853713"><a name="p1752613853713"></a><a name="p1752613853713"></a><a href="获取镜像老化规则列表.md">获取镜像老化规则列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p052698183712"><a name="p052698183712"></a><a name="p052698183712"></a>获取镜像老化规则列表。</p>
</td>
</tr>
<tr id="row105261286374"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p352610814374"><a name="p352610814374"></a><a name="p352610814374"></a><a href="删除镜像老化规则.md">删除镜像老化规则</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p55268813376"><a name="p55268813376"></a><a name="p55268813376"></a>删除镜像老化规则。</p>
</td>
</tr>
<tr id="row1052611812373"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p852648203715"><a name="p852648203715"></a><a name="p852648203715"></a><a href="获取镜像老化规则记录.md">获取镜像老化规则记录</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p952628103716"><a name="p952628103716"></a><a name="p952628103716"></a>获取镜像老化规则记录。</p>
</td>
</tr>
<tr id="row12526158183710"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p195266811379"><a name="p195266811379"></a><a name="p195266811379"></a><a href="修改镜像老化规则.md">修改镜像老化规则</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p252617833710"><a name="p252617833710"></a><a name="p252617833710"></a>修改镜像老化规则。</p>
</td>
</tr>
<tr id="row75268813716"><td class="cellrowborder" valign="top" width="32%" headers="mcps1.2.3.1.1 "><p id="p352616853712"><a name="p352616853712"></a><a name="p352616853712"></a><a href="获取镜像老化记录.md">获取镜像老化记录</a></p>
</td>
<td class="cellrowborder" valign="top" width="68%" headers="mcps1.2.3.1.2 "><p id="p852698143712"><a name="p852698143712"></a><a name="p852698143712"></a>获取镜像老化记录。</p>
</td>
</tr>
</tbody>
</table>

