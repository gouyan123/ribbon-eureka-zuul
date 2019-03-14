FROM 47.110.53.235:8089/shanglv51/java:v0.2

#将本地文件挂载到当前容器
VOLUME /tmp
# 将当前目录下的*.jar添加到镜像中去，并且命名为app.jar
ADD *.jar app.jar
# 镜像启动的时候执行这个命令
ENTRYPOINT java ${JAVA_OPTS} -Djava.security.egd=file:/dev/./urandom -jar /app.jar