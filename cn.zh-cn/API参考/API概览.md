# API概览<a name="swr_02_0065"></a>

通过使用容器镜像服务提供的接口，您可以实现对组织、镜像仓库、镜像信息的查询，也可以实现对组织、镜像仓库、镜像的管理操作。

## 组织管理<a name="section1131612414306"></a>

|**API**|**说明**|
|--|--|
|创建组织|创建组织。|
|删除组织|删除组织。|
|查询组织列表|查询组织列表。|
|获取组织详情|查询某个组织的详细信息，包括组织ID、组织名称、创建者和用户权限。|


## 镜像仓库管理<a name="section4932103819336"></a>

<a name="table3913195215332"></a>
<table><tbody><tr id="row2913115215330"><td class="cellrowborder" valign="top" width="38.59%"><p id="p155145914280"><a name="p155145914280"></a><a name="p155145914280"></a><strong id="b4282191718249"><a name="b4282191718249"></a><a name="b4282191718249"></a>API</strong></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p1254915972814"><a name="p1254915972814"></a><a name="p1254915972814"></a><strong id="b2285161722412"><a name="b2285161722412"></a><a name="b2285161722412"></a>说明</strong></p>
</td>
</tr>
<tr id="row49131252163315"><td class="cellrowborder" valign="top" width="38.59%"><p id="p16387155134819"><a name="p16387155134819"></a><a name="p16387155134819"></a><a href="在组织下创建镜像仓库.md">在组织下创建镜像仓库</a></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p173871455144811"><a name="p173871455144811"></a><a name="p173871455144811"></a>在组织下创建镜像仓库。</p>
</td>
</tr>
<tr id="row1913125213337"><td class="cellrowborder" valign="top" width="38.59%"><p id="p3643453174816"><a name="p3643453174816"></a><a name="p3643453174816"></a><a href="删除组织下的镜像仓库.md">删除组织下的镜像仓库</a></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p0643175315481"><a name="p0643175315481"></a><a name="p0643175315481"></a>删除组织下的镜像仓库。</p>
</td>
</tr>
<tr id="row1191335219339"><td class="cellrowborder" valign="top" width="38.59%"><p id="p207961550184814"><a name="p207961550184814"></a><a name="p207961550184814"></a><a href="更新镜像仓库的概要信息.md">更新镜像仓库的概要信息</a></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p121701508378"><a name="p121701508378"></a><a name="p121701508378"></a>更新组织下的镜像仓库概要信息，包括镜像类型、是否公有、描述信息。</p>
</td>
</tr>
<tr id="row15913952153311"><td class="cellrowborder" valign="top" width="38.59%"><p id="p9795250174816"><a name="p9795250174816"></a><a name="p9795250174816"></a><a href="查询镜像仓库概要信息.md">查询镜像仓库概要信息</a></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p61691806371"><a name="p61691806371"></a><a name="p61691806371"></a>查询组织下镜像仓库的概要信息，包括仓库ID、组织ID、仓库名称、仓库描述信息、仓库创建者、仓库大小、镜像pull路径等。</p>
</td>
</tr>
<tr id="row119131352103310"><td class="cellrowborder" valign="top" width="38.59%"><p id="p0795050194818"><a name="p0795050194818"></a><a name="p0795050194818"></a><a href="查询镜像仓库列表.md">查询镜像仓库列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p161673011371"><a name="p161673011371"></a><a name="p161673011371"></a>查询镜像仓库列表。</p>
</td>
</tr>
<tr id="row16914195212339"><td class="cellrowborder" valign="top" width="38.59%"><p id="p45251171204"><a name="p45251171204"></a><a name="p45251171204"></a><a href="查询共享镜像列表.md">查看共享镜像列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p11525197112013"><a name="p11525197112013"></a><a name="p11525197112013"></a>查看共享镜像列表。</p>
</td>
</tr>
</tbody>
</table>

## 镜像版本管理<a name="section333842216348"></a>

