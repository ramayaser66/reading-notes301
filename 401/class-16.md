

# Spring Security 

## Authentication and Access Control

a powerful and highly customizable authentication and access-control framework.
 Spring Security is a framework that focuses on providing both authentication and authorization to Java applications.


 it provides:
 - Comprehensive and extensible support for both Authentication and Authorization

- Protection against attacks like session fixation, clickjacking, cross site request forgery, etc

- Servlet API integration

- Optional integration with Spring Web MVC


`AuthenticationManager`

 **Authentication**

 the interface for authentications, it has one method that can do: 

 - Return an Authentication.
 if it can verify that the input is a valid principal.

- Throw an AuthenticationException if the input is an invalid principal.

It is handled by an application depending on the application itself.

- Return null if it cannot decide.

it's used: 
 ProviderManager

 delegates to a chain of AuthenticationProvider instances, which resembles an AuthenticationManager, but it has an extra method to allow the caller to query whether it supports a given Authentication. 


 * Customizing Authentication Managers
  it provides some configuration helpers to get common authentication manager features set up in the application
like, 

`AuthenticationManagerBuilder`
  it set up in-memory, JDBC, or LDAP user details or for adding a custom UserDetailsService.


 **authorization**

implementations provided by the framework:

- AccessDecisionVoter 
considers an Authentication and a secure Object, decorated with ConfigAttributes

## Web Security

maintains a filter chain internally where each of the filters has a particular responsibility and filters are added or removed from the configuration depending on which services are required.

![](https://miro.medium.com/max/2380/1*jmzLl8Z3w-TpfHmmLKcg2Q.png)

