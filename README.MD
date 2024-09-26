# Flask Bookstore project frontend
## Project Overview

Welcome to the Inkspire Library Management System! This project is designed to facilitate the management of books, customers, and loans in a library setting. Below is a comprehensive overview of the HTML pages included in this project, along with features, installation instructions, and more.

## Project Overview
Inkspire Library is a web-based application designed for the efficient management of library operations, including tracking books, customers, and loan transactions. This application allows admin users to perform CRUD operations on library records, providing an intuitive interface for managing data.

## Features
- **User Authentication:** Secure login and registration for admin users.
- **Book Management:** Add, edit, delete, and view book details.
- **Customer Management:** Add, edit, delete, and manage customer records.
- **Loan Management:** Track and manage loans, including overdue loans.
- **Responsive Design:** Mobile-friendly design using Bootstrap for optimal viewing across devices.
- **Data Validation:** Ensure accurate data entry with frontend validations.

## Technologies Used
- **Frontend:** HTML, CSS (Bootstrap), JavaScript (Axios for API requests)
- **Backend:** Flask (Python web framework)
- **Database:** SQLite for storing books, customers, and loan information.

# HTML Pages
### `index.css`
A style page for all pages in the client and admin side of the frontend.
## Client side of the frontend
### `index.html`
The homepage of Inkspire Library.
- This page introduces the user to the library system, featuring a **navbar** for easy navigation and a **search bar** to allow users to search for books by title or author.
- A **carousel** dynamically displays featured books to draw user attention.
- Buttons to login as an admin or explore the full collection of books are also present.
**Key Features:**
- Book search bar.
- Carousel showcasing featured books.
- Admin login button (opens a modal for authentication)
### `all_books.html`
Displays all books in the library.
- This page presents all the books in the system in a grid/card layout.
- Each book is represented as a **card** showing its image, title, author, and availability status.
- Users can click on a book to see more details about it or initiate a loan and get sent to the loan form in new_loan.html.
**Key Features:**
- Grid layout of books using **Bootstrap** for responsiveness.
### `new_customer.html`
A form for adding new customers.
- This page allows users to add new customer.
- Upon submission, the customer is added to the system and can start borrowing books.
### `New_loan.html`
A form for registering a new book loan.
- Users can use this page to register a new book loan for a customer.
- The form includes fields for selecting the customer, book, and loan period.
- Once submitted, the system records the loan and updates the book’s availability status.

**Key Features:**
- Form to select a customer and book for loan.
- Integration with the back-end to update loan data and availability of books.

### `return.html`
 A form to return books and delete them from loan.
 ### `about.html`
 a html page that explains about the client side of the frontend
## Admin side of the frontend
### `navbar`
Admin users can also access login and registration functionalities in the nav bar that in every admin page. all admin pages can also search for customer names as well as books names and authers.
### `off canvas`
Every admin page has a off canva button to every page in the admin side, which are:
- admin.html
- books_data.html
- customers_data.html
- loans_data.html
- about_admin.html

There also a two buttons that one deletes all tables and the other create the tables and insert data in them from the backend.
### `admin.html`
The main administration dashboard for the Library. It provides navigation to other sections of the application, including managing books, customers, and loans. 

- **Features:**
  - Easy navigation to different management sections.
  - Overview of key library statistics.

### `books_data.html`
A dedicated page for managing the library's book collection. Admin users can add, edit, delete, and view details about the books available in the library. 

- **Features:**
  - Form for adding new books.
  - Editable fields for existing book records.
  - Dynamic table displaying book information.

### `customers_data.html`
This page allows the admin to manage customer records effectively. Admin users can add new customers, update existing records, and delete customers as needed.

- **Features:**
  - Form for adding new customers.
  - Editable customer information.
  - List of all customers with options to delete or edit records.

### `loans_data.html`
A page for managing loan transactions in the library. Admin users can view all loans, including overdue loans, and update loan information.
 ### `about_admin.html`
 a html page that explains about the admin side of the frontend.

- **Features:**
  - Form for creating new loans.
  - List view of all loans with status indicators.
  - Options to edit and delete existing loans.

## Setup Instructions
To set up the Library Management System on your local machine, follow these steps:

### **Clone the repository:**
   git clone repository-url
    Navigate into the project directory:
### Install required dependencies:
    pip install -r requirements.txt