FROM maven:ibmjava-alpine AS builder
WORKDIR /spring-app
COPY . .
RUN mvn clean package


FROM eclipse-temurin:11-jre-alpine
WORKDIR /spring-app
COPY --from=builder /spring-app/target/hello-0.0.1-SNAPSHOT.jar .
EXPOSE 8080
ENTRYPOINT ["java", "-jar"]
CMD ["hello-0.0.1-SNAPSHOT.jar"]
