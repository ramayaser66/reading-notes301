
# Relationships in Spring Data

type of relationships:

- ## One-to-One Relationship 

 the primary key of one table exists as a foreign key on another table 

  using the` @OneToOne` annotation. 

  NOTE: The `@RestResource` annotation is optional and can be used to customize the endpoint

 - ## One-to-Many

 sing the `@OneToMany` and `@ManyToOne` annotations.

 NOTE: the optional` @RestResource `annotation to customize the association resource. 

The primary key of one table exists as a foreign key on another table. 

 - ## Many-to-Many
the association between the two entities is tracked by a cross-reference table. This is a table that holds both of the related entities’ primary keys as foreign keys.

 using `@ManyToMany` annotation

 # Integration testing  

 it verifies the end-to-end behavior of a system.

 the Spring MVC  allows to test framework in order to write and run integration tests that test controllers without explicitly starting a Servlet container.

 - Maven dependencies are required for integration tests:

 1. junit-jupiter-engine
 2.  junit-jupiter-api
 3.  Spring test
 4. Hamcrest
 5. JSON path 

## Spring MVC Test Configuration 

- Enable Spring in Tests with JUnit 5 
 
 JUnit 5 defines an extension interface through which classes can integrate with the JUnit test. 

 1. add the `@ExtendWith` annotation to our test classes and specifying the extension class to load. 

 2. add the `@ContextConfiguration` annotation to load the context configuration and bootstrap the context that our test will use.
 use the ApplicationConfig.class config class, which loads the configuration we need for this particular test.


  3. use SpringExtension.class in order to ruen the test.

  4. add the `@WebAppConfiguration`, which will load the web application context, you can pass the value attribute or by default, it looks for the root web application at path src/main/webapp. 

- WebApplicationContext Object


it provides a web application configuration. It loads all the application beans and controllers into the context

- Mocking Web Context Beans
It encapsulates all web application beans and makes them available for testing.

- Verify Test Configuration
- Write the Integration Tests:

1. Verify View Name 

`perform()` method will call a GET request method, which returns the ResultActions. Using this result, we can have assertion expectations about the response, like its content, HTTP status, or header. 

`andDo(print()) `will print the request and response. This is helpful to get a detailed view in case of an error. 

`andDo(print())` will print the request and response. This is helpful to get a detailed view in case of an error

2. Verify Response Body

`andExpect(MockMvcResultMatchers.status().isOk())` will verify that response HTTP status is Ok (200). This ensures that the request was successfully executed. 


`andExpect(MockMvcResultMatchers.jsonPath(“$.message”).value(“Hello World!!!”))` will verify that response content matches with the argument “Hello World!!!“. Here, we used jsonPath, which extracts response content and provides the requested value.

`andReturn() will return the MvcResult object`, which is used when we have to verify something that isn't directly achievable by the library. In this case, we've added assertEquals to match the content type of the response that is extracted from the MvcResult object


- Send GET Request With Path Variable
- Send GET Request With Query Parameters
- Send POST Request
