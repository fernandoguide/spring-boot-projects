# Spring Boot and Testcontainers Example

Related Articles
* [Spring Boot Testcontainers example](https://mkyong.com/spring-boot/spring-boot-testcontainers-example/)

## Technologies:
* Spring Boot 3.1.2 (Spring Web MVC, Spring Data JPA and Spring Test)
* Testcontainers 1.19.0
* PostgreSQL 15, Alpine Linux base image `postgres:15-alpine`
* Java 17
* JUnt 5

## How to start
```
$ git clone https://github.com/mkyong/spring-boot.git

$ cd spring-boot-testcontainers

$ ./mvnw test

$ ./mvnw spring-boot:run
```

### Building and running your application

When you're ready, start your application by running:
`docker compose up --build`.

Your application will be available at http://localhost:8080.

### Deploying your application to the cloud

First, build your image, e.g.: `docker build -t myapp .`.
If your cloud uses a different CPU architecture than your development
machine (e.g., you are on a Mac M1 and your cloud provider is amd64),
you'll want to build the image for that platform, e.g.:
`docker build --platform=linux/amd64 -t myapp .`.

Then, push it to your registry, e.g. `docker push myregistry.com/myapp`.

Consult Docker's [getting started](https://docs.docker.com/go/get-started-sharing/)
docs for more detail on building and pushing.