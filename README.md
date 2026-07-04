# Library Management - Dependency Injection using Spring

## Overview

This project demonstrates **Dependency Injection (DI)** using the Spring Framework. The `BookRepository` dependency is injected into the `BookService` class using **Setter Injection** configured through the `applicationContext.xml` file.

## Technologies Used

- Java
- Spring Framework (Spring Core)
- Maven
- XML Configuration

## Project Structure

```text
LibraryManagement/
│
├── pom.xml
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/
│   │   │       └── library/
│   │   │           ├── MainApp.java
│   │   │           ├── service/
│   │   │           │   └── BookService.java
│   │   │           └── repository/
│   │   │               └── BookRepository.java
│   │   └── resources/
│   │       └── applicationContext.xml
```

## Features

- Demonstrates Spring IoC (Inversion of Control).
- Implements Dependency Injection using Setter Injection.
- Configures dependencies using XML.
- Retrieves Spring-managed beans from the IoC container.

## Dependency Injection

The `BookRepository` bean is injected into the `BookService` bean using the following configuration:

```xml
<property name="bookRepository" ref="bookRepository"/>
```

## How to Run

1. Clone the repository.
2. Open the project in your preferred IDE.
3. Allow Maven to download the required dependencies.
4. Run `MainApp.java`.

## Expected Output

```text
Book Service is working...
Book Repository is working...
```

## Learning Outcomes

- Understand Spring IoC Container.
- Configure Setter Injection using XML.
- Manage dependencies between classes using Spring.
- Load and use Spring beans from the Application Context.

## Author

**Harini**
