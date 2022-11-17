# spring-framework-tutorials

<ins>Background

Spring is one of the most popular frameworks in Java and has many projects associated with it such as: Spring Cloud, Spring Security, Spring Boot and more.
The Spring framework tackles common application problems, provides patterns and a structure for Java applications, and 
is also used to develop business services.

There are several "Types of Objects" in Spring: Objects that hold data and instances of classes with business logic methods.

The way we share object instances is through **Dependency Injection**.

The Spring framework specifically provides us with: Application Context & Dependency Injection, Data Access (simplifies connecting to and working with databases), Spring MVC (web apps, rest APIs).

<ins>Supporting Material

[What is the Spring framework really all about? (YouTube/JavaBrains)](https://www.youtube.com/watch?v=gq4S-ovWVlM)
<br>

## Table of Contents
[1. Configuration](#1-configuration)
<br>
[2. Spring MVC](#2-spring-mvc)
<br>
[3. Dependency Injection](#3-dependency-injection)
<br>
[4. Available Annotations](#4-available-annotations)
<br>
[5. Scheduling](#5-scheduling)
<br>

## 1. Configuration

"Bean" is a key concept of the Spring Framework. They are the objects that form the backbone of your (Spring) application and are managed by the Spring IoC container.

Therefore, a bean is an object that is instantiated, assembled, and otherwise managed by a Spring IoC container.

Inversion of Control (IoC) = a process in which an object defines its dependencies without creating them. This object delegates the job of constructing such dependencies to an IoC container.

<ins>Supporting Material

[Spring ultimate basics: What are Spring Beans and what is the Spring Container? (YouTube/MaaikeBrightBoost)](https://www.youtube.com/watch?v=aS9SQITRocc)
<br>
[Basic @Bean @Configuration Code Example (Baeldung/NguyenNamThai)](https://www.baeldung.com/spring-bean)
<br>

### 2. Spring MVC

Spring MVC is a Java framework which is used to build web applications. It follows the Model-View-Controller design
pattern. It implements all the basic features of a core Spring framework like Inversion of Control and Dependency Injection.
 
Spring MVC provides an elegant solution to use MVC in the Spring framework by the help of DispatcherServlet. Here, DispatcherServlet is a class that receives the incoming request and maps it to the right resource such as controllers, models, and views.

- Model - contains the data of the application. The data can be encompassed within a single object or a collection of objects.

- Controller - contains the business logic of an application. Here, the @Controller annotation is used to mark the class as the controller.

- View - represents the provided information in a particular format, Generally, JSP+JSTL is used to create a view page.
Although, Spring also supports other view technologies such as Apache Velocity, Thymeleaf and FreeMarker.

In Spring Web MVC, the DispatcherServlet class works as the "front controller". It is responsible for managing the flow of the Spring MVC application.

Advantages of Spring MVC: separates the roles, light-weight servlet container, powerful configuration, rapid development, easy to test and flexible mapping.

<ins>Supporting Material

[MVC Explained in 4 Minutes (YouTube/WebDevSimplified)](https://www.youtube.com/watch?v=DUg2SWWK18I)
<br>
[Spring MVC Tutorial Code Example (JavaTPoint)](https://www.javatpoint.com/spring-mvc-tutorial)
<br>

Now that we are delving into web application and REST API related materials, it is useful to understand what backend and frontend is!

[Backend web development - a complete overview (2021) (YouTube/SuperSimpleDev)](https://www.youtube.com/watch?v=XBu54nfzxAQ)
<br>
[Frontend web development - a complete overview (2021) (YouTube/SuperSimpleDev)](https://www.youtube.com/watch?v=WG5ikvJ2TKA)
<br>

### 3. Dependency Injection

Inversion of Control is a principle in software engineering which transfers the control of objects or portions of a program
to a container or framework. We most often use it in the context of object-oriented programming.

Dependency Injection is a pattern we can use to implement IoC, where the control that is being inverted is setting an
object's dependencies.

In the Spring framework, the interface ApplicationContext represents the IoC container. The Spring container is
responsible for instantiating, configuring and assembling objects known as beans, as well as managing their life cycles.

In order to assemble beans, the container uses configuration metadata, which can be in the form of XML configuration or
annotations.

Dependency Injection is basically providing the objects that an object needs (its dependencies) instead of having it construct them itself. It's a very useful technique for testing, since it allows dependencies to be mocked or stubbed out.

Dependency Injection in Spring can be done through constructors (recommended), setters or fields.

<ins>Supporting Material

[Learn Dependency Injection and Write Better Code (YouTube/AmigosCode)](https://www.youtube.com/watch?v=eQ90v7HQT-Q)
<br>
[Understanding Dependency Injection (Stackoverflow/gtiwari333)](https://stackoverflow.com/a/6085922)
<br>

### 4. Available Annotations

Traditionally, Spring allows a developer to manage bean dependencies by using XML-based configuration.
There is an alternative way to define beans and their dependencies. This method is a Java-based configuration.

Unlike the XML approach, Java-based configuration allows you to manage bean components programmatically. That’s why Spring annotations were introduced.

Some Spring core framework annotations:
1. @Configuration
2. @Bean
3. @PreDestroy and @PostContruct
4. @ComponentScan
5. @Component
6. @PropertySource
7. @Service
8. @Repository
9. @Autowired

Some important Spring MVC annotations:
1. @Controller
2. @RequestMapping
3. @PathVariable
4. @RequestParam
5. @ModelAttribute
6. @RequestBody and @ResponseBody
7. @RequestHeader and @ResponseHeader

<ins>Supporting Material

[Spring Annotations (DigitalOcean/PankaJ)](https://www.digitalocean.com/community/tutorials/spring-annotations)
<br>

### 5. Scheduling

Scheduling is a process of executing the tasks for the specific time period. Spring Boot provides a good support to write a scheduler on the Spring applications.
The annotations associated with this operation are:
- @EnableScheduling
- @Scheduled

<ins>Supporting Material

[How to Schedule Tasks/Jobs in Springboot using @Scheduled annotation (YouTube/DailyCodeBuffer)](https://www.youtube.com/watch?v=ZXlxQ3z4zDE)
<br>