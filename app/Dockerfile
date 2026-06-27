FROM eclipse-temurin:21-jre

WORKDIR /app

RUN apt-get update && apt-get install -y unixodbc && rm -rf /var/lib/apt/lists/*

COPY my-app.jar app.jar

EXPOSE 8277

ENTRYPOINT ["java", "-jar", "app.jar"]
