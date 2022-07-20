# For Java 11, try this
FROM adoptopenjdk/openjdk11:alpine-jre

# Refer to Maven build -> finalName
ARG JAR_FILE=target/spring-boot-web.jar

# cd /opt/app
WORKDIR /opt/app

# cp target/spring-boot-web.jar /opt/app/app.jar
COPY ${JAR_FILE} app.jar

# indicate the application will expose serviceon port 8080
EXPOSE 8080

# java -jar /opt/app/app.jar
ENTRYPOINT ["java","-jar","app.jar"]

# docker build -t spring-boot:1.0 .
# docker run -d -p 8080:8080 -t spring-boot:1.0
# access http://localhost:8080

# cd D:\docker-samples\docker-java
# docker build -t springboot:2.0 -f ./docker-spring-boot/Dockerfile ./docker-spring-boot
