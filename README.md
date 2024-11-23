# spring
- Hello GenZ. We are going to learn Spring in this repository.
- We learn, write , understand together.
# To start with you must have the following softwares in your system 
1. jdk 17 or higher (spring 3 support only after the version)
2. Any java IDE( I will be using Eclipse)
3. Now add Spring Tools (STS) Plugin in Eclipse
Open Eclipse IDE.
Go to Help -> Eclipse Marketplace.
In the search box, type "Spring Tools" and press Enter.
Find "Spring Tools (aka Spring IDE and Spring Tool Suite)" in the list and click Install.


# What is "Spring"
- I can say its a popular java framework to develop enterprise web application.
- It as a large number of helper classes and annotation

### Problem with spring
- Developing a traditional spring application is really hard because
1. Which JAR dependencies do I need for this Spring project?
2. How do I set up configuration?
Should I use XML configuration or Java configuration?
4. How do I install the server?
Tomcat, JBoss, WebSphere and so on.
- Now ***Springboot*** comes into the picture
# Springboot
Optimized version of spring which reduces manual configuration and provide a embedded server. Overall it solves the problem with spring.
- Example:
  - Using **Spring** is like baking a cake from scratch. You buy all the ingredients, measure everything, mix it, and bake it. You have complete control, but it takes time and effort.
  - Using **Spring Boot** is like using a ready-made cake mix. You just add water (or minimal effort), follow a simple instruction, and your cake is ready much faster. It’s less work and perfect if you don’t need to customize everything.
# Spring vs Springboot
- research on your own and make a list.
# Spring Initializer
- It's a website provided by Spring to create a spring starter project. It's wrap everything you need like jdk, **maven**/gradle, dependencies(avoid snapshot versions)(spring-web, spring-jpa .. etc) and download it as a .war/.jar. Now import that folder to your IDE and you are all set with a web application.

![Screenshot (5)](https://github.com/user-attachments/assets/4b7c1290-3f10-495b-8bbc-1ca00e38077a)


# How to run a spring boot application
- spring boot app can run standalone(Embedded server) (your .jar file, open in IDE then run (or) with commandline java -jar youappname.jar)
- we can run in tradional way(take your .war file then deploy in the server(tomcat))

# why am I using Maven (Maven is a project management tool)
When building your Java project,you may need additional JAR files.For example, Spring, Hibernate, Commons Logging,JSON and so forth.And one approach is to simply download the JAR files  from each project website  and then manually add those JAR files  to your build/classpath.  And that's fine and that'll work okay.However, Maven provides a nice solution.  We simply tell Maven the projects that you're working on,the dependencies like Spring, Hibernate, etcetera.Maven will go out and download the JAR files for those projects for you and Maven will automatically make those JAR files available during compile and run.
  - POM(***project object Model***) ---> read about pom.xml structure for full level understanding

![Screenshot (4)](https://github.com/user-attachments/assets/e4619349-4c41-46e6-a25b-41f27928f621)

# Spring Starter
- A Spring Starter is a feature provided by Spring Boot to simplify dependency management in your project. It is essentially a pre-defined set of libraries bundled together for specific functionalities. By adding a single starter to your project, you automatically include all the necessary dependencies without having to manage them individually.
###  Examples of Common Spring Starters
1. **spring-boot-starter-web :** Used to build web applications (including RESTful APIs). It includes dependencies like Spring MVC, Tomcat (embedded server), and JSON processing.

2. **spring-boot-starter-data-jpa:** Used for working with relational databases using JPA (Java Persistence API). It includes Hibernate and Spring Data JPA.

3. **Spring-boot-starter-security:** Provides security features like authentication and authorization for your application.
- **In a Maven project, you simply include the starter as a dependency in your pom.xml**
- **Spring-boot-starter-parent** is a pre-configured setup in Maven that provides default settings, dependency versions, and build tools, so you can start building your app with less effort.
- **spring-boot-dev-tools** automatically restart your web application. Just add this dependency in pom.xml


# Spring Project Structure

![Screenshot (6)](https://github.com/user-attachments/assets/6ffa7d16-5d46-423d-91e2-7c1118475adf)









