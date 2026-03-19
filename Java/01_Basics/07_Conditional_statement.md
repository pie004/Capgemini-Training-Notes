# **Conditional Statements (decision making statements)**

* if
* if-else
* nested if
* if-else-if
* else-if ladder

✔ used when **more than one condition**

---

# **Switch Statement**

* switch - doesn't take condition (constant value condition)
* switch (data / variable / expression)
* only 3 type supports → **int, char, String**

---

# **Advantage**

* multiple cases can be executed at a single time (**fall-through if break not used**)

```java
switch(expression)
{
    case v1:   // statements
               break;

    case v2:   // statements
               break;

    case vn:   // statements
               break;

    default:   // statements  // optional
               break;
}
```

---

# **(Control transfer statement)**

→ **break**

* once hits break, it transfer the control to outside of the block
* used in loop + switch

→ **continue**

* skips current iteration and moves to next iteration (only in loop)

---

# **CTE (unreachable statement)**

→ If we write any statement after break and before starting a new case 
→ it becomes unreachable statement (compile-time error)

---

# **Loop**

✔ for
✔ while
✔ do while
✔ for each loop

→ **used for repetition of statements**

---

# **1) while → while(condition)**

(entry control loop)

```java
vd & vi
while(condition)
{
    // statements
    // updation
}
```

* 0 iteration it takes to execute the first iteration
* first checks condition then enters loop
* executes till condition becomes false

---

# **2) do while →**

(exit control loop)

```java
vd & vi
do
{
    // statements
    // updation
}
while(condition);
```

* 1 iteration will be executed first
* condition checked after execution

---

# **VD & VI (Variable Declaration & Initialization)**
* VD → int i;
* VI → int i = 0;

---

# **3) for**

```java
for(VD & VI; condition; updation)
{
    // statements
}
```

* nothing is mandatory except semicolon ( ; )
* initialization can be skipped
* condition can be skipped (infinite loop)
* updation can be skipped

---

# **extra loop notes (added)**

* infinite loop → `for(;;)` or `while(true)`
* nested loop → loop inside another loop
* break → terminate loop
* continue → skip iteration

---

# Use → for and while loop:
→ **for** → when number of iterations known
→ **while** → when condition based

---

