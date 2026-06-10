FROM amazoncorretto:17-jre

WORKDIR /app

COPY my-app.jar app.jar

EXPOSE 8277

ENTRYPOINT ["java", "-jar", "app.jar"]
