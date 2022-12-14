<h1 align="center">
  🚕 Taxi Service
</h1>

## ⚡ Overview
This is a simple and minimalistic taxi application, designed to showcase my experience working with various Java web development technologies.

It supports authentication, registration and CRUD operations.
The program is written according to SOLID principles and Dependency Injection design pattern.

## 🚀 Features
* Display all Drivers / Cars / Manufacturers
* Display all Cars by Driver
* Create new Driver / Car / Manufacturer
* Add Driver to Car
* Soft delete Driver / Car / Manufacturer

## 📷 Screenshots
### Home screen
<img src="images/main.png" alt="Home page" width="652">

### All Drivers screen
<img src="images/allDrivers.png" alt="All Drivers page" width="652">

## 🧩 Core of the project is 3-layered architecture, implemented following SOLID principles:
- Data access layer: DAO
- Business logic layer: Services
- Presentation layer: Controllers

## 💡 Technologies:
- Java 11
- pure JDBC + MySQL
- Servlets
- JSP + JSTL
- Apache Tomcat
- Maven

## ▶️ How to run this project
#### Tools needed:

- IntelliJ IDEA Ultimate IDEA
- ApacheTomcat Tomcat
- MySQL Workbench 

1. Clone the project on your IDE
2. Use [`/resources/init_db.sql`](https://github.com/vyshnevsky/my-taxi-service/blob/main/src/main/resources/init_db.sql) to create a schema and tables.
Warning! if you already have a DB named "taxi", this script will delete it and create a new empty DB with the same name.
3. Configure [`/util/ConnectionUtil.java`](https://github.com/vyshnevsky/my-taxi-service/blob/main/src/main/java/taxi/util/ConnectionUtil.java#L9) replace URL, USERNAME, PASSWORD stubs with your properties.
4. Configure Tomcat server (it is recommended to use [version 9.0.50](https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.50/bin/))
   (Add New Configuration -> TomCat -> Local -> Fix -> taxi-service:war exploded -> OK)
5. Run project!

## 📌 UML diagram
![UML diagram](images/dbRelations.png)
