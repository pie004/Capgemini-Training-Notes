# **Datatypes**

Datatypes define the type of value a variable can hold and how a computer system interprets and operates on that data.

They are generally classified into two types:

* **Primitive (basic)**
* **Non-primitive (complex / user-defined)**

---

## **i) Primitive Datatypes**

There are **8 primitive datatypes**:

| Datatype      | Size              | Range                  | Digits (approx)    |
| ------------- | ----------------- | ---------------------- | ------------------ |
| **byte**      | 1 byte (8 bits)   | -128 to +127           | 3 digits           |
| **short**     | 2 bytes (16 bits) | -32768 to +32767       | 5 digits           |
| **int**       | 4 bytes (32 bits) | -2³¹ to 2³¹ - 1        | 10 digits          |
| **long (l)**  | 8 bytes (64 bits) | -2⁶³ to 2⁶³ - 1        | 19 digits          |
| **float (f)** | 4 bytes (32 bits) | ±3.4E−38 to ±3.4E+38   | 7 digits           |
| **double**    | 8 bytes (64 bits) | ±1.7E−308 to ±1.7E+308 | 15–16 digits       |
| **char**      | 2 bytes (16 bits) | 0 to 65535             | 1 character        |
| **boolean**   | JVM dependent     | true / false           | 1 bit (conceptual) |

---

## **ii) Non-Primitive Datatypes**

Non-primitive datatypes **do not store actual values**, they store **memory addresses (references)**.

### Types:

* **String** *(collection of characters)*

  ```java
  String name = "Piyasa";
  ```

* **Array** *(stores multiple values of same type)*

  ```java
  int[] marks = {70, 80, 90};
  ```

* **Class** *(user-defined blueprint)*

  ```java
  class Student {
      int roll;
  }
  ```

* **Object** *(instance of a class)*

  ```java
  Student s = new Student();
  ```

* **Interface** *(used to achieve abstraction)*

  ```java
  interface Printable {
      void print();
  }
  ```

---