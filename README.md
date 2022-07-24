# :oncoming_taxi: Taxi service :oncoming_taxi:
 
 `A simple web application that supports authentication, and basic CRUD operations.`
 
 ### Features

* Sign in as a driver;
* Add/delete/view manufacturers, cars, drivers;
* Set drivers to cars;
* View your current cars.

***

### Description:

When you enter the site, Authentication Filter check if you are authenticated. If not, it redirects you to login page,
where you can log in or register by creating a new driver. After authentication, it passes you to the main page, where
you can visit the links of creating, viewing or deleting manufacturers, drivers and cars. When logged in, you can view 
your current cars. Also, you can log out by pressing the button at the header of the site.
Taxi service app uses N-tier architecture model with three layers: Controller, Service and DAO, and a relational database for storing data about manufacturers, drivers, cars and many-to-many relations between cars & drivers.

![diagram](join-db-diagram.png)

***

You can view this application deployed on heroku here: https://nameless-temple-09193.herokuapp.com/

***

### Developed with:

* Java;
* JDBC;
* Servlet API;
* MySQL;
* JSP, JSTL;
* CSS;
* Tomcat;
* Heroku.

***

### How to run this project:

* Clone this repository;
* Create a database with MySQL;
* Run init_db.sql from src/main/java/taxi/resources in your DBMS program (Workbench/Intellij IDEA/CLI);
* Fill URL, USERNAME & PASSWORD fields in src/main/java/taxi/util/ConnectionUtil.java with your db url, username & password respectively;
* Add a Tomcat configuration;
* Run your tomcat configuration;
* Or you can write in console: `java -jar target/dependency/webapp-runner.jar target/*.war`, this will run your application locally with heroku.


