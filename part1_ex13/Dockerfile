# FROM openjdk:14-jdk-alpine
FROM openjdk:latest

# RUN apt-get update
# RUN apt-get install -y curl wget
# RUN apt-get install -y git
COPY . /usr/src/myapp

# RUN git clone https://github.com/docker-hy/spring-example-project.git
WORKDIR /usr/src/myapp
RUN chmod u+x ./mvnw
RUN ./mvnw package
EXPOSE 8080

CMD ["/bin/bash"]
ENTRYPOINT java -jar ./target/docker-example-1.1.3.jar