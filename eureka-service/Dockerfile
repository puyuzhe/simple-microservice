#起始镜像
FROM java:8-jdk-alpine

#维护者信息
MAINTAINER pyz

# 执行命令(修改下时区)
RUN  apk add -U tzdata && \
     ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime

#copy
COPY target/eureka-service.jar ./

#指定端口
EXPOSE 6379

#执行启动
CMD java -jar /eureka-service.jar