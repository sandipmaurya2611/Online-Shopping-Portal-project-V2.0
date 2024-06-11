# Online Shopping Portal

This project is an Online Shopping Portal built using PHP. It includes features for both users and administrators, such as user registration, profile management, shopping cart, product management, and order management.

## Project Features

### User Features
- **User Registration**: New users can register for an account.
- **User Login System**: Registered users can log in to their accounts.
- **Change Password**: Users can change their passwords.
- **Forgot Password**: Users can reset their passwords if forgotten.
- **Profile Management**: Users can manage their profile information.
- **Shopping Cart**: Users can add items to their cart and proceed to checkout.
- **Wishlist**: Users can add items to their wishlist for future purchase.
- **Order History**: Users can view their past orders.

### Admin Features
- **Product Management**: Admins can add, update, and delete products.
- **Order Management System**: Admins can manage customer orders.
- **User Management**: Admins can manage user accounts.
- **Category/Sub-Category Creation**: Admins can create and manage product categories and sub-categories.

## Technologies Used

- **Frontend**: HTML, AJAX, jQuery, JavaScript
- **Backend**: PHP (PHP5.6, PHP7.x, PHP8.x)
- **Database**: MySQL (MySQL 5.x, MySQL 8.x)
- **Web Browsers**: Mozilla, Google Chrome, IE8, OPERA
- **Server Software**: XAMPP / Wamp / Mamp / Lamp (anyone)

## Installation

### Prerequisites
- A web server with PHP and MySQL support (XAMPP, WAMP, MAMP, LAMP)
- A web browser (Mozilla, Google Chrome, IE8, OPERA)

### Steps

1. Clone the repository:

    ```bash
    git clone https://github.com/yourusername/online-shopping-portal.git
    cd online-shopping-portal
    ```

2. Create a MySQL database and import the provided SQL file (`database.sql`) to set up the database schema:

    ```sql
    CREATE DATABASE shopping_portal;
    USE shopping_portal;
    SOURCE path_to_database.sql;
    ```

3. Update the database configuration in the PHP files:

    ```php
    // db_config.php
    define('DB_SERVER', 'localhost');
    define('DB_USERNAME', 'your_db_username');
    define('DB_PASSWORD', 'your_db_password');
    define('DB_DATABASE', 'shopping_portal');
    ```

4. Start your web server and navigate to the project directory in your web browser:

    ```bash
    http://localhost/online-shopping-portal
    ```

## Usage

1. Register as a new user or log in with an existing account.
2. Browse products, add items to your shopping cart or wishlist.
3. Proceed to checkout to complete your purchase.
4. Admins can log in to the admin panel to manage products, orders, and user accounts.

## Project Structure

```plaintext
├── css/
│   ├── styles.css        # CSS styles
├── js/
│   ├── main.js           # Main JavaScript logic
├── admin/
│   ├── index.php         # Admin panel
│   ├── manage-products.php # Product management
│   ├── manage-orders.php # Order management
│   ├── manage-users.php  # User management
│   ├── manage-categories.php # Category management
├── user/
│   ├── register.php      # User registration
│   ├── login.php         # User login
│   ├── profile.php       # Profile management
│   ├── cart.php          # Shopping cart
│   ├── wishlist.php      # Wishlist
│   ├── order-history.php # Order history
├── index.php             # Homepage
├── db_config.php         # Database configuration
├── README.md             # Project documentation
└── database.sql          # Database schema
