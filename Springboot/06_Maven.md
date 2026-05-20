## What is Maven?
Maven is a build automation tool used primarily for Java projects. It manages a project's build, documentation, reporting, dependencies, and distribution. Maven uses a Project Object Model (POM) to manage the project's configuration and dependencies.  

## Why use Maven in Spring Boot?
1. **Dependency Management**: Maven automatically downloads and manages the libraries your project depends on, including transitive dependencies (dependencies of your dependencies).
2. **Build Automation**: Maven provides a standardized way to build your project, run tests, and package your application.
3. **Project Structure**: Maven enforces a standard directory structure for your project, making it easier to understand and maintain.
4. **Integration with IDEs**: Most modern IDEs have built-in support for Maven, making it easier to manage dependencies and build your project.
5. **Plugins**: Maven has a rich ecosystem of plugins that can be used to perform various tasks such as code analysis, testing, and deployment.

## How to understand that a project is using Maven?
Look for a `pom.xml` file in the root directory of the project. This file is the Project Object Model (POM) file that Maven uses to manage the project. It contains information about the project, its dependencies, and build configuration. If you see a `pom.xml` file, it indicates that the project is using Maven for build and dependency management.

## “Maven reduces importing jar or libraries” - explain

In a normal Java project, if you want to use external libraries, you must:

* Download the `.jar` files manually
* Add them to the project build path
* Manage versions yourself
* Download dependent libraries separately

This becomes difficult when a project uses many libraries.

## How Maven helps:

Apache Maven automatically manages project dependencies (libraries).
Instead of manually downloading JAR files, you just write the dependency details in `pom.xml`.

Example:

```xml
<dependency>
    <groupId>org.springframework</groupId>
    <artifactId>spring-core</artifactId>
    <version>6.1.0</version>
</dependency>
```

Maven will:

* Download the required JAR automatically
* Download all dependent JARs
* Store them in the local repository
* Add them to the project classpath

> Maven removes the need to manually download and add JAR files because it automatically manages libraries and dependencies.

## Advantages

* Faster project setup
* Automatic dependency management
* Version control
* Easy project sharing
* Reduces errors from missing JARs

Official website: [Apache Maven](https://maven.apache.org)


## How to add library dependencies using Apache Maven? Example: Add OpenCSV Dependency in Maven Project

- Open the Maven Repository website

Usually you will see: [Maven Repository](https://mvnrepository.com), Click it.

- Search for OpenCSV, click the OpenCSV library result.

- You will see many versions, click the latest version number.

- On that page you will see different tabs: Click **Maven**.

- Copy the dependency code:

```xml
<dependency>
    <groupId>com.opencsv</groupId>
    <artifactId>opencsv</artifactId>
    <version>5.9</version>
</dependency>
```
- Open your project in IDE, go to  pom.xml

- Paste the code inside `<dependencies>`

Example:

```xml
<dependencies>

    <dependency>
        <groupId>com.opencsv</groupId>
        <artifactId>opencsv</artifactId>
        <version>5.9</version>
    </dependency>

</dependencies>
```

After saving:

* Maven downloads the JAR automatically
* Adds it to your project
* You can now use OpenCSV in Java code


* [OpenCSV Project](https://opencsv.sourceforge.net/)
* [Apache Maven](https://maven.apache.org)

