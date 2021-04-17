
# Spring MVC

a Java framework for building web applications
MVC stands for Model-View -Controller 

It implements all the basic features of a core spring framework like: 
- Inversion of Control 
- Dependency Injection

it provides an elegant solution to use MVC in spring framework by the help of `DispatcherServlet`, which is 
a class that receives the incoming request and maps it to the right resource such as controllers, models, and views.



Using Spring MVC will require:

1. Spring model attributes
2. Request parameters
3. Session attributes
4. ServletContext attributes
5. Spring beans



![](https://i.pinimg.com/originals/61/9f/8c/619f8c7ee117f86c232e3caff422c36e.jpg)

_____________________________________________________


- `Model: ` 
 A model contains the data of the application. A data can be a single object or a collection of object. 

  It can be accessed using views model attributes

- `Controller: `
 A controller contains the business logic of an application. Here, the @Controller annotation is used to mark the class as the controller.

 It prepares a model map with data and selecting a view to be rendered. 

- `View: ` 
A view represents the provided information in a particular format. Generally, JSP+JSTL is used to create a view page. Although spring also supports other view technologies such as Apache Velocity, Thymeleaf and FreeMarker.

In the case of Thymeleaf, it is transformed into a Thymeleaf context object, that makes all the defined variables available to expressions executed in templates.

- `Front Controller: ` 
 In Spring Web MVC, the DispatcherServlet class works as the front controller. It is responsible to manage the flow of the Spring MVC application.

![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRTdqDydTf7KHOy_QXJDLh4pM4wAo_-08_BRw&usqp=CAU)
