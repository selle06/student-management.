Student Management System

A simple web-based Student Management System developed using:

Node.js

Express.js

EJS

MySQL

Git

GitHub

Features

View students

Add students

Edit students

Delete students

Search students

Form validation

Installation

Clone the repository:

git clone https://github.com/selle06/student-management.git


Install dependencies:

npm install


Database Setup

Open MySQL / PHPMyAdmin.

Create the database:

CREATE DATABASE student_management;
USE student_management;


Create the students table:

CREATE TABLE students (
    id INT AUTO_INCREMENT PRIMARY KEY,
    student_id VARCHAR(20) NOT NULL UNIQUE,
    first_name VARCHAR(100) NOT NULL,
    last_name VARCHAR(100) NOT NULL,
    course VARCHAR(100) NOT NULL,
    year_level INT NOT NULL,
    email VARCHAR(150) NOT NULL,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);


Configure the database connection

Create a .env file or configure your app.js settings:

DB_HOST=localhost
DB_USER=root
DB_PASSWORD=
DB_NAME=student_management


Run
node app.js


Open
Navigate to: http://localhost:3000
