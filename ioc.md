# Inversion Of Control:
- Java is an object oriented programming language, which means everything in java revolves around objects.
- In genral, java objects are created and maintained by application(i.e developer).
- But with spring we can outsource the object creation and maintainace to spring framework.
- *Spring provide us with ***Spring IOC container*** also known as Spring Container which is like Object Factory.It takes the object responsibility*.
- We have two types of IOC Containers
    1. Bean Factory
    2. Application Context
       - *We use Application Context in most of the cases, bcz it's internally extends Bean Factory.*
- We have 2 different ways of implementing (creating) IOC Container:
    1. XML
    2. java
### 1. Using XML Configuration
           1. Create the class you wanted.(Eg: Demo)
           2. Now we need to configure xml file. This is the file which we pass to IOC container & IOC container will create the object as we told(configured) in xml file.
           3. Now pass the xml to IOC Container
           
    
           

  
      
  
