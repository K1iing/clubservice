# Etapa de construção
FROM maven:3.8-openjdk-17 AS build

WORKDIR /app
COPY ./pom.xml ./
RUN mvn dependency:go-offline

COPY ./src ./src
RUN mvn clean package -DskipTests -Dmaven.test.skip=true  # Ignora testes totalmente

# Etapa de execução
FROM openjdk:17-jdk-slim

COPY --from=build /app/target/*.jar /app.jar

EXPOSE 8080

ENTRYPOINT ["java", "-jar", "/app.jar"]
