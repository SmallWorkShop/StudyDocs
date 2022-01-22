# 安装mysql镜像
```shell
# 下载mysql镜像文件
docker pull mysql:5.7


# 启动mysql容器并且指定端口映射
docker run --name dev-mysql -e MYSQL_ROOT_PASSWORD=zz123456 -p 3306:3306 -d mysql:5.7 


```