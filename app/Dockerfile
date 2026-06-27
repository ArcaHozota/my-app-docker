FROM eclipse-temurin:21-jre

WORKDIR /app

RUN apt-get update && apt-get install -y unixodbc libaio1t64 && rm -rf /var/lib/apt/lists/* \
    && ln -sf /usr/lib/aarch64-linux-gnu/libaio.so.1t64 /usr/lib/aarch64-linux-gnu/libaio.so.1

COPY my-app.jar app.jar

EXPOSE 8277

ENTRYPOINT ["java", "-jar", "app.jar"]
