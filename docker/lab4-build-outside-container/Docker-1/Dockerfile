FROM amazoncorretto:17-alpine3.21
WORKDIR /app
COPY target/demo-0.0.1-SNAPSHOT.jar .
EXPOSE 8080
CMD ["java","-jar","app.jar"]