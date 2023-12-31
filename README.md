# CINEMA-APP
![International-Union-of-Cinemas-Calls-for-Open-Standards-in-the-Cinema-Industry.jpg](assets/International-Union-of-Cinemas-Calls-for-Open-Standards-in-the-Cinema-Industry.jpg)
## Introduction
Simple example of concept web app that follows RESTful API rules and supports user authentication, authorization as well as various CRUD operations, the application also has a division of beneficiaries into roles (USER and ADMIN). Created using Spring & Hibernate.

## Project structure

#### The structure of this project consists of 3 levels:
* Data access layer (DAO).
* Application layer (service).
* Presentation layer (controllers).
---
## Project functionality:
Here is the entity relations diagram to better understand app's functionality:
![Cinema_scheme.png](assets/Cinema_scheme.png)
---
## Opportunities depending on the role


User (at first you must register - when registering, a basket associated with the user will be automatically created):
* GET: /orders (display all the orders)
* GET: /shopping-carts/by-user (display the contents of the current user's shopping)
* POST: /orders/complete (complete the current order)
* PUT: /shopping-carts/movie-sessions (add movie session to the shopping cart)

Admin:
* POST: /cinema-halls (add new cinema hall)
* POST: /movies (add new movie)
* POST: /movie-sessions (add new movie session)
* PUT: /movie-sessions/{id} (update movie session with specified id)
* DELETE: /movie-sessions/{id} (delete movie session by id)
* GET: /users/by-email (find user by email)

User and Admin:
* GET: /cinema-halls (display all the cinema halls)
* GET: /movies (display all the movies)
* GET: /movie-sessions/available (display all the available movie sessions)
---
## Technologies used ⚙️:

* Java 17
* Hibernate 5.6.14.Final <img src="assets/58480887cef1014c0b5e48ec.png" style="width: 20px; height: 20px;" />
* Spring Core 5.3.20
* Spring Web 5.3.20 <img src="assets/spring-3-logo-png-transparent.png" style="width: 20px; height: 20px;" />
* Spring Security 5.6.10
* MySQL 8.0.33<img src="assets/mysql-logo-png-transparent.png" style="width: 40px; height: 20px;" />
* Apache TomCat 9.0.76
* Maven  4.0

___
## How to start the application
1. Clone this project from GitHub;
2. Install Apache Tomcat version 9.x.x.;
3. Install Postman for sending requests;
4. Create an empty database using your Database Management Systems;
5. In the db.properties change YOUR_URL, YOUR_USERNAME and YOUR_PASSWORD values to the ones you specified when installing MySQL, also change JDBC_DRIVER;
6. Add Tomcat configuration;
7. Run the project and enjoy !

