<h1>Introduction to Spring Framework</h1>


What is Framework:
---
Framework is a software component/tool which provides in-built capabilities or functionalities, out-of-the-box solutions in terms of in-built services, plugins or libraries which helps us to build an application seamlessly fast and also helps us to keep our source code intuitive and modular.

What is the difference between Framework & Technologies:
---
Framework provides us ready-made tools and services to build any application seamlessly and also helps us to maintain our source-code modular and intuitive per industry guidelines which is very important now a days.
On the other hand if we are using simple technologies in order to build anything i.e. application then may be for the same requirement we have to write a bit longer code which is not recommended by IT industry at all. 
SO if we are using any technologies in order to build a real-time application then may we have to write bit longer code for the same requirement if we would use any framework also it is very much possible that  if you are using any technology in order to build a real-time application then your source code won’t look institutive and modular which is not at all accepted by the industry.
Again if we are using any technology then may be you have to depend on any third party libraries to provide some sort of services.

What is Spring:
---
Spring is a Java based back-end application development framework which is used to build or create enterprise applications seamlessly.
What is Spring Module/ Spring Architecture:
It is also known as modular framework or framework of frameworks because it provides or contains/comprises/incorporates various different modules under it; collectively called as Spring framework.
Which is different from one another and can be used independently ( for different purpose); Spring framework mainly provides 5 different modules under it; these are:
1) Spring Core Module or Spring Core IOC Container Module
2) Spring Web Module
3) Spring Data Access & Integrations Module
4) Spring AOP Module
5) Spring Testing Module
Again each module itself contains various other sub modules under it { which we will discuss late on one by one }.
Each module in Spring framework is different from each other and can be used independently in the project based on our requirement.

*NOTE*
---
One important thing we should know is that it is not one big framework which mean when we looked at our maven dependencies which are present in our project then its not one big spring jar file present there. There are a lot of small jars file which are present like:  spring-core; spring-beans; spring-context; spring-aop; spring-jcl; spring-desk etc. 
SO spring is not really one big framework.  SO its not like we have to use the entire spring framework. Spring is built in a very modular way. And this enables us to use specific modules without using the other modules of spring.
For example, if we want to use the IOC and DI functionalities/features in our project in order to inject the dependency from one class to another class then we should use Spring core module.

Likewise, if we want to build a web based application then we should use Spring web module.
This Spring module again comprise 4 different sub modules under it; these are: Web, Web-Servlets, Web-Struts and Web-Portlet.
Let’s suppose I want to build a web application using Spring framework but I don’t want to use Spring framework itself because since it a small scale application so I simply want to use simple Servlet/JSP technologies to build this project. For that requirement too Spring provides us a solution in the form of Web-Servlet sub module of Spring Web Module.

Again let’s suppose I want to build a web based application for my requirement but my requirement is to use Struts framework for this requirement too Spring has a solution. Spring provides us Web-Struts sub module for this requirement. SO using this module we can easily build a web application development using Struts framework.
Similarly, If my requirement to build full-fledged, secured, more scalable enterprise-application development then Spring has a solution for it also. We can use Spring MVC module to build large scale enterprise applications.
So we can see that Spring provides us end to end solutions for our work and in addition to this it also doesn’t force us to use its own framework instead it provides us in-built functionality of other technologies and framework. That’s why it is called as framework of frameworks.

In addition to these modules Spring Team/Spring framework also provides various other in-built advanced functionalities in the form of separate jar or set of jars files which are collectively called as Spring Projects.

Spring Projects:
---
So Spring Team provides various other advanced functionalities under the umbrella of Spring Projects in order to build the application seamlessly and institutively. 



Features of Spring:
---
What is the various features of spring framework : Why spring: Why spring is so popular among developers: What are the advantages of spring framework:
1) It is very popular framework so far: has Big Community Support: 
It is one the very few framework in Java world that remains as popular today as it was 15 years back. I remembered most of the framework from those days has lost their context. But spring is one of the very few framework which retains its popularity even today. 
Spring has a big community support. It exists in the market since 2003 and still dominating the market because Spring framework provides end-to end application development support.
Under the umbrella of Spring Project Spring teams also provide lots of advanced services to make any application development experience very easily and seamlessly.
Spring Team provides large umbrella in order to build any application very easily called Spring Project. Spring has evolved a lot during this period.
There is huge evolution in the architecture of applications during this decade. However Spring mange to stay relevant through variety of spring modules and spring projects.
2) Spring doesn’t entertain any plumbing code at all:
The second reason why spring is so popular because there is No Plumbing Code at all in our project development. Plumbing code means unnecessarily code that is not required in our application development. 
In plumbing code we have to write lots of try-catch block to handle the exceptions. But in spring we are not required to focus on handling exception instead we can just focus on our business functionalities like this.

> Private void insertTodo(Todo bean){
  jdbc.Template.update(INSERT_TODO_QUERY, bean.getDescription(), bean.isDone());
} 

> public void deleteTTodo(int d){
  jdbc.Template.update(DELETE_TODO_QUERY, id );
}

