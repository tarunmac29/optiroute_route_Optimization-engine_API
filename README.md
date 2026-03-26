# 🚀 Transport Route Optimizer API

A **Spring Boot-based REST API** that computes the most optimal route between stations using **Dijkstra’s Algorithm** with support for multiple optimization strategies like **distance, time, fare, and multi-criteria**.

---

## 📌 Project Overview

This project simulates a real-world **transport navigation system** where users can find the best route between two locations based on different factors.

It demonstrates strong understanding of:

* Data Structures & Algorithms (Graph + Dijkstra)
* Backend Architecture
* Clean Code & Design Patterns

---

## ✨ Features

✅ Find optimal routes between stations
✅ Multiple optimization strategies:

* 🚗 Shortest Distance
* ⏱️ Fastest Time
* 💰 Lowest Fare
* ⚖️ Multi-criteria (balanced)

✅ Handles edge cases:

* Unreachable destinations
* Invalid inputs

✅ High performance:

* No DB calls inside loops
* Fast response time (<500ms)

---

## 🧠 Tech Stack

* **Java 17**
* **Spring Boot**
* **Spring Data JPA**
* **MySQL**
* **Swagger (OpenAPI)**
* **Postman (API Testing)**

---

## 🏗️ Architecture

Clean layered architecture:

Controller → Service → Repository → Database

Design Patterns Used:

* **Strategy Pattern** (for optimization types)
* **Separation of Concerns**

---

## 📊 Algorithm Used

### 🔹 Dijkstra’s Algorithm

Used for finding the shortest/optimal path in a weighted graph.

* Nodes → Stations
* Edges → Routes
* Weights → Distance / Time / Fare

---

## 🔗 API Endpoints

### 📍 Stations

* `POST /stations` → Create station
* `GET /stations` → Get all stations

### 🛣️ Routes

* `POST /routes` → Create route
* `GET /routes` → Get all routes

### ⚡ Optimization

* `GET /routes/optimize?from=1&to=5&type=distance`
* `GET /routes/optimize?from=1&to=5&type=time`
* `GET /routes/optimize?from=1&to=5&type=fare`
* `GET /routes/optimize?from=1&to=5&type=multi`

---

## 📘 API Documentation (Swagger)

Access Swagger UI:

http://localhost:8082/swagger-ui.html

👉 Interactive API testing directly from browser

---

## 🧪 Testing

* Postman Collection created
* Includes:

  * Functional tests
  * Edge cases
  * Stress testing

---

## 📂 Project Structure

```
optimizer/
 ├── controller/
 ├── service/
 ├── repository/
 ├── entity/
 ├── dto/
 ├── config/
 ├── pom.xml
 └── README.md
```

---

## 🚀 How to Run

### 1. Clone Repository

```
git clone https://github.com/tarunmac29/transport-route-optimizer-api.git
```

### 2. Configure Database

Update `application.properties`:

```
spring.datasource.url=jdbc:mysql://localhost:3306/transport_db
spring.datasource.username=root
spring.datasource.password=your_password
```

### 3. Run Application

```
mvn spring-boot:run
```

---

## 📈 Future Enhancements

* 🌐 Frontend using React + Cytoscape.js
* 📍 Graph visualization of routes
* 🎯 Path highlighting
* 📡 Real-time traffic integration
* 📱 Mobile app integration

---

## 💡 Key Learnings

* Applying DSA in real-world backend systems
* Designing scalable APIs
* Writing clean and maintainable code
* Performance optimization techniques

---

## 🤝 Connect With Me

If you found this project interesting or want to collaborate, feel free to connect!

---

⭐ If you like this project, give it a star on GitHub!
