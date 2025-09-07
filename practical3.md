# Practical 3: Microservices Architecture with gRPC & Service Discovery

This practical implements a complete microservices architecture using gRPC, Consul service discovery, PostgreSQL databases, and Docker containerization.

---

## Implementation Screenshots

### 1. Docker Services - All Running
![Service Terminal Logs](img/4.png)

### 2. Consul Service Discovery
![Consul UI - Registered Services](img/7.png)

### 3. API Testing - CRUD Operations
![API Gateway Testing](img/3.png)

### 4. Service Logs - gRPC Communication
![Service Terminal Logs](img/4.png)

---

## Architecture Overview

- **API Gateway** (Port 8081) - HTTP to gRPC routing
- **Users Service** (Port 50051) - User management + PostgreSQL
- **Products Service** (Port 50052) - Product catalog + PostgreSQL  
- **Consul** (Port 8500) - Service discovery & health monitoring

### API Endpoints:
- `POST/GET /api/users` - User operations

    ![](img/8.png)

- `POST/GET /api/products` - Product operations

    ![](img/9.png)

- `GET /api/purchase-data` - Cross-service communication

    ![](img/10.png)

---

## Key Features

**gRPC Communication** - High-performance inter-service calls  
**Service Discovery** - Automatic registration with Consul  
**Database Per Service** - Microservices isolation pattern  
**Docker Containerization** - Complete containerized deployment  
**Health Monitoring** - Real-time service health checks  

---

## Technologies Used

- **Go 1.24.6** - Backend services
- **gRPC & Protocol Buffers** - Service communication
- **GORM + PostgreSQL** - Database layer
- **Consul** - Service discovery
- **Docker Compose** - Container orchestration

---

## 🔗 Source Code Repository

**Complete implementation:** [**Microservices Project**](https://github.com/Namgay282004/practical3-grpc)