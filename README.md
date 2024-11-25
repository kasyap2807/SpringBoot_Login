# SpringBoot_SECURITY

Spring Boot Login and Signup using Authentication and Spring Security

## Used Maven Repos

### Spring Security
### Spring WEB
### Spring JPA
### Spring DevTools
### MySQL Drivers
### JJWT : IMPL
### JJWT : API
### JJWT : JACKSON


## HOW TO RUN????...

Step - 1 -> Download Code in ZIP form
Step - 2 -> Extract Zip Code
Step - 3 -> Open It in intelliJ IDEA Community Edition
Step - 4 -> Refresh the Maven
Step - 5 -> Update The Mysql User, Password and DataBase
Step - 6 -> Run The Spring Boot 
Step - 7 -> Server Will Run in Localhost:8080 Port
Step - 8 -> Test It in Spring Boot

## API

### Login API 

REQUEST:

 http://localhost:8080/login - POST - BODY
 BODY = {
    "id":1,
    "username":"Krishna",
    "password":"P@123"
}

RESPONSE:

Token ( Eg. eyJhbGciOiJIUzI1NiJ9.eyJzdWIiOiJLcmlzaG5hIiwiaWF0IjoxNzMyNTI0NTc1LCJleHAiOjE3MzI1MjQ2ODN9.MVwsFv9LKDRzrfVmANrNuT6irCs559sjZGB9iTnee4E)

### SignUP API 

REQUEST:

 http://localhost:8080/login - POST - BODY
 BODY = {
    "id":1,
    "username":"Krishna",
    "password":"P@123"
}

RESPONSE:

 {
    "id":1,
    "username":"Krishna",
    "password":"P@123"
}

### get Data API 

REQUEST:

 http://localhost:8080/students - GET - with Bearer Token in Authorization(Eg. eyJhbGciOiJIUzI1NiJ9.eyJzdWIiOiJLcmlzaG5hIiwiaWF0IjoxNzMyNTI0NTc1LCJleHAiOjE3MzI1MjQ2ODN9.MVwsFv9LKDRzrfVmANrNuT6irCs559sjZGB9iTnee4E)

 RESPONSE:

[
  {
    "id":1,
    "name":"Navin",
    "marks":60
  },
  {
    "id":2,
    "name":"Kiran",
    "marks":65
  }
}
