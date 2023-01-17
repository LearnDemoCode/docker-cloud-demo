FROM openjdk:8u102-jdk

#设置时区
ENV TimeZone=Asia/Shanghai

#暴露端口
EXPOSE 9001
EXPOSE 10010

COPY ./app.jar /tmp/app.jar

#启动jar
ENTRYPOINT ["java", "-jar","-agentlib:jdwp=transport=dt_socket,server=y,suspend=n,address=9001","/tmp/app.jar"]
