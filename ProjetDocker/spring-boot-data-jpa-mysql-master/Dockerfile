FROM maven AS build

WORKDIR /app/myapp

COPY . .

RUN mvn clean package -DskipTests

FROM openjdk:19-alpine

WORKDIR /app

EXPOSE 8080

COPY --from=build /app/myapp/target/spring-boot-data-jpa*.jar app.jar

ENTRYPOINT ["java","-jar","app.jar"]