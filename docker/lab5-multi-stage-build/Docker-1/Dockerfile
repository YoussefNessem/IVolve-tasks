FROM maven:3.9.16-eclipse-temurin-17-alpine AS build
WORKDIR /app
COPY . .
RUN mvn package

FROM amazoncorretto:17-alpine3.21
WORKDIR /app
COPY --from=build /app/target/demo-0.0.1-SNAPSHOT.jar app.jar
CMD ["java", "-jar", "app.jar"]
EXPOSE 8080