<a name="table1121125913341"></a>
<table><tbody><tr id="row1121195943415"><td class="cellrowborder" valign="top" width="38.59%"><p id="p12361432193310"><a name="p12361432193310"></a><a name="p12361432193310"></a><strong id="b1187851452818"><a name="b1187851452818"></a><a name="b1187851452818"></a>API</strong></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p1735617327334"><a name="p1735617327334"></a><a name="p1735617327334"></a><strong id="b138821814162816"><a name="b138821814162816"></a><a name="b138821814162816"></a>说明</strong></p>
</td>
</tr>
<tr id="row82127597346"><td class="cellrowborder" valign="top" width="38.59%"><p id="p2794125004815"><a name="p2794125004815"></a><a name="p2794125004815"></a><a href="查询镜像tag列表.md">查询镜像tag列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p21651406373"><a name="p21651406373"></a><a name="p21651406373"></a>查询某一个镜像仓库的所有镜像版本。</p>
</td>
</tr>
<tr id="row182128599341"><td class="cellrowborder" valign="top" width="38.59%"><p id="p6793450104811"><a name="p6793450104811"></a><a name="p6793450104811"></a><a href="删除指定tag的镜像.md">删除指定tag的镜像</a></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p8165140173719"><a name="p8165140173719"></a><a name="p8165140173719"></a>删除镜像仓库中指定tag的镜像。</p>
</td>
</tr>
</tbody>
</table>

## 共享账号管理<a name="section647115972814"></a>

<a name="table158841013295"></a>
<table><tbody><tr id="row115891104290"><td class="cellrowborder" valign="top" width="38.59%"><p id="p71541167341"><a name="p71541167341"></a><a name="p71541167341"></a><strong id="b1699463682817"><a name="b1699463682817"></a><a name="b1699463682817"></a>API</strong></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p16153181623410"><a name="p16153181623410"></a><a name="p16153181623410"></a><strong id="b189981936192815"><a name="b189981936192815"></a><a name="b189981936192815"></a>说明</strong></p>
</td>
</tr>
<tr id="row258971062916"><td class="cellrowborder" valign="top" width="38.59%"><p id="p1617512015712"><a name="p1617512015712"></a><a name="p1617512015712"></a><a href="创建共享帐号.md">创建共享帐号</a></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p13176220165710"><a name="p13176220165710"></a><a name="p13176220165710"></a>创建共享帐号。镜像上传后，您可以共享<span class="keyword" id="keyword149651164212"><a name="keyword149651164212"></a><a name="keyword149651164212"></a>私有镜像</span>给其他帐号，并授予下载该镜像的权限。</p>
</td>
</tr>
<tr id="row9589151019293"><td class="cellrowborder" valign="top" width="38.59%"><p id="p736595615610"><a name="p736595615610"></a><a name="p736595615610"></a><a href="删除共享帐号.md">删除共享帐号</a></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p129123259110"><a name="p129123259110"></a><a name="p129123259110"></a>删除共享帐号。</p>
</td>
</tr>
<tr id="row12589171022912"><td class="cellrowborder" valign="top" width="38.59%"><p id="p18418134820563"><a name="p18418134820563"></a><a name="p18418134820563"></a><a href="更新共享帐号.md">更新共享帐号</a></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p103461628015"><a name="p103461628015"></a><a name="p103461628015"></a>更新共享帐号。</p>
</td>
</tr>
<tr id="row195891510172911"><td class="cellrowborder" valign="top" width="38.59%"><p id="p514917153219"><a name="p514917153219"></a><a name="p514917153219"></a><a href="判断共享帐号是否存在.md">判断共享帐号是否存在</a></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p51499156219"><a name="p51499156219"></a><a name="p51499156219"></a>判断共享帐号是否存在。</p>
</td>
</tr>
<tr id="row2589141032917"><td class="cellrowborder" valign="top" width="38.59%"><p id="p1731148728"><a name="p1731148728"></a><a name="p1731148728"></a><a href="获取共享帐号列表.md">获取共享帐号列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p47313817219"><a name="p47313817219"></a><a name="p47313817219"></a>获取共享帐号列表。</p>
</td>
</tr>
</tbody>
</table>

## API版本信息<a name="section23842042162916"></a>

