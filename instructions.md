# Spring Boot Empty MVC Template

## About

This is an empty MVC template for quick bootstrapping of projects.

## How to run

You can run the application from the command line with Maven. 
Or you can build a single executable JAR file that contains all the necessary dependencies, classes, and resources, and run that.
Go to the root folder of the application and type:
```
./mvnw spring-boot:run
```
Or you can build the JAR file with 
```
./mvnw clean package
``` 
Then you can run the JAR file:
```
java -jar target/empty-template-0.0.1-SNAPSHOT.jar
```
The application should be up and running within a few seconds.

Go to the web browser and visit `http://localhost:8190/home`

In `/src/main/resources/application.properties` file it is possible to change 
the port number.

## Helper Tools

### HAL REST Browser

Go to the web browser and visit `http://localhost:8190/`

You will need to be authenticated to be able to see this page.

### H2 Database web interface

Go to the web browser and visit `http://localhost:8190/h2-console`

In field **JDBC URL** put 
```
jdbc:h2:mem:empty_template_db
```

In `/src/main/resources/application.properties` file it is possible to change both
web interface url path, as well as the datasource url.
