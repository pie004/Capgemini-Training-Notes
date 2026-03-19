# 📘 TYPE CASTING

**Type Casting:**
The process of **converting one datatype into another datatype**.

👉 It can be:

* Primitive → Primitive
* Non-Primitive → Non-Primitive

---

## Types of Type Casting

### 1) Auto Widening (Implicit Casting) ↑

* Done **automatically by the compiler**
* No data loss
* Smaller datatype → Larger datatype

👉 Compiler internally adds type conversion.

### Order of Widening:
byte → short → int → long → float → double
        ↑
       char
---

### 2) Narrowing (Explicit Casting) ↓

* Done **manually by programmer**
* May cause **data loss**
* Larger datatype → Smaller datatype

---

## Example of Narrowing

```java
short s = 128;
byte b = s;   // ❌ Compile-time error
```

### To Resolve:

```java
byte b = (byte) s;   // ✔ Explicit casting
System.out.println(b);  // Output: -128
```

---

## Important Concept (VERY IMPORTANT ⚠️)

* `byte` range = **-128 to 127**
* When value exceeds range → it **loops (overflow)**

👉 That’s why:

```
128 → -128
129 → -127
130 → -126
135 → -121
```

✔ It behaves like a **circular loop**

---

# 📘 SYNTAX

## Widening Syntax (Implicit)

```java
higherRangeDatatype variableName = lowerRangeValue;
```

### Example:

```java
int a = 10;
double d = a;   // automatic conversion
```

---

## Narrowing Syntax (Explicit)

```java
lowerRangeDatatype variableName = (lowerRangeDatatype) higherRangeValue;
```

### Example:

```java
double d = 10.5;
int a = (int) d;   // explicit conversion → 10
```

---

# 📘 EXTRA NOTES

* Compiler **automatically handles widening**
* Programmer must **explicitly handle narrowing**
* Narrowing can cause:

  * Data loss
  * Overflow
  * Unexpected results
