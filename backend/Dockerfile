FROM maven:3.8.3-openjdk-17

WORKDIR /opt

COPY . .

RUN mvn clean package -DskipTests

ENTRYPOINT ["java", "-jar", "target/student-registration-backend-0.0.1-SNAPSHOT.jar"]