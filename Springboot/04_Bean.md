## What is a Bean?

In the Spring ecosystem, a **Bean** is simply an object that is instantiated, assembled, and managed by the **Spring IoC (Inversion of Control) container**.

Think of a Bean as a "managed object." In standard Java, you create an object using the `new` keyword. In Spring, you let the framework do it for you.

---

### **The "Factory" Analogy**

* **Standard Java:** You are a contractor who has to go to the store, buy the wood, cut it, and build a chair yourself (`Chair c = new Chair()`).
* **Spring Bean:** You are the manager. You tell the factory (Spring Container), "I need a chair with these specific dimensions." The factory builds it, maintains it, and gives it to you whenever you need it. That chair is the **Bean**.

---

### **The Lifecycle of a Bean**

The container is responsible for the entire life of the bean:

1. **Instantiation:** Spring creates the object.
2. **Populating Properties:** Spring injects any dependencies (other beans) it needs.
3. **Usage:** Your application uses the bean to do work.
4. **Destruction:** When the app shuts down, Spring cleans up the object.

---

### **How do you define a Bean?**

In modern Spring Boot, you usually define beans using **Annotations**. This tells Spring, "Hey, keep an eye on this class and manage it for me."

* **`@Component`**: The most basic way to tell Spring a class is a bean.
* **`@Service` / `@Repository**`: Specialized versions of `@Component` for business logic or database access.
* **`@Bean`**: Used inside a configuration class to manually define a bean (often used when you're integrating a third-party library).

---

### **Bean Scopes (How many are created?)**

By default, Spring beans are **Singletons**. This is a very important concept:

**Singleton** (Default):  Only **one instance** of the bean is created for the entire application. Everyone shares the same object.
**Prototype** : A **new instance** is created every single time you ask for it.
**Request** : (Web apps only) A new instance is created for every single HTTP request.
**Session** : (Web apps only) One instance per user session (e.g., a shopping cart).

---

### **Why use Beans instead of `new`?**

1. **Loose Coupling:** Your classes don't need to know how to create their dependencies; they just receive them.
2. **Easier Testing:** You can easily swap a "Real Database Bean" for a "Mock Database Bean" during testing.
3. **Centralized Management:** You can change the behavior of an object (like its scope or configuration) in one place without touching every file where it’s used.


## Previously application context used to give bean in spring, now how it is resolved in spring boot?

In traditional Spring Framework, we manually created and used the `ApplicationContext` to get beans. But in Spring Boot, this is mostly handled automatically using **Dependency Injection** with `@Autowired` or constructor injection.

Here, Spring Boot automatically:

1. Creates the bean
2. Stores it in ApplicationContext
3. Injects it where needed

So, `ApplicationContext` still exists internally, but Spring Boot manages it automatically through auto-configuration and component scanning.