<a name="table92329542292"></a>
<table><tbody><tr id="row132321054112912"><td class="cellrowborder" valign="top" width="38.59%"><p id="p1987234172812"><a name="p1987234172812"></a><a name="p1987234172812"></a><strong id="b193231342303"><a name="b193231342303"></a><a name="b193231342303"></a>API</strong></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p286834118284"><a name="p286834118284"></a><a name="p286834118284"></a><strong id="b132514413018"><a name="b132514413018"></a><a name="b132514413018"></a>说明</strong></p>
</td>
</tr>
<tr id="row523275411294"><td class="cellrowborder" valign="top" width="38.59%"><p id="p95265792016"><a name="p95265792016"></a><a name="p95265792016"></a><a href="查询所有API版本信息.md">查询所有API版本信息</a></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p195261076209"><a name="p195261076209"></a><a name="p195261076209"></a>查询容器镜像服务所有可用的API版本信息列表。</p>
</td>
</tr>
<tr id="row123310543292"><td class="cellrowborder" valign="top" width="38.59%"><p id="p05261876202"><a name="p05261876202"></a><a name="p05261876202"></a><a href="查询指定API版本信息.md">查询指定API版本信息</a></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p155261579206"><a name="p155261579206"></a><a name="p155261579206"></a>查询容器镜像服务指定API版本信息列表。</p>
</td>
</tr>
</tbody>
</table>

## 组织权限管理<a name="section10399203033012"></a>

<a name="table1520663712304"></a>
<table><tbody><tr id="row67322333319"><td class="cellrowborder" valign="top" width="38.59%"><p id="p1973318332318"><a name="p1973318332318"></a><a name="p1973318332318"></a><strong id="b1571610442317"><a name="b1571610442317"></a><a name="b1571610442317"></a>API</strong></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p2073343303115"><a name="p2073343303115"></a><a name="p2073343303115"></a><strong id="b872084417315"><a name="b872084417315"></a><a name="b872084417315"></a>说明</strong></p>
</td>
</tr>
<tr id="row220733743014"><td class="cellrowborder" valign="top" width="38.59%"><p id="p5814416584"><a name="p5814416584"></a><a name="p5814416584"></a><a href="创建组织权限.md">创建组织权限</a></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p781417135817"><a name="p781417135817"></a><a name="p781417135817"></a>为组织添加授权，使某些用户可以管理/编辑/读取该组织下的镜像。</p>
</td>
</tr>
<tr id="row1720711377307"><td class="cellrowborder" valign="top" width="38.59%"><p id="p481431145812"><a name="p481431145812"></a><a name="p481431145812"></a><a href="删除组织权限.md">删除组织权限</a></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p1681441175818"><a name="p1681441175818"></a><a name="p1681441175818"></a>删除某些用户对组织的操作权限。</p>
</td>
</tr>
<tr id="row1620723773015"><td class="cellrowborder" valign="top" width="38.59%"><p id="p18147113583"><a name="p18147113583"></a><a name="p18147113583"></a><a href="更新组织权限.md">更新组织权限</a></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p1081410110585"><a name="p1081410110585"></a><a name="p1081410110585"></a>更新某些用户对组织的操作权限类型。</p>
</td>
</tr>
<tr id="row37851959123016"><td class="cellrowborder" valign="top" width="38.59%"><p id="p89031771584"><a name="p89031771584"></a><a name="p89031771584"></a><a href="查询组织权限.md">查询组织权限</a></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p17903278585"><a name="p17903278585"></a><a name="p17903278585"></a>查询组织权限。</p>
</td>
</tr>
</tbody>
</table>

## 镜像权限管理<a name="section5665118133117"></a>

