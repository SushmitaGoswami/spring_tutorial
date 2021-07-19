# Spring_tutorial

## Advantages: 
1. Use Java POJO. 
2. Dependency injection, inversion of contol
3. Declartive programming via AOP and many more.

## Framework:
- **Core container** :- Creating bean and making it available.
- **Infrastructure** :-  AOP, message queue, Instrumentation(Java agent like JMX), 
- **Data access layer** :- JDBC, ORM, Transaction, JMS(asynchronus way of java message service)
- **Web Layer** :- Servlet, web
- **Test layer** :- junit

## Spring projects :- 
These are add ons on core framework. example - Spring (security, LDAP, Cloud, HateOS etc.).

## Inversion of control(IOC) :- 
Out source the object creation and management to outside object factory. Based on configuration, Spring object factory provides the bean of the specific object.
Spring Container supports IOC by following configurations, 
1. XML, 
2. Annotation, 
3. Java source code


## Dependency Injection
Client delegate the call to another factory to provide the dependency while IOC create the instance of the object. DI can be achieved in 3 types
1. Constructor Injection,
2. Field Injection,
3. Method Injection.
