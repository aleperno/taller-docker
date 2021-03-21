FROM openjdk:11-jre-slim

WORKDIR /app

COPY passwordapi.jar /app/passwordapi.jar

EXPOSE 8080/tcp

CMD ["java", "-jar", "/app/passwordapi.jar"]
