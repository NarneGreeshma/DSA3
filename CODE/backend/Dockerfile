FROM maven:3.9-eclipse-temurin-21

WORKDIR /app

COPY pom.xml .
COPY src ./src

RUN mvn clean compile

EXPOSE 8080

CMD ["mvn", "exec:java", "-Dexec.mainClass=com.labmatch.Main"]