<a name="table14776526103114"></a>
<table><tbody><tr id="row1494524973120"><td class="cellrowborder" valign="top" width="38.59%"><p id="p79451649113114"><a name="p79451649113114"></a><a name="p79451649113114"></a><strong id="b025320313329"><a name="b025320313329"></a><a name="b025320313329"></a>API</strong></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p139455496317"><a name="p139455496317"></a><a name="p139455496317"></a><strong id="b132572320321"><a name="b132572320321"></a><a name="b132572320321"></a>说明</strong></p>
</td>
</tr>
<tr id="row077682611315"><td class="cellrowborder" valign="top" width="38.59%"><p id="p179032715816"><a name="p179032715816"></a><a name="p179032715816"></a><a href="创建镜像权限.md">创建镜像权限</a></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p109031473587"><a name="p109031473587"></a><a name="p109031473587"></a>为镜像授权，使某些用户可以管理/编辑/读取该镜像。</p>
</td>
</tr>
<tr id="row77779262311"><td class="cellrowborder" valign="top" width="38.59%"><p id="p19039795810"><a name="p19039795810"></a><a name="p19039795810"></a><a href="删除镜像权限.md">删除镜像权限</a></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p159037715814"><a name="p159037715814"></a><a name="p159037715814"></a>删除某些用户对镜像的操作权限。</p>
</td>
</tr>
<tr id="row1777792673119"><td class="cellrowborder" valign="top" width="38.59%"><p id="p89031175588"><a name="p89031175588"></a><a name="p89031175588"></a><a href="更新镜像权限.md">更新镜像权限</a></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="a7005bd3228d34f8ea0fb7b75b17cfbb2"><a name="a7005bd3228d34f8ea0fb7b75b17cfbb2"></a><a name="a7005bd3228d34f8ea0fb7b75b17cfbb2"></a>更新某些用户对镜像的操作权限类型。</p>
</td>
</tr>
<tr id="row67772267313"><td class="cellrowborder" valign="top" width="38.59%"><p id="p08621419155915"><a name="p08621419155915"></a><a name="p08621419155915"></a><a href="查询镜像权限.md">查询镜像权限</a></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p1790314710582"><a name="p1790314710582"></a><a name="p1790314710582"></a>查询镜像的权限。</p>
</td>
</tr>
</tbody>
</table>

## 镜像自动同步管理<a name="section7557751144111"></a>

<a name="table1488813044211"></a>
<table><tbody><tr id="row988810114220"><td class="cellrowborder" valign="top" width="38.59%"><p id="p105008103313"><a name="p105008103313"></a><a name="p105008103313"></a><strong id="b231041811423"><a name="b231041811423"></a><a name="b231041811423"></a>API</strong></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p9498141010318"><a name="p9498141010318"></a><a name="p9498141010318"></a><strong id="b33115180422"><a name="b33115180422"></a><a name="b33115180422"></a>说明</strong></p>
</td>
</tr>
<tr id="row19889609425"><td class="cellrowborder" valign="top" width="38.59%"><p id="p2790184223616"><a name="p2790184223616"></a><a name="p2790184223616"></a><a href="获取镜像自动同步任务信息.md">获取镜像自动同步任务信息</a></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p195353531029"><a name="p195353531029"></a><a name="p195353531029"></a>创建镜像自动同步任务后，可以通过此接口查询该任务的状态，以判断是否同步成功。</p>
</td>
</tr>
<tr id="row13889120204217"><td class="cellrowborder" valign="top" width="38.59%"><p id="p12379531361"><a name="p12379531361"></a><a name="p12379531361"></a><a href="获取镜像自动同步任务列表.md">获取镜像自动同步任务列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p564817535212"><a name="p564817535212"></a><a name="p564817535212"></a>获取为当前镜像仓库所创建的所有自动同步任务。</p>
</td>
</tr>
<tr id="row106111345542"><td class="cellrowborder" valign="top" width="38.59%"><p id="p1801155519361"><a name="p1801155519361"></a><a name="p1801155519361"></a><a href="创建镜像自动同步任务.md">创建镜像自动同步任务</a></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p1374485320215"><a name="p1374485320215"></a><a name="p1374485320215"></a>创建镜像自动同步任务，帮助您把最新推送的镜像自动同步到其他区域镜像仓库内。 镜像自动同步帮助您把最新推送的镜像自动同步到其他区域镜像仓库内，后期镜像有更新时，目标仓库的镜像也会自动更新，但已有的镜像不会自动同步。已有镜像的同步需要手动操作，详情请参见<a href="手动同步镜像.md">手动同步镜像</a>。</p>
</td>
</tr>
<tr id="row9611545643"><td class="cellrowborder" valign="top" width="38.59%"><p id="p1434174511366"><a name="p1434174511366"></a><a name="p1434174511366"></a><a href="删除镜像自动同步任务.md">删除镜像自动同步任务</a></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p834154518363"><a name="p834154518363"></a><a name="p834154518363"></a>根据目标区域、目标组织删除指定的镜像自动同步任务。</p>
</td>
</tr>
<tr id="row861024519418"><td class="cellrowborder" valign="top" width="38.59%"><p id="p1345719223710"><a name="p1345719223710"></a><a name="p1345719223710"></a><a href="手动同步镜像.md">手动同步镜像</a></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p185267131641"><a name="p185267131641"></a><a name="p185267131641"></a>对于镜像仓库已有的镜像，如果想在其他区域使用，需要手动触发镜像同步。判断是否同步成功的方法如下：</p>
<a name="ul03919591549"></a><a name="ul03919591549"></a><ul id="ul03919591549"><li>响应状态码为200，无报错信息，表示同步成功。</li><li>通过SWR管理控制台或调用<a href="查询镜像仓库概要信息.md">查询镜像仓库概要信息</a>接口，在目标区域的目标组织下，若存在所同步的镜像版本表示同步成功。</li></ul>
</td>
</tr>
</tbody>
</table>

