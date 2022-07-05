# docker memo

## images
1. 安装镜像： docker pull jenkins/jenkins:lts
2. 查看本机现有镜像：docker images


## containers
1. 查看已启动的容器：docker ps
2. 查看所有容器：docker ps -a
3. 进入容器：docker attach <container_id>
4. 停止容器：docker stop <container_id>
5. 移除单个容器：docker rm <container_id>
6. 移除多个容器：docker rm <container_id> <container_id>
8. docker run -d --name nginx-demo -p 80:80 -v /Users/allen/nginx/nginx.conf:/etc/nginx/nginx.conf -v /Users/allen/nginx/logs:/var/log/nginx -v /Users/allen/nginx/html:/usr/share/nginx/html -v /Users/allen/nginx/conf:/etc/nginx/conf.d --privileged=true nginx
95f56a2878a0c0dd282506fe294e27c51e9d7cf9c21192c6d41fdc95e4c1cb8b
