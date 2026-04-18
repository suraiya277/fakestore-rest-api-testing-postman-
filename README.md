# 🧪 REST API Testing Project - Fake Store

## 📌 Project Overview

This project demonstrates end-to-end REST API testing using Postman on the Fake Store API.
The focus is on validating API functionality, response structure, performance, and basic data integrity for the Product module.

---

## 🎯 Objectives

* Validate CRUD operations of Product API
* Ensure correct API response and status codes
* Verify response structure and required fields
* Perform basic negative testing
* Measure API response performance

---

## 🛠️ Tools & Technologies

* **Postman** – API testing
* **REST API** – API architecture
* **JSON** – Data format
* **GitHub** – Project hosting

---

## 🌐 API Details

* **Base URL:** https://fakestoreapi.com
* **API Type:** REST

---

## 📦 Tested Module: Product

### 🔹 Endpoints Covered

| Method | Endpoint         | Description        |
| ------ | ---------------- | ------------------ |
| GET    | `/products`      | Get all products   |
| GET    | `/products/{id}` | Get single product |
| POST   | `/products`      | Create product     |
| PUT    | `/products/{id}` | Full update        |
| PATCH  | `/products/{id}` | Partial update     |
| DELETE | `/products/{id}` | Delete product     |

---

## ✅ Test Coverage

* ✔ Status code validation
* ✔ Response time validation
* ✔ JSON structure validation
* ✔ Field verification (id, title, price, category)
* ✔ CRUD operation testing
* ✔ Basic negative testing

---

## 🧪 Sample Test Validations

* Verify status code is **200 / 201**
* Validate response time is under acceptable limit
* Check response type (array/object)
* Ensure required fields exist
* Validate generated ID for new resources

---

## 📁 Project Structure

```
rest-api-testing-fakestore
 ┣ 📁 postman
 ┃ ┗ FakeStore.postman_collection.json
 ┃ ┗ FakeStore.environment.json
 ┣ 📁 test-cases
 ┃ ┗ testcases.md
 ┗ README.md
```

---

## ▶️ How to Run the Project

1. Open Postman
2. Import the collection file from `/postman` folder
3. Run individual requests or use Collection Runner
4. View test results in Postman console

---

## ⚠️ Important Note

This project uses a mock API.

* Data is not permanently stored
* POST, PUT, PATCH, DELETE responses are simulated
* Validation is based on response only

---

## 🚀 Key Learning Outcomes

* Hands-on experience with REST API testing
* Understanding of HTTP methods (GET, POST, PUT, PATCH, DELETE)
* Writing test scripts using Postman
* Validating API responses and performance
* Basic understanding of real-world API behavior

---

## 👩‍💻 Author

**Umme Suraiya Kawsary Aktar**

SQA Engineer (Entry-Level)

---
