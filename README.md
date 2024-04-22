# Simple Calculator Microservice

## Overview

This is a simple calculator RESTful API microservice built using Node.js and Express. It provides basic arithmetic operations such as addition, subtraction, multiplication, and division. It also provides error handling mechanisms for validation.

It uses winston logger for logging in the application.

## Usage

### Base URL

```
http://localhost:3000
```

### Endpoints

---

**1. Health Check**

- `/`
- Method: `GET`
- Description: Checks if the microservice is running. Use this to check if the server is running.
- Response:

  - **Status Code:** 200 OK

    ```json
    {
      "message": "Calculator Microservice Running"
    }
    ```

---

**2. Addition Endpoint**

- **EndPoint**: `/add/:num1/:num2`
- **Method**: `GET`
- **Description**: Performs addition operation on two numbers.
- **Parameters:**
  - `num1` (number): The first operand.
  - `num2` (number): The second operand.
- **Response**:

  - **Status Code:** 200 OK
  - **Body:**

    ```json
    {
      "result": <addition result>
    }
    ```

  - **Status Code:** 400 BAD REQUEST
  - **Body:**

    ```json
    {
      "error": <error description>
    }
    ```

---

**3. Subtraction Endpoint**

- **EndPoint**: `/subtract/:num1/:num2`
- **Method**: `GET`
- **Description**: Performs subtraction operation on two numbers.
- **Parameters:**
  - `num1` (number): The first operand.
  - `num2` (number): The second operand.
- **Response**:

  - **Status Code:** 200 OK
  - **Body:**

    ```json
    {
      "result": <subtraction result>
    }
    ```

  - **Status Code:** 400 BAD REQUEST
  - **Body:**

    ```json
    {
      "error": <error description>
    }
    ```

---

**4. Multiplication Endpoint**

- **EndPoint**: `/multiply/:num1/:num2`
- **Method**: `GET`
- **Description**: Performs multiplication operation on two numbers.
- **Parameters:**
  - `num1` (number): The first operand.
  - `num2` (number): The second operand.
- **Response**:

  - **Status Code:** 200 OK
  - **Body:**

    ```json
    {
      "result": <multiplication result>
    }
    ```

  - **Status Code:** 400 BAD REQUEST
  - **Body:**

    ```json
    {
      "error": <error description>
    }
    ```

---

**5. Division Endpoint**

- **EndPoint**: `/divide/:num1/:num2`
- **Method**: `GET`
- **Description**: Performs division operation on two numbers.
- **Parameters:**
  - `num1` (number): The first operand.
  - `num2` (number): The second operand.
- **Response**:

  - **Status Code:** 200 OK
  - **Body:**

    ```json
    {
      "result": <division result>
    }
    ```

  - **Status Code:** 400 BAD REQUEST
  - **Body:**

    ```json
    {
      "error": <error description>
    }
    ```

# Examples

**Addition:** `http://localhost:3000/add/6/8`

- **Result**: 14

**Subtraction:** `http://localhost:3000/subtract/10/8`

- **Result**: 2

**Multiplication:** `http://localhost:3000/multiply/6/7`

- **Result**: 42

**Division:** `http://localhost:3000/divide/24/8`

- **Result**: 3

---
