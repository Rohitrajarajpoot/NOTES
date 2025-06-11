difrent tools used for diffrent languge



| **Language/Framework** | **Build Tool/Command**            | **Test Command**       | **Docker Base Image**                 | **Common CI/CD Notes**                                  |
| ---------------------- | --------------------------------- | ---------------------- | ------------------------------------- | ------------------------------------------------------- |
| **Node.js**            | `npm install`                     | `npm test`             | `node:18-alpine`                      | Fast builds, good for microservices, lightweight image  |
| **Java (Spring Boot)** | `mvn clean install` (Maven)       | `mvn test`             | `openjdk:17-jdk-slim`                 | Build takes time, JAR/WAR artifact produced             |
| **.NET Core**          | `dotnet build`                    | `dotnet test`          | `mcr.microsoft.com/dotnet/aspnet:7.0` | Needs SDK for build, runtime image for deploy           |
| **Python**             | `pip install -r requirements.txt` | `pytest` or `unittest` | `python:3.10-slim`                    | Needs virtualenv sometimes, good for scripting/services |
