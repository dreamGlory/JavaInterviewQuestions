<!-- TOC -->

- [Spring面试常问点](#Spring面试常问点)
    - [IOC（控制反转）](#IOC(控制反转))
    - [AOP（面向切面）](#AOP(面向切面)) 
    - [DI（依赖注入）](#DI(依赖注入))
    - [@ComponentScan ](#ComponentScan)
    
<!-- /TOC -->

# Spring面试常问点  

## IOC(控制反转)  

&emsp;&emsp;所谓的IoC，对于Spring来说，就是由Spring来负责控制对象的生命周期和对象间的关系。所有的类都会在Spring容器中登记，并告诉Spring你能做什么、需要什么，然后Spring会在系统运行到适当的时候，把你要的主动给你，同时也把你交给其他需要你的东西。所有的类的创建、销毁都由 Spring来控制，也就是说控制对象生存周期的不再是引用它的对象，而是Spring。对于某个具体的对象而言，以前是它控制其他对象，现在是所有对象都被Spring控制，所以这叫控制反转。  

## AOP(面向切面)  

&emsp;&emsp;面向切面编程

## DI(依赖注入)  

&emsp;&emsp;  

## ComponentScan  
&emsp;&emsp;@ComponentScan用于批量注册bean。这个注解会让Spring去扫描某些包及其子包中所有类，然后将满足一定条件的类作为bean注册到Spring容器中。  
&emsp;&emsp;默认情况下，任何参数都不设置，会将@ComponentScan修饰的类所在的包作为扫描包，默认情况下useDefaultFilters为true，Spring容器内部会使用默认过滤器。  
常用参数：  
&emsp;&emsp;value：指定要扫描的包，例：com.demo  
&emsp;&emsp;basePackages：作用跟value一样，但不能和value同时存在  
&emsp;&emsp;basePackageClasses：指定一些类，Spring容器会扫描这些类所在的包一起子包中的类  
&emsp;&emsp;nameGenerator：自定义bean名称生成器  
&emsp;&emsp;useDefaultFilters：对扫描的类是否启用默认过滤器，默认为true  
&emsp;&emsp;includeFilters：过滤器：用来配置被扫描出来的那些类会被作为组件注册到容器中  
&emsp;&emsp;excludeFilters：过滤器，和includeFilters作用刚好相反，用来对扫描的类进行排除的，被排除的类不会被注册到容器中  

