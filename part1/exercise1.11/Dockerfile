FROM amazoncorretto:8-alpine3.17

RUN apk update && apk add git

WORKDIR /app
RUN git clone https://github.com/docker-hy/material-applications.git

RUN cd material-applications/spring-example-project && chmod +x ./mvnw && ./mvnw package

CMD java -jar /app/material-applications/spring-example-project/target/docker-example-1.1.3.jar

