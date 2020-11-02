# spring-microservice-oauth2-keycloak-starter

For detailed tutorial, please refer to the post.  
https://kunkkali.blogspot.com/2020/10/build-j2ee-micro-services-architecture.html

## docker-compose.yml
Replace host ip inside with your own, then run the following cmd to start:

`docker-compose up --build`

Navigate to the following url, then Login keycloak with dev/123

`localhost:8080/api/consume/`

## Fetch access token and refresh token from keycloak server
Post a request to get an access token:

`POST http://localhost:18080/auth/realms/spring-micro-main/protocol/openid-connect/token`  
 `Content-Type: application/x-www-form-urlencoded`
 
 `&client_id=spring-micro-gateway&username=dev&password=123&grant_type=password&client_secret=756b0558-018b-4809-b478-bd5b4995d325`

## Test API
Get request with bearer token:

`GET localhost:8080/api/produce/`  
 `Authorization: Bearer <your bearer token here>`
