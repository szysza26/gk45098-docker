FROM openjdk:11

RUN apt-get update && apt-get install -y maven
COPY ./gk45098-backend /app
RUN cd /app && mvn -Dmaven.test.skip package

ENTRYPOINT ["java","-jar","/app/target/gk45098-backend-0.0.1-SNAPSHOT.jar"]
