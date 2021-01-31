FROM openjdk:11.0-slim
RUN ./mvnw clean install -Dmaven.test.skip=true
ARG JAR_FILE=target/*.jar
COPY ${JAR_FILE} app.jar
ENTRYPOINT ["java","-jar","/app.jar"]
