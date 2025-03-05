# Hotel Booking Management System



## Overview
The **Hotel Booking Management System** is a web-based application designed to facilitate online room reservations, customer management, and booking tracking. It enables users to search for available rooms, make reservations, and manage their bookings efficiently. The system also provides an admin panel for hotel staff to manage room availability and customer records.

## Features
- **User Authentication:** Secure login and registration system.
- **Room Booking:** Users can search, view, and book hotel rooms.
- **Payment Integration:** Supports online and offline payment methods.
- **Admin Dashboard:** Manage rooms, bookings, and customers.
- **Email Notifications:** Sends confirmation emails for successful bookings.
- **Responsive Design:** Works across all devices.



## Tech Stack
- **Frontend:** HTML, CSS, JavaScript
- **Backend:** PHP
- **Database:** MySQL
- **Server:** XAMPP (Apache, MySQL, PHP, and Perl)

## Installation Guide
### Prerequisites
- Install **XAMPP** for running PHP and MySQL.
- A web browser (Chrome, Firefox, etc.)

### Steps to Set Up the Project
1. **Clone the Repository:**
   ```bash
   git clone https://github.com/yourusername/hotel-booking.git
   cd hotel-booking
   ```
2. **Start XAMPP and Configure Database:**
   - Open XAMPP Control Panel.
   - Start **Apache** and **MySQL** services.
   - Open `phpMyAdmin` and create a new database named `hotel_db`.
   - Import `hotel_db.sql` from the project folder.
3. **Configure the Database Connection:**
   - Open `config.php` and update the database credentials:
   ```php
   <?php
   $conn = mysqli_connect("localhost", "root", "", "hotel_db");
   if (!$conn) {
       die("Connection failed: " . mysqli_connect_error());
   }
   ?>
   ```
4. **Run the Project:**
   - Move the project folder to `htdocs` in the XAMPP directory.
   - Open a browser and visit:
     ```
     http://localhost/hotel-booking/
     ```


## How It Works
1. **User Registration & Login:**
   - Users sign up and log in to book rooms.
2. **Room Search & Booking:**
   - Users select available rooms and make a reservation.
3. **Admin Panel:**
   - Hotel staff can add, edit, and delete room listings.
4. **Booking Confirmation:**
   - Users receive an email confirmation.


