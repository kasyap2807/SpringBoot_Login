# SpringBoot_SECURITY

Spring Boot Login and Signup using Authentication and Spring Security

## Used Maven Repos

1. Spring Security
2. Spring WEB
3. Spring JPA
4. Spring DevTools
5. MySQL Drivers
6. JJWT : IMPL
7. JJWT : API
8. JJWT : JACKSON


## HOW TO RUN????...

Step - 1 -> Download Code in ZIP form <br/> <br/>
Step - 2 -> Extract Zip Code <br/> <br/>
Step - 3 -> Open It in intelliJ IDEA Community Edition <br/> <br/>
Step - 4 -> Refresh the Maven <br/> <br/>
Step - 5 -> Update The Mysql User, Password and DataBase <br/> <br/>
Step - 6 -> Run The Spring Boot <br/> <br/>
Step - 7 -> Server Will Run in Localhost:8080 Port <br/> <br/>
Step - 8 -> Test It in PostMan 

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

 http://localhost:8080/students - GET - with Bearer Token in Authorization <br/>
 (Eg. eyJhbGciOiJIUzI1NiJ9.eyJzdWIiOiJLcmlzaG5hIiwiaWF0IjoxNzMyNTI0NTc1LCJleHAiOjE3MzI1MjQ2ODN9.MVwsFv9LKDRzrfVmANrNuT6irCs559sjZGB9iTnee4E)

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
