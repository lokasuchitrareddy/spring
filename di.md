# Dependency Injection
- It's nothing but injecting dependencies(helper objects).
- The client(developer/application) delegates to anthor object(ApplicationContext/IOC Container) the responsibility of providing it's(Client's) dependencies(helper objects).
- Spring container will automatically provide/injects your dependecies.
### Dependency Injection can done in 3 ways
1. Constructor Injection

   
               @Component
               public class Car
               {
                  private final Engine engine;

                  // Constructor Injection
                  @Autowired
                  public Car(Engine engine)
                  {
                    this.engine = engine;
                  }
              }

2. Setter Injection

               @Component
               public class Car
               {
                  private Engine engine;

                  // Setter Injection 
                  @Autowired
                  public void setEngine(Engine engine)
                  {
                    this.engine = engine;
                  }
              }
   
3. Feild Injection

   
               @Component
               public class Car
               {
                   @Autowired
                   private Engine engine;
                }



![Screenshot (13)](https://github.com/user-attachments/assets/9fa6043e-72eb-4ab1-8d4c-d4cfc133868e)


    
  
