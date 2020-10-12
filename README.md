# spring-oauth2-demo

An oauth2 show case based on spring cloud(zuul,eureka,oauth2), using JWT(JSON Web Token). 

Webapp is an API gateway and oauth2 client which represents all the internal web services. 

Auth-server is an authentication and authorization server protected by spring security modules.

Resource centre is a resource server protected by oauth2. 


mvn spring-boot:run

http://localhost:8080/resource/
