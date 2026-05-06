FROM eclipse-temurin:21-jdk

WORKDIR /app

COPY demo/ /app/demo

WORKDIR /app/demo

RUN ./mvnw clean package -DskipTests || mvn clean package -DskipTests

EXPOSE 8080

CMD ["java","-jar","target/demo-0.0.1-SNAPSHOT.jar"]