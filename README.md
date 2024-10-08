# Hotel Management Web App

## Overview

The Hotel Management Web App is a full-stack application that allows users to manage hotel operations efficiently. It provides functionalities for administrators, customers, and staff, enabling them to handle reservations, manage room types, and facilities, and maintain customer data.

## Technologies Used

- **Frontend:** ReactJS
- **Backend:** Node.js, Express
- **Database:** MySQL
- **Other Tools:** phpMyAdmin for database management

## Features

- **Admin Panel:** 
  - Manage hotel information
  - Add, edit, and delete rooms and facilities
  - View and manage customer reservations

- **Customer Portal:**
  - Register and manage personal information
  - View available rooms and facilities
  - Make and manage reservations

- **Staff Management:**
  - Manage staff information and roles

## Database Structure

The database consists of the following tables:

1. **admin**
   - `admin_id`: Unique identifier for the admin
   - `hotel_id`: Associated hotel
   - `admin_name`: Name of the admin
   - `admin_email`: Email of the admin
   - `admin_password`: Password for admin login

2. **customer**
   - `cust_id`: Unique identifier for the customer
   - `cust_name`: Name of the customer
   - `cust_email`: Email of the customer
   - `cust_phone`: Phone number of the customer
   - `cust_password`: Password for customer login

3. **facilities**
   - `facility_id`: Unique identifier for the facility
   - `facility`: Name of the facility
   - `facility_cost`: Cost of the facility

4. **hotel**
   - `hotel_id`: Unique identifier for the hotel
   - `hotel_name`: Name of the hotel
   - `hotel_addr`: Address of the hotel
   - `hotel_email`: Email of the hotel
   - `hotel_phone`: Phone number of the hotel

5. **reservation**
   - `r_id`: Unique identifier for the reservation
   - `cust_id`: Associated customer
   - `room_id`: Associated room
   - `booking_date`: Date of booking
   - `start_date`: Start date of the reservation
   - `end_date`: End date of the reservation
   - `amount`: Total amount for the reservation (including taxes)

6. **room**
   - `room_id`: Unique identifier for the room
   - `type_id`: Associated room type
   - `facility_id`: Associated facilities
   - `status_id`: Availability status
   - `hotel_id`: Associated hotel
   - `images`: Links to room images

7. **room_status**
   - `status_id`: Unique identifier for the room status
   - `availability`: Status of the room (available/not available)

8. **room_type**
   - `type_id`: Unique identifier for the room type
   - `type_name`: Name of the room type (e.g., AC, Non-AC)
   - `cost`: Cost of the room type

9. **servents**
   - `s_id`: Unique identifier for the staff member
   - `hotel_id`: Associated hotel
   - `s_name`: Name of the staff member
   - `s_phone`: Phone number of the staff member
   - `s_adhar`: Aadhar number of the staff member
   - `s_age`: Age of the staff member
   - `s_salary`: Salary of the staff member
## Getting Started

1. **Clone the Repository:**

   ```
bash
git clone https://github.com/555Shivam/hotelmanagement_backend


