Hotel Reservation System

Overview

A simple Java-based hotel reservation system using MySQL. It allows users to book rooms, view, update, and delete reservations.

Features

Reserve a Room

View Reservations

Get Room Number

Update Reservation

Delete Reservation

Requirements

Java (JDK 8 or higher)

MySQL Database

MySQL JDBC Driver

Setup

Create a MySQL database hotel_db and a reservations table:

CREATE DATABASE hotel_db;
USE hotel_db;
CREATE TABLE reservations (
    reservation_id INT AUTO_INCREMENT PRIMARY KEY,
    guest_name VARCHAR(255),
    room_number INT,
    contact_number VARCHAR(20),
    reservation_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

Update database credentials in HotelReservationSystem.java:

private static final String url = "jdbc:mysql://localhost:3306/hotel_db";
private static final String username = "root";
private static final String password = "Admin@123";

Run the Application

Compile the program:

javac HotelReservationSystem.java

Run the application:

java HotelReservationSystem

Author

Developed by Harsh Tripathi.

