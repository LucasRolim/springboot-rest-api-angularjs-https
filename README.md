## REST HTTPS API with Spring Boot and Angular JS.

[![Build Status](https://travis-ci.org/ORolim/springboot-rest-api-angularjs-https.svg?branch=master)](https://travis-ci.org/ORolim/springboot-rest-api-angularjs-https)
[![Coverage Status](https://coveralls.io/repos/github/ORolim/springboot-rest-api-angularjs-https/badge.svg?branch=master)](https://coveralls.io/github/ORolim/springboot-rest-api-angularjs-https?branch=master)
[![codebeat badge](https://codebeat.co/badges/8192c7a4-8747-4177-b4f3-9f35faea2e84)](https://codebeat.co/projects/github-com-orolim-springboot-rest-api-angularjs-https-master)

### Technology stack:

* Maven;
* FindBugs;
* Travis CI;
* Tomcat embedded;
* Spring Boot;
* JUnit;
* Mockito;
* Logback (as SLF4J facade);
* Spring Web;
* Spring Data JPA;
* Hibernate (as JPA implementation);
* MySQL Relation Database;
* Spring Security (as basic authentication);
* Angular JS, HTML, CSS.

### To run this application use:

```bash
mvn spring-boot:run
  ```

### This is what my REST API does:

Go to `https://localhost:8443` to test and must specify a username: `root` and password: `12345`

* POST request to `/api/v1/objects/` with a "object" object as JSON creates a new "object";
* GET request to `/api/v1/objects/` returns a list of "objects";
* GET request to `/api/v1/objects/1` returns the "object" with ID 1;
* PUT request to `/api/v1/objects/3` with a "object" object as JSON updates the "object" with ID 3;
* DELETE request to `/api/v1/objects/4` deletes the "object" with ID 4;
* DELETE request to `/api/v1/objects/` deletes all the "objects".

### The view in the Postman:

[https://localhost:8443/api/v1/objects](https://localhost:8443/api/v1/objects) 

Message body: `{"title":"Absorber", "value":"123123"}`

![alt tag](http://i.piccy.info/i9/805925eb5dd73435f3b1d9d94bafbb39/1479759393/66174/1085055/rest11.jpg)

_**Open browser and browse at: 
[https://localhost:8443](https://localhost:8443)**_

![alt tag](http://i.piccy.info/i9/7656c6d92ad0b4f722500bb6ebbf944e/1479758651/77123/1085055/resthttps.jpg)

_**To run the SonarQube use:**_

```bash
mvn clean install sonar:sonar
```