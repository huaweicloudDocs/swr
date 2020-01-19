# 创建用户并授权使用SWR<a name="swr_01_0072"></a>

如果您需要对您所拥有的容器镜像服务（SWR）进行精细的权限管理，您可以使用[统一身份认证服务](https://support.huaweicloud.com/usermanual-iam/zh-cn_topic_0079496985.html)（Identity and Access Management，简称IAM），通过IAM，您可以：

-   根据企业的业务组织，在您的华为云账号中，给企业中不同职能部门的员工创建IAM用户，让员工拥有唯一安全凭证，并使用SWR资源。
-   根据企业用户的职能，设置不同的访问权限，以达到用户之间的权限隔离。
-   将SWR资源委托给更专业、高效的其他华为云账号或者云服务，这些账号或者云服务可以根据权限进行代运维。

如果华为云账号已经能满足您的要求，不需要创建独立的IAM用户，您可以跳过本章节，不影响您使用SWR服务的其它功能。

本章节为您介绍对用户授权的方法，操作流程如[图1](#fig673713328586)所示。

## 前提条件<a name="section559312413518"></a>

-   “Tenant Administrator”属于策略，请先在IAM控制台中开通基于策略的访问控制公测，开通方法请参见：[申请基于策略的访问控制公测](https://support.huaweicloud.com/usermanual-iam/iam_01_019.html)。
-   给用户组授权之前，请您了解用户组可以添加的SWR权限，并结合实际需求进行选择，SWR支持的系统权限，请参见：[SWR系统权限](https://support.huaweicloud.com/productdesc-swr/swr_03_0005.html)。若您需要对除SWR之外的其它服务授权，IAM支持服务的所有权限请参见[权限策略](https://support.huaweicloud.com/permissions/policy_list.html?product=swr)。

## 示例流程<a name="section1946765275520"></a>

**图 1**  给用户授权SWR权限流程<a name="fig673713328586"></a>  
![](figures/给用户授权SWR权限流程.jpg "给用户授权SWR权限流程")

1.  <a name="li8135822590"></a>[创建用户组并授权](https://support.huaweicloud.com/usermanual-iam/zh-cn_topic_0046611269.html)

    在IAM控制台创建用户组，并授予容器镜像服务的管理员权限“SWR Admin”。

2.  [创建用户并加入用户组](https://support.huaweicloud.com/usermanual-iam/zh-cn_topic_0046611303.html)

    在IAM控制台创建用户，并将其加入[1](#li8135822590)中创建的用户组。

3.  [用户登录](https://support.huaweicloud.com/usermanual-iam/iam_01_0552.html)并验证权限

    新创建的用户登录控制台，切换至授权区域，验证权限：

    -   在“服务列表”中选择容器镜像服务，进入SWR主界面，左侧导航栏中选择“组织管理“，在右侧页面单击“创建组织“，如果能创建组织，说明权限设置成功。


