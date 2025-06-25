# You can change this base image to anything else
# But make sure to use the correct version of Java
#FROM adoptopenjdk/openjdk11:alpine-jre
FROM eclipse-temurin
#FROM eclipse-temurin:11-jre-alpine

# Simply the artifact path
ARG artifact=target/demo-0.0.1-SNAPSHOT.jar

WORKDIR /opt/app

COPY ${artifact} app.jar

# This should not be changed
ENTRYPOINT ["java","-jar","app.jar"]
