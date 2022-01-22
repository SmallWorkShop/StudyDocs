# 安装postgresql
```shell
# 1. 下载镜像文件
docker pull postgres:9.6.24

# 2. 启动容器
docker run --name dev-postgres -e POSTGRES_PASSWORD=zz123456 -p 5432:5432 -d postgres:9.6.24



```