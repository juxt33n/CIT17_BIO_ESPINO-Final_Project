# CIT17_BIO_ESPINO-Final_Project

Description:
SnapShop is a user-friendly eCommerce platform designed to enable users to post, manage, and browse product listings effortlessly. It features user authentication, an intuitive dashboard, and a cropping tool for custom product images.

## Table of Contents

-[Setup](#setup)
-[Test](#test)

-------------------------------------------------------------------------------------------------------------------------------

## Setup

Setup Instructions

1. Prerequisites
A web server such as XAMPP or WAMP.
PHP (version 7.4 or higher).
MySQL database.
Browser supporting modern HTML, CSS, and JavaScript features.

2. Clone the Repository
Download or clone the project files into the htdocs (or equivalent) directory in your server:
git clone <repository-url>

3. Set Up the Database

-------------------------------------------------------------------------------------------------------------------------------

1. Start your server and navigate to the phpMyAdmin interface.
2. Create a database called user_system. 
3. Import the provided SQL file (user_system.sql) to set up the necessary tables. Use the following steps:

Open phpMyAdmin.

Select the user_system database.

Click Import and upload the user_system.sql file.

The database will include:

users: To store user information.

products: To store product listings.


4. Update Database Connection

Modify the db_connect.php file (or similar) with your database credentials:

<?php
$conn = new mysqli('localhost', 'root', '', 'user_system');

if ($conn->connect_error) {
    die("Connection failed: " . $conn->connect_error);
}
?>

5. Start the Server
   
1. Launch XAMPP or WAMP and start the Apache and MySQL services.
2. Open a browser and navigate to http://localhost/ecommerce_system/index.php

   
-------------------------------------------------------------------------------------------------------------------------------

## Test

1. User Testing

Open the site in a browser.

Login/Registration: Create a new account or log in with an existing user.

Dashboard: Navigate to the dashboard to add, edit, and delete product listings.

Image Cropping: Test the cropping functionality by uploading and cropping a product image.


2. Database Verification

Verify that user data is saved correctly in the users table.

Check that product details (name, image, price) are saved in the products table.


3. Responsive Testing

Open the site on different devices (mobile, tablet, desktop) to ensure the design is responsive.
