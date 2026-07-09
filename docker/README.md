# Docker

This directory contains hands-on labs related to Docker containerization and container management during the iVolve Internship.

## Labs

### Lab 3

Run Java Spring Boot Application in a Container using Maven image.

- Build the application inside the Docker container.
- Create Docker image.
- Run and test the application.

[Lab 3 - Build Inside Container](lab3-build-inside-container/)

---

### Lab 4

Run Java Spring Boot Application in a Container using Java Runtime image.

- Build the application using Maven on the host machine.
- Create lightweight Docker image using Java 17 runtime.
- Run and test the application.

[Lab 4 - Build Outside Container](lab4-build-outside-container/)

---

### Lab 5

Run Java Spring Boot Application using Multi-Stage Docker Build.

- Build the application in a dedicated builder stage.
- Copy only the generated JAR into the runtime image.
- Create a smaller production-ready image.
- Run and test the application.

[Lab 5 - Multi-Stage Build](lab5-multi-stage-build/)

---

### Lab 6

Managing Docker Environment Variables Across Build and Runtime.

- Pass environment variables using the command line.
- Load environment variables from an external file.
- Define default environment variables inside the Docker image.
- Verify the application behavior in each scenario.

[Lab 6 - Environment Variables](lab6-environment-variables/)

---

### Lab 7

Docker Volume and Bind Mount with Nginx.

- Create and use a Docker volume to persist Nginx logs.
- Use a bind mount to serve static content from the host machine.
- Verify content updates without rebuilding the container.
- Verify persisted logs.

[Lab 7 - Volumes and Bind Mounts](lab7-volumes-and-bind-mounts/)