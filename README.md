# CRUD APP Using Node.js&MySQL
 Using Node.js as backend development env, MySQL as a database this is a CRUD APP 
 
 
 ## Prerequisites ##

# Before you join this tutorial it is assumed that you meet the requirements listed below:

   - Node JS installed on your PC.
   - Express JS.
   - MySQL & phpmyadmin (xampp).
   - templating engines -ejs-.
   
   
  # This application lets you to adding players to a database and also display their details from the database. You can also delete and edit player details.
  
  ## Install required modules.

# The following modules are going to be needed to successfully build the app.

    express: used to create handle routing and process requests from the client.
    express-fileupload: Simple express file upload middleware that wraps around busboy.
    body-parser: used to parse incoming request from the client.
    mysql: Node JS driver for MySQL.
    ejs: templating engine to render html pages for the app.
    req-flash: used to send flash messages to the view
    nodemon: Installed globally. It is used to watch for changes to files and automatically restart the server.

# Creating the database for the app

Copy the command below and navigate to your phpmyadmin dashboard and execute the following query in the console 
(usually found at the bottom of the page) in order to create database and table for the app.

CREATE DATABASE socka;
CREATE TABLE IF NOT EXISTS `players` (
  `id` int(5) NOT NULL AUTO_INCREMENT,
  `first_name` varchar(255) NOT NULL,
  `last_name` varchar(255) NOT NULL,
  `position` varchar(255) NOT NULL,
  `number` int(11) NOT NULL,
  `image` varchar(255) NOT NULL,
  `user_name` varchar(20) NOT NULL,
  PRIMARY KEY (`id`)
) ENGINE=InnoDB  DEFAULT CHARSET=latin1 AUTO_INCREMENT=1;