## 触发器管理<a name="section921411254619"></a>

<a name="table13969133414610"></a>
<table><tbody><tr id="row189691534266"><td class="cellrowborder" valign="top" width="38.59%"><p id="p9921030647"><a name="p9921030647"></a><a name="p9921030647"></a><strong id="b866917481962"><a name="b866917481962"></a><a name="b866917481962"></a>API</strong></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p1291953016418"><a name="p1291953016418"></a><a name="p1291953016418"></a><strong id="b36711548369"><a name="b36711548369"></a><a name="b36711548369"></a>说明</strong></p>
</td>
</tr>
<tr id="row129691634565"><td class="cellrowborder" valign="top" width="38.59%"><p id="p114583293710"><a name="p114583293710"></a><a name="p114583293710"></a><a href="创建触发器.md">创建触发器</a></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p7458525372"><a name="p7458525372"></a><a name="p7458525372"></a>创建触发器。</p>
</td>
</tr>
<tr id="row2096914341269"><td class="cellrowborder" valign="top" width="38.59%"><p id="p445819211372"><a name="p445819211372"></a><a name="p445819211372"></a><a href="获取镜像仓库下的触发器列表.md">获取镜像仓库下的触发器列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p4902125214424"><a name="p4902125214424"></a><a name="p4902125214424"></a>获取镜像仓库下的触发器列表。</p>
</td>
</tr>
<tr id="row1196916347615"><td class="cellrowborder" valign="top" width="38.59%"><p id="p124587233718"><a name="p124587233718"></a><a name="p124587233718"></a><a href="删除触发器.md">删除触发器</a></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p1651217572423"><a name="p1651217572423"></a><a name="p1651217572423"></a>删除触发器。</p>
</td>
</tr>
<tr id="row79708345611"><td class="cellrowborder" valign="top" width="38.59%"><p id="p052568133719"><a name="p052568133719"></a><a name="p052568133719"></a><a href="获取触发器详情.md">获取触发器详情</a></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p18525108193718"><a name="p18525108193718"></a><a name="p18525108193718"></a>获取触发器详情。</p>
</td>
</tr>
<tr id="row397013341667"><td class="cellrowborder" valign="top" width="38.59%"><p id="p115254811377"><a name="p115254811377"></a><a name="p115254811377"></a><a href="更新触发器配置.md">更新触发器配置</a></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p9526687370"><a name="p9526687370"></a><a name="p9526687370"></a>更新触发器的状态。</p>
</td>
</tr>
</tbody>
</table>

## 镜像老化规则管理<a name="section12744881782"></a>

