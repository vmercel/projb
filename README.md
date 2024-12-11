# AI-Driven Diet Monitoring and Suggestion System

## Project Overview

This project is a **Spring Boot-based AI-enabled system** for monitoring patient dietary habits and providing personalized diet recommendations. It consists of two parts:
1. **Monitoring Service**: Collects and stores food logs and vitals data from patients.
2. **Recommendation Service**: Processes the data to generate AI-based diet recommendations and allows dietitians to review them.

The system is built with modern design principles, follows a microservices architecture, and exposes REST APIs for interaction. There is no GUI, making it suitable for integration with external systems.

---

## Features

1. **User Management**:
   - Manage users with roles (`PATIENT` and `DIETITIAN`).

2. **Food Logging**:
   - Record meals with details like calorie intake and nutrients.
   - Retrieve food logs based on user and date.

3. **Vitals Monitoring**:
   - Record vitals such as heart rate, calories burned, and steps.
   - Analyze trends over time.

4. **Diet Recommendations**:
   - Generate personalized diet plans based on food logs and vitals.
   - Review and approve/reject recommendations.

5. **Analysis Service**:
   - Perform statistical analysis on patient data.

6. **Notification Service** (optional):
   - Notify patients when recommendations are generated or reviewed.

7. **REST API**:
   - Expose endpoints for food logging, vitals monitoring, and recommendations.

---

## Technology Stack

### Backend
- **Framework**: Spring Boot (Web, Data-JPA, Security, Profiles)
- **Database**: MySQL
- **AI Integration**: TensorFlow (or PyTorch) for diet recommendation models
- **Messaging**: Apache Kafka (optional for real-time notifications)

### Deployment
- **Cloud**: Deployed on AWS/Heroku/Azure
- **Containerization**: Docker (optional)

---

## System Architecture

### Entities and Relationships
- **User**: Manages patient and dietitian details.
- **FoodLog**: Tracks meal details like calories and nutrients.
- **Vitals**: Records patient vitals like heart rate and steps.
- **DietRecommendation**: Stores AI-generated diet plans.
- **DietitianReview**: Captures feedback and approval from dietitians.

### Architecture
- **Microservices**:
  - Monitoring Service: Manages food logs and vitals.
  - Recommendation Service: Processes data and generates recommendations.
- **Hexagonal Design**:
  - Core business logic encapsulated in domain models.
  - Separate adapters for APIs and databases.
- **Event-Driven Communication** (optional):
  - Kafka streams for real-time updates.

---

## Installation and Setup

### Prerequisites
- Java 17 or later
- Maven
- MySQL
- Docker (optional for containerized deployment)

### Steps to Run

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/diet-monitoring-system.git
   cd diet-monitoring-system
   
   
   test sentence
   
