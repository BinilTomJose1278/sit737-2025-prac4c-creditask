# SIT737-2025-Prac5P – Dockerized Calculator Microservice

## Overview

This project is a Dockerized calculator microservice built using **Node.js**, **Express.js**, and **Winston** logging. It performs basic arithmetic operations like addition, subtraction, multiplication, division, power, modulo, and square root through RESTful API endpoints.

---

##  Features

- REST API for basic arithmetic operations
- Logging of incoming requests and outgoing responses using Winston
- Dockerized using a custom Dockerfile
- Health checks using Docker Compose
- Automatic container restart on failure
- Logs persisted using volume binding

---

##  Technologies Used

- Node.js
- Express.js
- Winston Logger
- Docker
- Docker Compose

---

##  How to Run the App

### Step 1: Clone the Repository

```bash
git clone  https://github.com/BinilTomJose1278/sit737-2025-prac5p.git
cd sit737-2025-prac5p

```

Step 2: Ensure Docker Is Installed
Make sure Docker is installed on your system. You can download Docker Desktop from:

https://www.docker.com/products/docker-desktop

----
### Verify Docker Installation
```bash
docker --version
```

Step 3: Build and Run the Application Using Docker Compose
```bash
docker-compose up --build
```
This command will:

Build a Docker image using the Dockerfile

Start a container running your calculator app

Expose it on http://localhost:3000

Apply a health check to monitor availability

Mount the local logs/ folder to persist logs

---

Step 4: Test the Calculator API

You can test the microservice using a browser or Postman.

Available endpoints:

Route	Description	Example
/add	Addition	/add?num1=10&num2=5
/subtract	Subtraction	/subtract?num1=10&num2=5
/multiply	Multiplication	/multiply?num1=10&num2=5
/divide	Division	/divide?num1=10&num2=2
/power	Exponentiation	/power?num1=2&num2=3
/modulo	Modulo	/modulo?num1=10&num2=3
/sqrt	Square root (only num1)	/sqrt?num1=25



