# SpringSecurityUsingUserDetailsService


* Spring Framework + Spring Security + Java Configuration + MVC + Maven , Example
* Spring Security using, AuthenticationManagerBuilder..userDetailsService(Custom UserDetailsService)
* Spring Security example for Spring 4 MVC + JSP View with pure Java Configuration (no XML), using Maven build tool.
* Spring4 + MVC, Integration without using the web.xml and Spring_Servlet.xml file. 
* By using WebMvcConfigurerAdapter class and WebApplicationInitializer interface to replace above files.

> **###1. Technologies**
* Spring 4.0.3.RELEASE
* Spring Security 3.2.5.RELEASE {spring-security-web, spring-security-config, spring-security-taglibs}
* Maven 3.1
* JSTL 1.2

> **###2. To Run this project locally**
* $ git clone https://github.com/AkashChauhanSoftEngi/SpringSecurityUsingUserDetailsService
* $ mvn tomcat7:run

> **###3.  Access** 
* http://localhost:8080/SpringSecurityUsingHibernate/
* http://localhost:8080/SpringSecurityUsingHibernate/login
* http://localhost:8080/SpringSecurityUsingHibernate/admin

> **###4. Important things to keep in mind**
* While using overloaded configure method we need to use 
  - AuthenticationManagerBuilder.userDetailsService(Custom UserDetailsService);
  - For this, we need to implement UserDetailsService interface and populate our custom data into user using UserDetails interface
  - Later jsp, will communicate through filter using user class[POJO]
  - So the authentication will be done by this way
* In this project, custom login form is being used instead of default spring security login form

