# JavaAssignment4


# 3D Vector Operations System (Java)

## Overview

This project is a **Java-based 3D Vector Operations System** that demonstrates object-oriented programming concepts, custom exception handling, and the use of Java’s built-in `Vector` collection.

The application allows users to create 3D vectors and perform mathematical operations such as **addition, subtraction, and dot product**. It also ensures robustness by handling invalid inputs using a custom exception.

---

## Features

* Create 3D vector objects
* Perform vector addition
* Perform vector subtraction
* Compute dot product of vectors
* Store multiple vectors using Java `Vector` collection
* Handle invalid operations using custom exceptions
* Demonstrate exception handling with null vectors and invalid values

---

## Project Structure

### 1. VectorException Class

A custom exception class that extends `Exception`.

Purpose:

* Handles invalid vector operations
* Ensures data integrity during vector creation and operations

---

### 2. Vector3D Class

Represents a 3D mathematical vector.

#### Data Members

* `x` – x-coordinate
* `y` – y-coordinate
* `z` – z-coordinate

#### Constructors

* **Default Constructor** – initializes vector to (0, 0, 0)
* **Parameterized Constructor** – initializes vector with given values and validates inputs

#### Methods

* `add(Vector3D v)` – returns the sum of two vectors
* `subtract(Vector3D v)` – returns the difference of two vectors
* `dotProduct(Vector3D v)` – returns the dot product
* `display()` – prints the vector in coordinate form

---

### 3. JavaVectorDemo Class

The main class containing the `main` method.

Responsibilities:

* Creates multiple `Vector3D` objects
* Stores them in a Java `Vector` collection
* Performs vector operations using stored elements
* Demonstrates exception handling

---

## Vector Operations

### Addition

Adds corresponding components of two vectors:

```
(x1 + x2, y1 + y2, z1 + z2)
```

### Subtraction

Subtracts corresponding components:

```
(x1 - x2, y1 - y2, z1 - z2)
```

### Dot Product

Calculates scalar product:

```
x1*x2 + y1*y2 + z1*z2
```

---

## Exception Handling

The program throws a custom `VectorException` in the following cases:

* If any vector component is `NaN`
* If a null vector is used in operations
* If invalid vector operations are attempted

---

## How to Run the Program

### Prerequisites

* Java Development Kit (JDK) installed
* Terminal or command prompt

### Steps

1. Compile the program:

```
javac JavaVectorDemo.java
```

2. Run the program:

```
java JavaVectorDemo
```

---

## Sample Output

```
Stored 3D Vectors:
(2.0, 3.0, 4.0)
(1.0, 5.0, 2.0)
(7.0, 1.0, 6.0)

Operations on Vectors:
Addition: (3.0, 8.0, 6.0)
Subtraction: (1.0, -2.0, 2.0)
Dot Product: 25.0

Vector Exception: Null vector cannot be added
```

---

## Concepts Used

* Object-Oriented Programming (OOP)
* Classes and Objects
* Encapsulation
* Constructors
* Exception Handling (try-catch)
* Custom Exceptions
* Java Collections (`Vector`)
* Mathematical vector operations

---


