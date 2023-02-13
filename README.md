## 使用方法
到docker-compose.yml文件所在目录中执行命令启动

docker-compose -f [文件名] -p 项目名 up -d

以Redis为例

```shell
docker-compose -f redis-docker-compose.yml -p redis-server up -d
```

加 -p 命令是为了执行多个docker-compose文件时，指定项目名，否则会报错

停止并删除镜像
```shell
docker-compose -f redis-docker-compose.yml -p redis-server down --rmi all
```
