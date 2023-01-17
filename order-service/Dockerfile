FROM openjdk:8u102-jdk
COPY ./app.jar /tmp/app.jar
ENTRYPOINT java -Xdebug -Xrunjdwp:transport=dt_socket,server=y,suspend=n,address=9002 -jar /tmp/app.jar