<a name="table2096212179812"></a>
<table><tbody><tr id="row99621817388"><td class="cellrowborder" valign="top" width="38.59%"><p id="p1825124469"><a name="p1825124469"></a><a name="p1825124469"></a><strong id="b14370438484"><a name="b14370438484"></a><a name="b14370438484"></a>API</strong></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p982224065"><a name="p982224065"></a><a name="p982224065"></a><strong id="b9373193810819"><a name="b9373193810819"></a><a name="b9373193810819"></a>说明</strong></p>
</td>
</tr>
<tr id="row29621217185"><td class="cellrowborder" valign="top" width="38.59%"><p id="p752648113717"><a name="p752648113717"></a><a name="p752648113717"></a><a href="创建镜像老化规则.md">创建镜像老化规则</a></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p4526582372"><a name="p4526582372"></a><a name="p4526582372"></a>创建镜像老化规则。</p>
</td>
</tr>
<tr id="row49624171384"><td class="cellrowborder" valign="top" width="38.59%"><p id="p1752613853713"><a name="p1752613853713"></a><a name="p1752613853713"></a><a href="获取镜像老化规则列表.md">获取镜像老化规则列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p052698183712"><a name="p052698183712"></a><a name="p052698183712"></a>获取镜像老化规则列表。</p>
</td>
</tr>
<tr id="row1496311174815"><td class="cellrowborder" valign="top" width="38.59%"><p id="p352610814374"><a name="p352610814374"></a><a name="p352610814374"></a><a href="删除镜像老化规则.md">删除镜像老化规则</a></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p55268813376"><a name="p55268813376"></a><a name="p55268813376"></a>删除镜像老化规则。</p>
</td>
</tr>
<tr id="row1396313171887"><td class="cellrowborder" valign="top" width="38.59%"><p id="p852648203715"><a name="p852648203715"></a><a name="p852648203715"></a><a href="获取镜像老化规则记录.md">获取镜像老化规则记录</a></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p952628103716"><a name="p952628103716"></a><a name="p952628103716"></a>获取镜像老化规则记录。</p>
</td>
</tr>
<tr id="row1796318171687"><td class="cellrowborder" valign="top" width="38.59%"><p id="p195266811379"><a name="p195266811379"></a><a name="p195266811379"></a><a href="修改镜像老化规则.md">修改镜像老化规则</a></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p252617833710"><a name="p252617833710"></a><a name="p252617833710"></a>修改镜像老化规则。</p>
</td>
</tr>
<tr id="row896301717817"><td class="cellrowborder" valign="top" width="38.59%"><p id="p352616853712"><a name="p352616853712"></a><a name="p352616853712"></a><a href="获取镜像老化记录.md">获取镜像老化记录</a></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p852698143712"><a name="p852698143712"></a><a name="p852698143712"></a>获取镜像老化记录。</p>
</td>
</tr>
</tbody>
</table>

## 临时登录指令<a name="section12112125514519"></a>

<a name="table1584213511615"></a>
<table><tbody><tr id="row9843759618"><td class="cellrowborder" valign="top" width="38.59%"><p id="p1115812521575"><a name="p1115812521575"></a><a name="p1115812521575"></a><strong id="b58663181061"><a name="b58663181061"></a><a name="b58663181061"></a>API</strong></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p91550521779"><a name="p91550521779"></a><a name="p91550521779"></a><strong id="b1286812181763"><a name="b1286812181763"></a><a name="b1286812181763"></a>说明</strong></p>
</td>
</tr>
<tr id="row13843251364"><td class="cellrowborder" valign="top" width="38.59%"><p id="p1027733216202"><a name="p1027733216202"></a><a name="p1027733216202"></a><a href="生成临时登录指令.md">生成临时登录指令</a></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p1727783252014"><a name="p1727783252014"></a><a name="p1727783252014"></a>通过获取响应消息头的X-Swr-Dockerlogin的值及响应消息体的host值，可生成临时登录指令。</p>
</td>
</tr>
</tbody>
</table>

## 配额管理<a name="section550910307819"></a>

<a name="table894620422819"></a>
<table><tbody><tr id="row1594712423818"><td class="cellrowborder" valign="top" width="38.59%"><p id="p139091342510"><a name="p139091342510"></a><a name="p139091342510"></a><strong id="b4847352121014"><a name="b4847352121014"></a><a name="b4847352121014"></a>API</strong></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p59085343512"><a name="p59085343512"></a><a name="p59085343512"></a><strong id="b178526522103"><a name="b178526522103"></a><a name="b178526522103"></a>说明</strong></p>
</td>
</tr>
<tr id="row1694711421289"><td class="cellrowborder" valign="top" width="38.59%"><p id="p20277532112016"><a name="p20277532112016"></a><a name="p20277532112016"></a><a href="获取配额信息.md">获取配额信息</a></p>
</td>
<td class="cellrowborder" valign="top" width="61.41%"><p id="p202777323207"><a name="p202777323207"></a><a name="p202777323207"></a>获取配额信息。</p>
</td>
</tr>
</tbody>
</table>