> public List<Todo> retrieveAllTodos() throws SQLException {
  return jdbc.Template.query(SELECT_ALL_TODOS, new TodoMapper() );
}

In Spring we almost write 0 exceptional handling code because spring makes all its exceptions unchecked. So we don’t really need to do all the EH all these stuffs.
So with spring we don’t  required to write a plumbing code. So if we are writing 100 lines of code in spring then it is most probably some business logic only.

3) Spring is a modular framework:
The third reason why spring is very popular is it’s architecture flexibility it brings in. Spring is very modular framework.  Spring provides various different modules which are collectively called as Spring framework and some other advanced features in the form or separate jar or set of jars called Spring Projects which we can use/pick up in our project development based on our requirement without using all others.
So even though spring has really good MVC framework module however it still offers good support to all the other  MVC frameworks like struts. Even though spring has its own REST support through spring MVC module but still it does offers good support with JAXRS as well. 
So if we use spring in my project then my options are not really restricted.
SO if we choose to use spring in my project the we are still have the flexibility to choose other frameworks as well.
4) And the last reason why spring is really popular is it is able to stay with the current trend. For ex, in the last few years there is lots of evolutions with micro-services and cloud. And spring is able to come up with projects which helps it stay relevant, Spring has introduced the new project called Spring cloud, there is SB as well which helps us to develop MSs very quickly,. So these things makes spring retain its popularity.
5) Enable testable code: The most important reason that spring is so popular is because it enables writing testable code.
The core feature of spring is its DI and if we use DI properly then we would be able to write UTs for our code very easily.
Spring has really good integration with fws like Junit and mockito so it enables us to write good UTs very quickly.

SO these are the FIVE main reasons why spring remains popular because It Enable testable code, because it does not have any plumbling code at all, because it is flexible architecture and because it stays up with the trend.

1)	It is a Open source Light-weight and Loosely-Coupled application:
So Spring  makes our application/component more light weight and loosely coupled. Spring applications are LW and LC.
So Spring  makes our application/component more light weight and loosely coupled. Spring applications are LW and LC. Spring framework does not force us to use inheritance concept instead force us to use association concept to make our application light-weight and it also does not force us to create an object of one component inside another component to make components tightly-coupled instead it so force us to  use interface rule and RTP concept to make our components loosely coupled.
The Spring Framework doesn't force the programmer to inherit any class or implement any interface. That is why it is said non-invasive.
Spring is  a LW framework because of POJO class and Spring is LC  framework because of DI concept.
2)	POJO classes/ Java Beans class:
Spring simply use POJO/Java Bean class in order to implement its components.
It does not force us to extends any class or implements any interface in our component. Instead it simply uses association concept.
If we want the functionality or behavior of any other class in our own component then instead of extending that class we can simply associate with that class by using association oops concept.
For example, lets suppose we want the functionality of class B in class A then instead of extending the class B in our class A we can simple associate class B in class A by creating the object of class B in class A.
But in this way it will make our two classes TC.
SO Spring recommends us to use association i.e. has-a-relationship instead of inheritance i.e. is-a-relationship.
If we are using has-a-relationship or association model instead of extending-model in our component then our component will become light-weight also.
3)	It is thought of as a fw of fw:  because it provides support to various frameworks such as Struts, Hibernate, Tapestry, EJB, JSF, etc. 
The Spring framework comprises several modules such as IOC, AOP, DAO, Context, ORM, WEB MVC etc.
4)	In Spring we don’t need to extends or implements any classes or interfaces. In Spring we just write simple POJO classes or Java bean class to create controller, business or DAO layers. SO simple POJO classes are enough to create controller, business and dao layers by using spring.
All the required features i.e. super class or interface we can pass through our IOC container in the xml configuration file.
  
Spring Application Areas:
---
What are the various application areas of spring or using spring framework what kind of application we can build:
Using spring framework we can build n nos. of applications because it provides end-to-end project development solutions from presentation layer or UI layer till persistence layer/data source layer.
So using spring framework we can build Standalone applications by using Spring core module because it doesn’t require any app/web server.
Using Spring we can also build simple to complex web based application by using Spring Web module which further contains various 4 sub modules to build web based applications.
Using Spring we can also build Enterprise based applications by using Spring Web MVC Module.
Using spring we can also build micro-services based applications or REST applications or integration applications or interoperable applications by using Spring Web MVC module and by using SpringBoot.
SpringBoot is one of the Spring Project provided by Spring team which is mainly used to build web services or micro-services very easily.
  
What are the various companies using Spring:
---
Most top most companies called FAANG i.e. Facebook, Amazon, Apple, Netflix, Google using Spring framework undoubtedly.

What are the disadvantages of Spring framework:
---
As per as my knowledge I don’t find any disadvantages with spring as such instead it only provides us lots of benefits only.
However, since it’s so vast framework and it has solution for every problem so sometimes for developers it’s hard to figure out where exactly we need to start with.
Except this I don’t find any problem with spring.

{Until now whatever we have been using is the core container of the spring fw. Here we will use Spring beans, core, context and SPEL. So we will create an AC and we will use spring to manage our dependencies which is beans.}

