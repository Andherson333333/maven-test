
FROM adoptopenjdk/openjdk11:alpine-jre
RUN addgroup -S mygroup && adduser -S myuser -G mygroup
USER myuser
ARG artifact=target/spring-boot-web.jar
WORKDIR /opt/app
COPY ${artifact} app.jar
ENTRYPOINT ["java","-jar","app.jar"]
