FROM openjdk:8u121
MAINTAINER GhostBusters
WORKDIR /app
RUN mvn clean package
COPY ./target/orderservice-0.0.1-SNAPSHOT.jar /app/
ENTRYPOINT ["java", "-Djava.security.egd=file:/dev/./urandom", "-jar", "orderservice-0.0.1-SNAPSHOT.jar"]
EXPOSE 8083
