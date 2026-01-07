# Mini Library System - CC105 Final Project

## Introduction
This project is a **Mini Library System** designed to manage books, members, and borrowed books.  
It demonstrates basic database management using **MySQL** and web development using **HTML, CSS, and JavaScript**.  
The system allows users to view, add, and track books, members, and borrowed books.

## Database Design
The database consists of **3 related tables**:

1. **Books**  
   - `book_id` (Primary Key)  
   - `title`  
   - `author`  

2. **Members**  
   - `member_id` (Primary Key)  
   - `name`  
   - `email`  

3. **BorrowedBooks**  
   - `borrow_id` (Primary Key)  
   - `book_id` (Foreign Key → Books)  
   - `member_id` (Foreign Key → Members)  
   - `borrow_date` (default current date)  
   - `return_date`  

The tables are linked via foreign keys to ensure **data integrity**. Sample data is included in `mini_library.sql`.

## Web Interface
The system has **3 HTML pages**:

1. **books.html**  
   - Displays the list of books  
   - Form to add a new book  
   - JavaScript validation ensures both title and author are entered  

2. **members.html**  
   - Displays the list of members  
   - Form to add a new member  
   - JavaScript validation ensures both name and email are entered  

3. **borrowed.html**  
   - Displays borrowed book records  
   - Form to record a book borrowed by a member  
   - JavaScript validation ensures both Book ID and Member ID are entered  

## Key Functionalities
- Add new records (books, members, borrowed books)  
- View existing records in tables  
- Basic client-side form validation using JavaScript  

## Challenges and Learning
- Understanding how to structure the database with proper **primary and foreign keys**  
- Learning to create **interactive forms** with validation using JavaScript  
- Integrating **frontend forms** with sample backend data for demonstration  

## Screenshots
*(Screenshots will be added after opening each HTML page in a browser.)*
