FROM amazoncorretto:8

EXPOSE 8080

WORKDIR /usr/src/app

COPY . .

# Thanks to the comments in Discord I realised I had to add this on Windows for mvnw package to work.
RUN sed -i 's/\r$//' mvnw

RUN ./mvnw package

CMD ["java", "-jar", "./target/docker-example-1.1.3.jar"]