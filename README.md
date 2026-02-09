# CST8915 Lab 1: Algonquin Pet Store on Azure VM

**Student Name**: Bosi Chen\
**Student ID**: 041040774\
**Course**: CST8915 Full-stack Cloud-native Development\
**Semester**: Winter 2026

---

## Demo Video

🎥 [Watch Demo Video](https://youtu.be/tNiB14rJcUQ)

---

## Technical Explanations

Purpose: What is this service responsible for?
Technology Stack: Which language/framework does it use and why?
Architecture Role: How does it fit into the microservices architecture?
Inter-Service Communication: How does it interact with other services?

### Order Service (Node.js)

The Order Service manages customer orders and interacts with RabbitMQ for message queuing. 

It is built with Node.js, which is a common JavaScript runtime designed for backend services. 

In the microservices architecture, this service acts as a bridge between the front end and the backend processing. 

It uses REST API for order submission and interacts with RabbitMQ to queue order messages. 

### Product Service (Rust)

Handles product listings. Manages product details and inventory.

It is written in Rust, which is a fast, memory-safe language for creating high-performance APIs.

In the microservice architecture, it provides REST API endpoints that allow other parts of the system to fetch product details and send to the front end. 

### Store Front (Vue.js)

A front-end application where customers can browse and order products.

It is built with Vue.js, a modern JavaScript framework used for creating interactive web applications.

In the microservices architecture, it displays the user interface, shows the product by fetching data from the Product Service and sends completed orders to the Order Service for processing.
