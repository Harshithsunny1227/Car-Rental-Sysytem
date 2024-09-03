---

# Car Rental System

## Overview

The Car Rental System is a C++-based application designed to manage car rentals efficiently. It supports multiple user roles (Customer, Employee, Manager) and provides a range of functionalities, including car rental, return processing, and database management. The system is built with a focus on security, data persistence, and user-friendly interaction.

## Features

- **User Management**: 
  - Supports different user roles: Customer, Employee, and Manager.
  - Role-based access to system functionalities.
  - Secure login with password protection and authentication keys for employees and managers.

- **Car Rental Process**:
  - Rent a car, view available cars, and extend rental periods.
  - Calculate total rent and apply fines for late returns.
  - Return cars and update their condition ratings.

- **Database Management**:
  - Persistent storage and retrieval of user and car data using text file-based databases.
  - Add, update, and delete records for cars, customers, and employees.
  - Automatically updates the database files to reflect any changes made during the session.

## File Structure

- **src/**: Contains the source code files for the project.
  - `CarRentalSystem.cpp`: The main driver file for the program.
  - `cars.cpp`: Implementation of car-related functionalities.
  - `users.cpp`: Implementation of user-related functionalities (Customer, Employee, Manager).
  - `functions.cpp`: Contains utility functions used across the project.
  
- **include/**: Contains header files defining classes and functions.
  - `cars.hpp`: Header file for the `Cars` and `CarsDb` classes.
  - `users.hpp`: Header file for the `Users`, `Customer`, `Employee`, `Manager`, and `UsersDb` classes.
  - `macros.hpp`: Header file for macros and forward declarations.

- **database/**: Stores the text files used as databases.
  - `carsdatabase.txt`: Stores car details.
  - `customersdata.txt`: Stores customer details.
  - `employeedata.txt`: Stores employee details.
  - `managerdata.txt`: Stores manager details.

## Installation and Setup

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/YourUsername/Car-Rental-System.git
   cd Car-Rental-System
   ```

2. **Navigate to the Source Directory**:
   ```bash
   cd src
   ```

3. **Compile the Program**:
   ```bash
   g++ -o main.exe CarRentalSystem.cpp cars.cpp users.cpp functions.cpp
   ```

4. **Run the Program**:
   ```bash
   ./main.exe
   ```

## Usage

- **Registering a New User**:
  - Choose your role (Customer, Employee, Manager).
  - Enter your name, a unique user ID, and create a password.
  - Employees and Managers will also create an authentication key.

- **Logging In**:
  - Enter your user ID and password.
  - Employees and Managers will be prompted to enter their authentication key.

- **Main Menu Options**:
  - View available cars for rent.
  - Rent a new car or extend the rental period of an existing one.
  - View a list of cars you have rented and your total dues.
  - Change your password or authentication key (for employees and managers).
  - Managers can add, update, or delete cars, customers, and employees.


---
