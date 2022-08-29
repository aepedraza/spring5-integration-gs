# Spring 5 Integration: Getting Started

Course by Jesper de Jong (Pluralsight)

## Requirements
1. Docker
2. Java 11
3. Maven 3.x

## How to run from 
1. Crreate and run `RabbitMQ` docker image
```
docker run -d -h rabbitmq --name=rabbitmq -p 5672:5672 -p 15672:15672 rabbitmq:3.7-management-alpine
```
2. Create and run `GreenMail` server
```
docker run -d -h greenmail --name=greenmail -p 3025:3025 -p 3143:3143 greenmail/standalone
```
3. Create JAR executables
```
mvn clean package
```
4. Run applications individually with `java` or `mvn` (spring boot plugin) commands
