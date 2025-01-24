# Build stage
FROM maven:3.8-openjdk-17 AS builder
WORKDIR /app
COPY src /app
RUN mvn clean package

# Run stage
FROM eclipse-temurin:17-jre-alpine
WORKDIR /app
COPY --from=builder /app/target/backend-0.0.1-SNAPSHOT.jar app.jar
EXPOSE 8080
ENTRYPOINT ["java", "-jar", "/app.jar"]

