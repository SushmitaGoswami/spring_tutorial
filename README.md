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


### Constructor Injection
Create the bean of main object and a constructor with dependency object, in spring configuratiion file, 
```
    <constructor-arg ref="dependency_bean">
    Behind the scene spring will pass the instance of the dependency bean in the constructor of the main object.
```

### Field/setter Injection
Create the bean of main object and a setter with dependency object, in spring configuratiion file,
```
			<property name="fortuneService" ref="dependent_bean_object"> 
      spring will call setFortuneService()and pass the dependent bean object during creation of the main object.
```

### Scope of a spring bean
Scope of a bean defines the following information,
	a. How many instance will be created?
	b. How will it be shared?
	c. How long will it live?
	
 Following are the some of the different scopes possible,
 1. **Singleton** :- only 1 instance is created by spring container, shared among all the beans who have requested the bean and lives until program executes. This is the default and used for stateless.
 2. **Prototype** :- For each container request/reference, 1 instance would be created.
 3. **Request** :- For each web request, 1 instance would be created.
 4. **Web-Session** :- Created for each web session, 1 instance would be created.

	
