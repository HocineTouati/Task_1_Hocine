# First Project Java – Spring MVC Application

## Project Description

This project is a simple Spring MVC web application developed using Spring Boot and Thymeleaf.

The application demonstrates the basic concepts of Spring MVC, including:

- Creating a Spring Controller
- Handling HTTP GET requests
- Passing data from a Controller to a View
- Using Thymeleaf templates
- Displaying static resources such as images
- Using request parameters in URLs

---

## Technologies Used

- Java 21
- Spring Boot
- Spring MVC
- Thymeleaf
- Maven

---

## Project Structure

```text
src
 └── main
      ├── java
      │     └── pl
      │          └── edu
      │               └── vistula
      │                    └── first_project_java
      │                         ├── FirstProjectJavaApplication.java
      │                         └── controller
      │                              └── HelloController.java
      │
      └── resources
            ├── templates
            │     └── greeting.html
            │
            └── static
                  └── vistula.png
```

---

## Application Features

### Home Page

The application redirects users to the greeting page.

Endpoint:

```text
/
```

---

### Greeting Page

Endpoint:

```text
/greeting
```

Displays a greeting message using Thymeleaf.

Default output:

```text
Hello, World
```

---

### Greeting With Custom Name

The application accepts a request parameter named `name`.

Example:

```text
/greeting?name=Hocine
```

Output:

```text
Hello, Hocine
```

---

## Controller Example

The controller handles incoming requests and sends data to the Thymeleaf template.

Example endpoint:

```java
@GetMapping("/greeting")
public String greeting(String name, Model model)
```

---

## Static Resources

The application displays a static image stored in:

```text
src/main/resources/static
```

The image is rendered inside the Thymeleaf template.

---

## How to Run the Project

1. Clone the repository
2. Open the project in IntelliJ IDEA
3. Reload Maven dependencies
4. Run the Spring Boot application
5. Open your browser
6. Navigate to:

```text
http://localhost:8080/greeting
```

or

```text
http://localhost:8080/greeting?name=YourName
```

---

## Learning Objectives

This project demonstrates:

- Spring Boot application setup
- Spring MVC controllers
- Request mapping
- Request parameters
- Thymeleaf templates
- Model attributes
- Static resource handling

---

## Author

Hocine Touati
