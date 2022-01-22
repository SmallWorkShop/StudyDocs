# 参考文档
<https://docker.easydoc.net/doc/81170005/cCewZWoN/lTKfePfP>

# 变更docker镜像存储路径
```shell
# 查看当前docker进程状态（状态为stoped可迁移）
wsl --list -v 

# 备份导出当前目录内容
wsl --export docker-desktop D:\Docker\docker-desktop.tar
wsl --export docker-desktop-data D:\Docker\docker-desktop-data.tar

# 删除原有数据
wsl --unregister docker-desktop
wsl --unregister docker-desktop-data

# 导入数据到新目录
wsl --import docker-desktop "D:\Docker\wsl\docker-desktop" "D:\Docker\docker-desktop.tar" --version 2
wsl --import docker-desktop-data "D:\Docker\wsl\docker-desktop-data" "D:\Docker\docker-desktop-data.tar" --version 2

```