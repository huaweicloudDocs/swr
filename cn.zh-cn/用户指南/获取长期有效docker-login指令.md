# 获取长期有效docker login指令<a name="swr_01_1000"></a>

本章节介绍如何获取长期有效的docker login指令，长期有效的docker login指令代指一年不会过期的登录指令。

## 操作步骤<a name="section140815918599"></a>

1.  <a name="li5768123671815"></a>获取镜像仓库访问地址、区域项目名称。
    1.  访问[我的凭证](https://console.huaweicloud.com/iam/?locale=zh-cn#/myCredential)。
    2.  在“API凭证”的项目列表中查找当前区域对应的项目。

        如下图所示，“华北-北京一“对应的项目为“cn-north-1“。

        **图 1**  区域与项目<a name="fig1548146070"></a>  
        ![](figures/区域与项目.png "区域与项目")

        镜像仓库地址为 : swr.区域项目名称.myhuaweicloud.com，如中国华北区1对应的镜像仓库地址为：swr.cn-north-1.myhuaweicloud.com。

2.  <a name="li1863783911295"></a>获取AK/SK访问密钥。

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >访问密钥即AK/SK（Access Key ID/Secret Access Key），表示一组密钥对，用于验证调用API发起请求的访问者身份，与密码的功能相似。如果您已有AK/SK，可以直接使用，无需再次获取。  

    1.  访问[我的凭证](https://console.huaweicloud.com/iam/?locale=zh-cn#/myCredential)。
    2.  在左侧导航栏中选择“访问密钥”，单击“新增访问密钥”。
    3.  输入当前用户的登录密码，并通过邮箱或者手机进行验证。

        >![](public_sys-resources/icon-note.gif) **说明：**   
        >在统一身份认证服务中创建的用户，如果创建时未填写邮箱或者手机号，则只需校验登录密码。  

    4.  单击“确定”，下载访问密钥，其中包含AK和SK。

        >![](public_sys-resources/icon-note.gif) **说明：**   
        >为防止访问密钥泄露，建议您将其保存到安全的位置。  


3.  <a name="li132430753010"></a>登录一台linux系统的计算机，执行如下命令获取登录密钥。

    **printf "_$AK_" | openssl dgst -binary -sha256 -hmac "_$SK_" | od -An -vtx1 | sed 's/\[ \\n\]//g' | sed 'N;s/\\n//'**

    其中$AK和$SK为[2](#li1863783911295)获取的AK/SK。

    **图 2**  示例<a name="fig56444333813"></a>  
    ![](figures/示例.png "示例")

4.  使用如下的格式拼接docker login指令。

    **docker login -u  **\[_区域项目名_\]**@**\[_AK_\]**  -p **  \[_登录密钥_\]  \[_镜像仓库地址_\]

    其中，区域项目名和镜像仓库地址在[1](#li5768123671815)中获取，AK在[2](#li1863783911295)中获取，登录密钥为[3](#li132430753010)的执行结果。

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >登录密钥字符串是经过加密的，无法逆向解密，从-p无法获取到SK。  
    >获取的docker login指令可在其他机器上使用并登录。  

5.  使用  **history -c**  命令清理相关使用痕迹，避免隐私信息泄露，为保证安全，获取docker login指令过程建议在开发环境执行。

