FROM openjdk:21-jdk-slim

WORKDIR /app

COPY target/user-service-*.jar app.jar

EXPOSE 8080

ENV JAVA_TOOL_OPTIONS="-XX:MaxRAMPercentage=75.0"

ENTRYPOINT ["java", "-jar", "app.jar"]