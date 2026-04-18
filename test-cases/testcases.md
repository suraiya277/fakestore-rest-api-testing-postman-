# 🧪 Fake Store API Testing - Test Cases

## 📌 Module: Product API

**Base URL:** https://fakestoreapi.com

---

## 🎯 Objective

To validate the functionality, performance, and reliability of Product-related REST API endpoints using Postman.

---

## 📋 Test Scope

* Functional Testing
* API Response Validation
* Performance Validation
* Data Integrity Check
* Basic Negative Testing

---

## ✅ TC_01: Get All Products

* **Endpoint:** `GET /products`
* **Method:** GET
* **Description:** Verify that all products are retrieved successfully

**Test Steps:**

1. Send GET request to `/products`

**Expected Results:**

* Status code is **200**
* Response time is **< 1500ms**
* Response body is an **array**
* Array is **not empty**
* Each product object contains:

  * id (number)
  * title (string)

---

## ✅ TC_02: Get Single Product

* **Endpoint:** `GET /products/{id}`
* **Method:** GET
* **Description:** Verify that a single product is retrieved correctly

**Test Steps:**

1. Send GET request to `/products/1`

**Expected Results:**

* Status code is **200**
* Response time is **< 1500ms**
* Response body is an **object**
* Object contains:

  * id
  * title
  * price
  * category

---

## ✅ TC_03: Create New Product(POST)

* **Endpoint:** `POST /products`
* **Method:** POST
* **Description:** Verify that a new product can be created

**Test Steps:**

1. Send POST request with valid JSON body

**Expected Results:**

* Status code is **200 or 201**
* Response time is **< 2000ms**
* Response body is an **object**
* Response contains:

  * id (auto-generated)
  * title (string)

---

## ✅ TC_04: Update Product (PUT)

* **Endpoint:** `PUT /products/{id}`
* **Method:** PUT
* **Description:** Verify full update of product

**Test Steps:**

1. Send PUT request to `/products/2` with updated data

**Expected Results:**

* Status code is **200 or 201**
* Response body is an **object**
* Response contains:

  * id
  * updated fields (based on API behavior)

---

## ✅ TC_05: Partial Update Product (PATCH)

* **Endpoint:** `PATCH /products/{id}`
* **Method:** PATCH
* **Description:** Verify partial update of product

**Test Steps:**

1. Send PATCH request with partial data

**Expected Results:**

* Status code is **200**
* Response body is an **object**
* Response contains:

  * id
* API acknowledges update request

---

## ✅ TC_06: Delete Product

* **Endpoint:** `DELETE /products/{id}`
* **Method:** DELETE
* **Description:** Verify product deletion

**Test Steps:**

1. Send DELETE request to `/products/2`

**Expected Results:**

* Status code is **200**
* Response body is an **object**
* Response contains:

  * id

---

## ❌ TC_07: Retrieve Invalid Product

* **Endpoint:** `GET /products/9999`
* **Method:** GET
* **Description:** Verify behavior with invalid product ID

**Test Steps:**

1. Send GET request with non-existing ID

**Expected Results:**

* Status code is **404** or error response
* Proper error handling is observed

---

## ⚠️ Assumptions & Limitations

* The API is a mock service; data is not persisted.
* POST, PUT, PATCH, and DELETE operations do not permanently modify data.
* Validation is performed based on API response only.

---

## 📊 Test Summary

| Test Type           | Covered |
| ------------------- | ------- |
| Functional Testing  | ✅       |
| CRUD Operations     | ✅       |
| Response Validation | ✅       |
| Performance Check   | ✅       |
| Negative Testing    | ✅       |

---

## 👨‍💻 Conclusion

All core CRUD operations for the Product module were successfully tested.
The API responses were validated for correctness, structure, and performance within expected limits.
