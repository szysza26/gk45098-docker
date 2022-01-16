FROM openjdk:11

WORKDIR /app

RUN apt-get update && apt-get install -y maven
RUN mvn package

ENTRYPOINT ["java","-jar","target/gk45098-backend-0.0.1-SNAPSHOT.jar"]
