FROM maven:3.9.16-eclipse-temurin-17-alpine
WORKDIR /app
COPY . .
RUN mvn package
EXPOSE 8080
CMD ["java","-jar","demo-0.0.1-SNAPSHOT.jar"]