# Getting Started

### Libraries & Tech
* Gradle 5.6
* Spring Boot 2.1.8
* Spring Cloud Gateway

### Gradle command
#### Clean
```shell script
./gradlew clean
```
#### Build
```shell script
./gradlew build
```
### Run Go service
```shell script
./binary/hello-go-mac-os
```
### Run cloud-gateway-demo
```shell script
host$ java -jar build/libs/cloud-gateway-demo-0.0.1-SNAPSHOT.jar --spring.config.location=file:src/main/resources/application.yml
```
or
```shell script
java -Dspring.config.location=file:src/main/resources/application.yml -jar build/libs/cloud-gateway-demo-0.0.1-SNAPSHOT.jar
```
### Actuator
#### Refresh yaml
```shell script
host$ curl -X POST http://localhost:9595/actuator/refresh
```