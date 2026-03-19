# 📘 VARIABLES

**Variable:**
A variable is a **memory block used to store data or values**.

---
## Types of Variable Operations
1. Variable Declaration
2. Variable Initialization
---
## 1) Declaration

**Definition:**
Creating a memory block with a name.

Syntax: datatype variableName;
Example: int a;

## 2) Initialization

**Definition:**
Assigning a value to a variable (from right to left).

Syntax: variableName = value;
Example: a = 10;

## Combination of Declaration + Initialization

Syntax: datatype variableName = value;
Example: int a = 10;

## Important Notes

* JVM takes care of everything from **memory creation to storing values**.
* Compiler only checks the **datatype**, not the actual value.

---

# 📘 TYPES OF VARIABLES

## Based on Datatypes

1. **Primitive Variables**
   → Variables declared using primitive datatypes (int, float, char, etc.)

2. **Non-Primitive Variables**
   → Variables declared using reference types (String, Array, Object, etc.)

---

## Based on Scope and Visibility

### 1) Local Variable

* Declared **inside a method/block**(main)
* Accessible **only within that block**

### 2) Global Variable (Instance Variable)

* Declared **inside class but outside methods**
* Accessible throughout the class

---

### Example:

```java
class A {
    int x;   // Global variable

    public static void main(String[] args) {
        int y = 10;  // Local variable
    }
}
```

---

## Important Points

* The `main()` method is inside class `A`, so it is also global.
* variables declared **outside methods are global (instance variables)**.
* Variables can only be declared inside a **class block (not outside the class in Java)**.

---

### Local Variable Rule
for local variable, if value of variable is not initialised, it doesn't return anything, as it doesn't  have any default value.so we can say:
* Must be **initialized before use**
* Otherwise → **compile-time error**
* Reason: Local variables do NOT have default values

---

### Global Variable Rule: 
- it takes garbage(default) value

* JVM provides **default values**
* Example:

  * int → 0
  * float → 0.0
  * boolean → false
  * object → null

---

# 📘 EXTRA NOTES

* **Re-initialization:**
  Changing/updating the value of a variable: a = 20;
* While re-initializing, **datatype is not written again**, only variable name is used.

---

# 📘 QUESTION

### Q) WAP in Java to print Aadhaar details:

Fields: ID, Name, Gender, Address, Number, Email ID

### Answer:

```java
class Aadhaar {
    public static void main(String[] args) {

        int id = 123456;
        String name = "Piyasa";
        String gender = "Female";
        String address = "Kolkata";
        long number = 9876543210L;
        String email = "piyasa@email.com";

        System.out.println("ID: " + id);
        System.out.println("Name: " + name);
        System.out.println("Gender: " + gender);
        System.out.println("Address: " + address);
        System.out.println("Number: " + number);
        System.out.println("Email: " + email);
    }
}
```
