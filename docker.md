# Docker

## Images

1. 安装镜像： docker pull jenkins/jenkins:lts
1. 查看本机现有镜像：docker images

## Containers

1. 查看已启动的容器：docker ps
1. 查看所有容器：docker ps -a
1. 进入容器：docker attach <container_id>
1. 停止容器：docker stop <container_id>
1. 移除单个容器：docker rm <container_id>
1. 移除多个容器：docker rm <container_id> <container_id>
1. docker run -d --name nginx-demo -p 80:80 -v /Users/allen/nginx/nginx.conf:/etc/nginx/nginx.conf -v /Users/allen/nginx/logs:/var/log/nginx -v /Users/allen/nginx/html:/usr/share/nginx/html -v /Users/allen/nginx/conf:/etc/nginx/conf.d --privileged=true nginx