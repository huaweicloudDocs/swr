# 制作Docker镜像<a name="swr_01_0007"></a>

本节指导用户通过Dockerfile定制一个简单的Web应用程序的Docker镜像。Dockerfile 是一个文本文件，其内包含了一条条的指令\(Instruction\)，每一条指令构建一层，因此每一条指令的内容，就是描述该层应当如何构建。

## 背景信息<a name="section84949264292"></a>

若使用Nginx镜像来创建容器应用，在浏览器访问时则会看到默认的Nginx欢迎页面，本节以Nginx镜像为例，修改Nginx镜像的欢迎页面，定制一个新的镜像，将欢迎页面改为“Hello, SWR!“。

>![](public_sys-resources/icon-note.gif) **说明：**   
>在国内下载DockerHub官方镜像，可通过“registry.docker-cn.com“访问，该镜像托管于中国大陆，本地用户现在将会享受到更快的下载速度和更强的稳定性。具体请参见[https://www.docker-cn.com/registry-mirror](https://www.docker-cn.com/registry-mirror)。  

## 前提条件<a name="section0201103753314"></a>

已安装Docker，如未安装可参见[安装Docker](安装Docker.md)。

## 操作步骤<a name="section1882512312913"></a>

1.  以root用户登录Docker所在机器。
2.  创建一个名为Dockerfile的文件。

    **mkdir mynginx**

    **cd mynginx**

    **touch Dockerfile**

3.  编辑Dockerfile。

    **vim Dockerfile**

    增加文件内容如下：

    ```
    FROM nginx
    RUN echo '<h1>Hello,SWR!</h1>' > /usr/share/nginx/html/index.html
    ```

    Dockerfile指令介绍如下。以下仅介绍简单指令，如需了解更多，请参见官方网站[https://hub.docker.com/](https://hub.docker.com/)。

    -   FROM语句：表示使用nginx镜像作为基础镜像，一个Dockerfile中FROM是必备的指令，并且必须是第一条指令。
    -   RUN语句：格式为RUN <命令\>，表示执行echo命令，在显示器中显示一段“Hello, SWR!“的文字。

4.  构建Docker镜像。

    **docker build -t nginx:v3 .**

    镜像构建的格式为：docker build \[选项\] <上下文路径\>

    -   **-t nginx:v3**：指定镜像的名称和版本。
    -   **.**：指定上下文路径，镜像构建命令将该路径下所有的内容打包给Docker引擎帮助构建镜像。

5.  执行以下命令，可查看到已成功部署的nginx镜像，版本为v3。

    **docker images**


