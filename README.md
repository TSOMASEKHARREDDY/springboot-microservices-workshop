# Microservices-workshop
This repository contains working sets of spring cloud samples with spring cloud dependencies of Dalston version

### Projects :

* Eureka-Server : Eureka service registration server 
* Eureka-Client-App1 : Eureka service discovery client registered with eureka-server
* Eureka-Client-App2 : Eureka service discovery client registered with eureka-server
* Eureka-Zuul-Proxy : Zuul reverse proxy server acting as reverse proxy pass to other microservices
* Eureka-Config-Server : Configuration server acting as a hub for centralized configuration.




### Spring Boot Version : 1.5.1.RELEASE

```
<parent>
		<groupId>org.springframework.boot</groupId>
		<artifactId>spring-boot-starter-parent</artifactId>
		<version>1.5.1.RELEASE</version>
		<relativePath/> <!-- lookup parent from repository -->
	</parent>
  
  ```

### How to run the project ? 

Download all the projects. 

* <b>Eureka Server </b> : start the eureka server at port 8080
* <b> Eureka Client App1 </b> : start the eureka client app1 listening at port 8081
* <b> Eureka Client App2 </b> : start the eureka client app2 listening at port 8082

test the clients registration by going to eureka :
 
 http://localhost:8080/ 
 
  <b>Test the clients </b> : 
 
 <b>Client 1</b>: http://localhost:8081/ 
 
 <b>Client 2</b>: http://localhost:8082/ 
 
  <b>Test the clients through Zuul proxy </b>: 
 
 Client 1: http://localhost:8085/app1/ --> routed to --> http://localhost:8081/
 
 Client 2: http://localhost:8085/app2/ --> routed to -->  http://localhost:8082/ 
 
 
