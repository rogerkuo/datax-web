FROM openjdk:8-jre-alpine

LABEL maintainer="rogerkuo"

VOLUME /tmp
ARG JAR_FILE
RUN echo $JAR_FILE
ADD $JAR_FILE app.jar
RUN sh -c 'touch /app.jar'
EXPOSE 9999
ENV SPRING_PROFILES_ACTIVE=k8s-dev
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/app.jar"]
