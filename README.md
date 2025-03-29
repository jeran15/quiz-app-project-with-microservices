# Quiz App Microservices  

## 📌 Overview  
A scalable quiz application built with **Spring Boot Microservices**, **Eureka Service Discovery**, and **API Gateway**.  

## 🛠 Tech Stack  
- **Backend**: Spring Boot, Spring Cloud  
- **Service Discovery**: Netflix Eureka  
- **API Gateway**: Spring Cloud Gateway  
- **Database**: PostgreSQL + Hibernate  
- **Communication**: REST APIs  

## 🚀 Features  
✔️ Dynamic quiz generation  
✔️ Centralized routing via API Gateway  
✔️ Fault-tolerant service registration  

## 🏗 Project Structure  
- `question-service`: Manages quiz questions  
- `quiz-service`: Generates quizzes  
- `api-gateway`: Routes requests  
- `service-registry`: Eureka server  

## 🔧 Setup  
1. Start Eureka Server (`service-registry`)  
2. Run services (`question-service`, `quiz-service`)  
3. Access via API Gateway (`http://localhost:8765`)  

quiz-app-project/
├── api-gateway/          (API Gateway)
├── question-service/     (Microservice with @EnableEurekaClient)
├── quiz-service/         (Microservice with @EnableEurekaClient)
└── service-registry/     (Eureka Server with @EnableEurekaServer)
