#  creating a user registration system where users can create an account by providing username, email and password, login and logout using PHP and MySQL.

## Prerequisite
* PHP
* MySql
* PHP-MySql Connector
* Ubuntu (Or any Linux Distro)(Preassuming apache2 is already installed.)

## Setting Up Environment

* **Step First:**
  Install **PHP** using this Command.
  
  ```
  sudo apt-get install php
  ```
  
* **Step Second:**
  Install **MySql** using this command.
  
  ```
  sudo apt-get install mysql
  
  ```
* **Step Third:**
  Install **MySql-Client** using this command.
  
  ```
  sudo apt-get install mysql-client
  
  ```
* **Step Fourth:**
  Install **PHP** and **MySql** Connector for saving password.
  
  ```
  sudo apt-get install php-mysql
  ```
 
 * **Step Fifth:**
  Open terminal and paste this command to open mysql databse;
 ```
 mysql -u root -p1234
 
 ```
 * **Step Sixth:**
  Create a **database**
  ```
  create database logindetails;
  ```
  </br>
  
  ```
  use logindetails;
  
  ```
  * **Step Seventh:**
  Create a table to store user data
  
  ```
  
  CREATE TABLE `users` (
  `id` int(11) NOT NULL AUTO_INCREMENT PRIMARY KEY,
  `username` varchar(100) NOT NULL,
  `email` varchar(100) NOT NULL,
  `password` varchar(100) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=latin1;


```
 * **Step Eighth:**
 
  Clone this repository and copy the registration folder to **/var/www/html/**
 ```
  sudo cp -r registration /var/www/html/
  
 ```
 
* **Step Nineth:**

  Restart the apache server
  
  ```
  sudo systemctl restart apache2
  
 ```
