# Docker基础知识<a name="swr_01_0006"></a>

Docker是一个开源的引擎，可以轻松的为任何应用创建一个轻量级的、可移植的、自给自足的容器。容器镜像服务兼容原生Docker，支持使用Docker CLI和原生API管理容器镜像。

## 安装Docker<a name="section941018533817"></a>

在安装Docker前，请了解Docker的基础知识，具体请参见  [Docker Documentation](https://docs.docker.com)。

Docker几乎支持在所有操作系统上安装，用户可以根据需要选择要安装的Docker版本，具体请参见[https://docs.docker.com/engine/installation/](https://docs.docker.com/engine/installation/)。

>![](public_sys-resources/icon-note.gif) **说明：**   
>-   Docker镜像的的存储可以使用华为云提供的容器镜像服务，由于容器镜像服务支持Docker 1.11.2及以上版本上传镜像，建议下载对应版本。  
>-   安装Docker需要连接互联网，内网服务器需要绑定弹性IP后才能访问。  

另外，在Linux操作系统下，可以使用如下命令快速安装Docker。

```
curl -fsSL get.docker.com -o get-docker.sh
sh get-docker.sh
```

## 制作Docker镜像<a name="section135321459915"></a>

本节指导您通过Dockerfile定制一个简单的Web应用程序的Docker镜像。Dockerfile是一个文本文件，其内包含了一条条的指令（Instruction），每一条指令构建一层，因此每一条指令的内容，就是描述该层应当如何构建。

使用Nginx镜像创建容器应用，在浏览器访问时则会看到默认的Nginx欢迎页面，本节以Nginx镜像为例，修改Nginx镜像的欢迎页面，定制一个新的镜像，将欢迎页面改为“Hello, SWR!“。

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

    Dockerfile指令介绍如下。

    -   FROM语句：表示使用nginx镜像作为基础镜像，一个Dockerfile中FROM是必备的指令，并且必须是第一条指令。
    -   RUN语句：格式为RUN <命令\>，表示执行echo命令，在显示器中显示一段“Hello, SWR!“的文字。

    保存并退出。

4.  使用 docker build \[选项\] <上下文路径\> 构建镜像。

    **docker build -t nginx:v3 .**

    -   -t nginx:v3：指定镜像的名称和版本。
    -   **.**：指定Dockerfile所在目录，镜像构建命令将该路径下所有的内容打包给Docker引擎帮助构建镜像。

5.  执行以下命令，可查看到已成功部署的nginx镜像，版本为v3。

    **docker images**


## 制作镜像压缩包<a name="section3433103111126"></a>

本节指导您将Docker镜像制作成tar或tar.gz文件压缩包。

1.  以root用户登录Docker所在机器。
2.  执行如下命令查看镜像。

    **docker images**

    查看需要导出的镜像及tag。

3.  执行如下命令制作镜像压缩包。

    **docker save \[OPTIONS\] IMAGE \[IMAGE...\]**

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >OPTIONS：--output , -o，表示导出到文件。（可选）  
    >压缩包格式为：.tar或.tar.gz。  

    示例：

    ```
    $ docker save nginx:latest > nginx.tar
    $ ls -sh nginx.tar
    108M nginx.tar
    
    $ docker save php:5-apache > php.tar.gz
    $ ls -sh php.tar.gz
    372M php.tar.gz
    
    $ docker save --output nginx.tar nginx
    $ ls -sh nginx.tar
    108M nginx.tar
    
    $ docker save -o nginx-all.tar nginx
    $ docker save -o nginx-latest.tar nginx:latest
    ```


