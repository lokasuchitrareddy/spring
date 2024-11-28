# Inversion Of Control:
- Java is an object oriented programming language, which means everything in java revolves around objects.
- In genral, java objects are created and maintained by application(i.e developer).
- But with spring we can outsource the object creation and maintainace to spring framework.
- *Spring provide us with ***Spring IOC container*** also known as Spring Container which is like Object Factory.It takes the object responsibility*.
# We have two types of IOC Containers
    1. Bean Factory
    2. Application Context
       - *We use Application Context in most of the cases, bcz it's internally extends Bean Factory.*
       - It implemented in the following ways
              1. ClassPathXmlApplicationContext : When your configuration file (beans.xml) is packaged with the application (e.g., in the resources folder).
              2. FileSystemXmlApplicationContext : When the XML configuration file is located outside the application (e.g., on a server, shared directory, or any external file location).
              3. AnnotationConfigApplicationContext : When you prefer Java-based configuration over XML for better readability and type safety.
        
 ![Screenshot (10)](https://github.com/user-attachments/assets/1c948754-0333-442d-a6ea-c09b5efcfd1a)

# We have 2 different ways of implementing (creating) IOC Container:
    1. XML
    2. java
    
### 1. Using XML Configuration

1. Create the class you wanted.(Eg: Demo)
![Screenshot (7)](https://github.com/user-attachments/assets/be1d2b5e-cd81-4873-a1b2-b5b35919b051)
2. Now we need to configure xml file. This is the file which we pass to IOC container & IOC container will create the object as we told(configured) in xml file. ***Xml file created in resources folder (most of people use that way)***
![Screenshot (8)](https://github.com/user-attachments/assets/4c4c4bdb-3d8c-4d67-947f-1e0db97b392b)
3. Now pass the xml to IOC Container
![Screenshot (9)](https://github.com/user-attachments/assets/79124fe6-741b-4062-b4bb-f29b690f207a)


### 2. Using Java Configuration

We use annotations like :
1. **`@Configuration`** - Marks a class as a setup for Spring beans (like a settings file).  
2. **`@Bean`** - Defines a method that gives Spring an object to manage (a recipe for creating things).  
3. **`@Component`** - Marks a class as something Spring should automatically manage (like registering it).  
4. **`@ComponentScan`** - Tells Spring where to look for classes marked as `@Component`.  
5. **`@Service`** - Similar to `@Component`, but specifically for service (business logic) classes.  
6. **`@Repository`** - Marks classes that deal with the database (like saving and retrieving data).  
7. **`@Controller`** - Marks classes that handle web requests (like a traffic cop for your app).  
8. **`@Autowired`** - Automatically connects one object to another (like plugging in a cable).  
9. **`@Qualifier`** - Helps pick the right object if there’s more than one choice.  
10. **`@Scope`** - Tells Spring how many instances of a bean to create (one or multiple).

1. Create a class you wanted(Eg : Demo) and annoted it with @Component
![Screenshot (11)](https://github.com/user-attachments/assets/e1329b60-f420-40b6-9805-8bb8def95a05)

2. Define a config class using annotations like @Configuration
3. Now pass the config class to IOC Container
![Screenshot (12)](https://github.com/user-attachments/assets/c25d25db-857d-4451-a84d-8a4afd24880c)


  

           
    
           

  
      
  
