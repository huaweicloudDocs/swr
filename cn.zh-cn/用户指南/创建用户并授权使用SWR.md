# 创建用户并授权使用SWR<a name="swr_01_0072"></a>

如果您需要对您所拥有的容器镜像服务（SWR）进行精细的权限管理，您可以使用[统一身份认证服务](https://support.huaweicloud.com/usermanual-iam/iam_01_0001.html)（Identity and Access Management，简称IAM），通过IAM，您可以：

-   根据企业的业务组织，在您的华为云帐号中，给企业中不同职能部门的员工创建IAM用户，让员工拥有唯一安全凭证，并使用SWR资源。
-   根据企业用户的职能，设置不同的访问权限，以达到用户之间的权限隔离。
-   将SWR资源委托给更专业、高效的其他华为云帐号或者云服务，这些帐号或者云服务可以根据权限进行代运维。

如果华为云帐号已经能满足您的要求，不需要创建独立的IAM用户，您可以跳过本章节，不影响您使用SWR服务的其他功能。

本章节为您介绍对用户授权的方法，操作流程如[图1](#fig5293113815405)所示。

## 前提条件<a name="section559312413518"></a>

给用户组授权之前，请您了解用户组可以添加的SWR权限，并结合实际需求进行选择，SWR支持的系统权限，请参见：[SWR系统权限](https://support.huaweicloud.com/productdesc-swr/swr_03_0005.html)。若您需要对除SWR之外的其他服务授权，IAM支持服务的所有权限请参见[系统权限](https://support.huaweicloud.com/usermanual-permissions/iam_01_0001.html)。

## 示例流程<a name="section1946765275520"></a>

**图 1**  给用户授予SWR权限流程<a name="fig5293113815405"></a>  
![](figures/给用户授予SWR权限流程.png "给用户授予SWR权限流程")

1.  <a name="li8135822590"></a>[创建用户组并授权](https://support.huaweicloud.com/usermanual-iam/iam_03_0001.html)

    在IAM控制台创建用户组，并授予容器镜像服务的管理员权限“SWR Admin“。

2.  [创建用户并加入用户组](https://support.huaweicloud.com/usermanual-iam/iam_02_0001.html)

    在IAM控制台创建用户，并将其加入[1](#li8135822590)中创建的用户组。

3.  [用户登录](https://support.huaweicloud.com/usermanual-iam/iam_01_0552.html)并验证权限

    新创建的用户登录控制台，切换至授权区域，验证权限（如果能顺利完成如下操作，说明权限设置成功）：

    1.  在“服务列表“中选择容器镜像服务，进入SWR主界面。
    2.  在左侧导航栏选择“组织管理“，单击右上角“创建组织“，输入组织名称，能够成功创建组织。
    3.  在左侧导航栏选择“我的镜像“，单击右上角“页面上传“，选择上一步创建的组织，以及一个本地的镜像文件，能够成功上传镜像。


