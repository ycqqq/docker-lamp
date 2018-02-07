# docker-lamp
一个基于docker构建的lamp应用，快速部署你的应用。


**启动应用**

1、安装docker环境。（参考docker文档 https://docs.docker.com/install/linux/docker-ee/centos/#install-docker-ee-1 ）

2、下载当前项目并解压，进入docker-compose.yml所在目录，执行*docker-compose build*构建镜像。

3、执行*docker-compose up -d*启动容器服务。

4、访问 http://localhost:8080 可看到phpinfo信息。

**提示**

1、应用的配置文件都放在对应应用的文件夹下，可以自行修改配置文件，执行*docker-compose build*重新构建镜像。

2、映射端口在docker-compose.yml中可以修改，同样需要重新build。

3、各个应用的日志文件，redis和mysql的数据文件使用共享目录挂载到容器中，文件都在host机对应应用的文件夹下。
