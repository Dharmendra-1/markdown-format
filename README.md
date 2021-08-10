![SOLID](https://miro.medium.com/max/1838/1*1Fl0dq4B7vq3zqR2k8bHdg.jpeg)

> ### **In software development, Object-Oriented Design plays a crucial role when it comes to writing flexible, scalable, maintainable, and reusable code.**

> ###  **The SOLID principle was introduced by Robert C. Martin, also known as Uncle Bob and it is a coding standard in programming.**


# 1. ***Single responsibility principle*** 

> ### This principle states that “a class should have only one reason to change” which means every class should have a single responsibility or single job or single purpose. 

> ### Example:- Take the example of developing software. The task is divided into different members doing different things as front-end designers do design, the tester does testing and the backend developer takes care of the backend development part then we can say that everyone has a single job or responsibility.

```javascript 

  function job(number){
    const double = number + number
    return double
  }

  job(5) 
```


# 2. ***Open-closed principle***

> ### This principle states that “software entities (classes, modules, functions, etc.) should be open for extension, but closed for modification” which means you should be able to extend a class behavior, without modifying it.

> ### Example:- Suppose developer A needs to release an update for a library or framework and developer B wants some modification or add some feature on that then developer B is allowed to extend the existing class created by developer A but developer B is not supposed to modify the class directly.

> ### Using this principle separates the existing code from the modified code so it provides better stability, maintainability and minimizes changes as in your code.


```javascript 

  function parent(){
    let name = "Robert C. Martin"
     
     console.log(name)
      
      function inner(){
          let name = 'Bob'

          console.log(name)
      }
    
   inner() 
  }

parent()

```


# ***3. Liskov’s Substitution Principle***

> ### The principle was introduced by Barbara Liskov in 1987 and according to this principle “Derived or child classes must be substitutable for their base or parent classes“.

> ### Example:- A farmer’s son should inherit farming skills from his father and should be able to replace his father if needed. If the son wants to become a farmer then he can replace his father but if he wants to become a cricketer then definitely the son can’t replace his father even though they both belong to the same family hierarchy.

```javascript 

  function parent(){
    let parentName = "Robert C. Martin"
     
     console.log(name)
      
      function inner(){
          let childName = 'Bob'
        
          console.log(parentName)        
          console.log(childName)
      }
    
    console.log(childName) //Error

   inner() 
  }

parent()
```


#  ***4.Interface Segregation Principle***

> ### It is similar to the single responsibility principle. It states that “do not force any client to implement an interface which is irrelevant to them“.
> ### Using this principle helps in reducing the side effects and frequency of required changes.

> ### Example:-  Suppose if you enter a restaurant and you are pure vegetarian. The waiter in that restaurant gave you the menu card which includes vegetarian items, non-vegetarian items, drinks, and sweets. In this case, as a customer, you should have a menu card that includes only vegetarian items, not everything which you don’t eat in your food. Here the menu should be different for different types of customers. The common or general menu card for everyone can be divided into multiple cards instead of just one.

```javascript

     function calculator(number){
             
        const sum = ()=>{
          return number+number
        }     
      
       const min = ()=>{
         return number - 1
       }

       const mul = ()=>{
         return number*number
       }
      
      sum()
      min()
      mul() 
     }

calculator()
```

# ***5. Dependency Inversion Principle***

> ### High-level modules/classes should not depend on low-level modules/classes. Both should depend upon abstractions.
> ### Abstractions should not depend upon details. Details should depend upon abstractions.

```javascript 

  function parent(){
    let parentName = "Robert C. Martin"
     
     console.log(name)
      
      function inner(){
          let childName = 'Bob'
        
          console.log(parentName)        
          console.log(childName)
      }
    
    console.log(childName) //Error

   inner() 
  }

parent()
```

 > ### Example :- A TV remote battery. Your remote needs a battery but it’s not dependent on the battery brand. You can use any XYZ brand that you want and it will work. So we can say that the TV remote is loosely coupled with the brand name.
