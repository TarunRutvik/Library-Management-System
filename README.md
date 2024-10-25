
# SpringBoot Application to manage Information(Authors and Books)

## Operations:

This application supports basic CRUD (Create, Read, Update) operations to manage entities within the database. Below is a summary of the functionality provided:

### 1. Populate Database:
The app automatically creates tables for identified entities using JPA. 
It then populates these tables with sample data (10 rows per table) to give a starting point for interaction and testing.

### 2. Create Operation:
Users can add new entities through a form implemented in a JSP page.
The app processes form submissions via a controller method, which validates and saves the new entities to the database.
Any integrity violations or errors are handled gracefully, providing user-friendly feedback.

### 3. Read Operation:

The app provides a view that lists all entities stored in the database.
A controller fetches data from the service layer and binds it to the JSP view for display.
The app also supports complex queries, such as performing inner joins between entities to return more detailed or related data.

### 4. Update Operation:

Users can update existing entities through the front-end interface.
A controller method processes update requests and saves the modified details to the database, ensuring data is always kept up to date.

## Requirements to Run This:

This application requires the following components to function correctly:

### 1. Entity Classes
The app defines its entities using JPA annotations like @Entity, @Id, and @OneToMany to establish relationships and constraints within the database.

### 2. Repository Layer
Repository interfaces are created by extending JpaRepository, providing easy access to database operations.
Custom query methods are included to support more complex data retrieval tasks.

### 3. Service Layer
Business logic is handled in the service layer, ensuring a seamless interaction between the controller and repository layers.
The service layer integrates with the repository to perform operations on entities.

### 4. Controller Layer
The app uses Spring MVC controllers to handle HTTP requests related to the management of entities.
It binds data between the model and view layers using JSTL or Expression Language (EL), ensuring a smooth user interface experience.

### 5. View Layer
JSP pages are used to create the user interface for adding, listing, and updating entity data.
CSS is applied to style the JSP pages, making the app visually appealing and user-friendly.

### 6. Testing
Unit tests are written using JUnit and Mockito to ensure the repository and service layers work as expected.
The app is tested for functionality by performing create, read, and update operations through the web interface.

## Techonologies Used:
1. Maven
2. JPA
3. Jquery
4. JPQL
5. JSP
6. Java Servlets(Tomcat Apache works)
7. MySQL (you can substitue this with PostGreSQL if you wish to do so)

## Setup Instructions:
The tools and technologies required to develop the application include HTML, CSS, JQuery, Java Servlets, Spring Boot, JSP, MySQL, and JPA. 

### HTML (HyperText Markup Language)

#### Role of HTML

HTML is the standard markup language used to create web pages. It provides the structure of a webpage, allowing the inclusion of elements such as headings, paragraphs, images, links, and other multimedia.

#### Installing and Setting Up HTML

HTML does not require installation. You can create HTML files using any text editor, such as Notepad, Sublime Text, or Visual Studio Code. Simply save the file with a .html extension.

### CSS (Cascading Style Sheets)

#### Role of CSS

CSS is used to style and layout web pages. It allows you to apply styles to HTML elements, controlling their appearance in terms of colour, font, size, spacing, and positioning.

#### Installing and Setting Up CSS

Like HTML, CSS does not require installation. CSS files can be created using any text editor and saved with a .css extension. CSS can be included in HTML documents using <link> or <style> tags.

### JQuery

#### Role of JQuery

JQuery is a fast, small, and feature-rich JavaScript library. It simplifies tasks like HTML document traversal and manipulation, event handling, and animation.

#### Installing and Setting Up JQuery

JQuery can be included in your project by downloading the library from the JQuery website or using a CDN. Add the following script tag to your HTML document:
```bash
<script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
```
### Java Servlets

#### Role of Java Servlets

Java Servlets are server-side programs that handle client requests and generate dynamic content. They are a core component of Java web applications.

#### Installing and Setting Up Java Servlets

Java Servlets are part of the Java EE platform. To set up, you need to install a servlet container like Apache Tomcat. Ensure you have the Java Development Kit (JDK) installed. Download and install Tomcat from Tomcat's official website.

### Spring Boot

#### Role of Spring Boot

Spring Boot is a framework for building Java-based applications. It simplifies the setup and development process by providing default configurations and an embedded server.

#### Installing and Setting Up Spring Boot

To start with Spring Boot, you need to have Java installed. Use a build tool like Maven or Gradle. You can create a Spring Boot project using Spring Initializr (https://start.spring.io/).

### JSP (JavaServer Pages)

#### Role of JSP

JSP is a technology used to create dynamic web content by embedding Java code into HTML pages. It allows for the development of dynamic, server-side content.

#### Installing and Setting Up JSP

JSP requires a servlet container like Apache Tomcat. Create JSP files with a .jsp extension and place them in the appropriate directory (usually the webapp folder in a Spring Boot project).

### MySQL

#### Role of MySQL

MySQL is a relational database management system used to store and manage application data. It is widely used due to its reliability and ease of use.

#### Installing and Setting Up MySQL

Download and install MySQL from MySQL's official website. Follow the installation instructions for your operating system.

### JPA (Java Persistence API)

#### Role of JPA

JPA is a Java specification for managing relational data. It provides an object-relational mapping (ORM) mechanism, allowing developers to work with database data using Java objects.

#### Installing and Setting Up JPA

JPA is typically used with Hibernate as the implementation. Add the necessary dependencies to your pom.xml (for Maven) or build.gradle (for Gradle) file.


Open a web browser and navigate to http://localhost:8081
