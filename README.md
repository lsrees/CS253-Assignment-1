# CS253-Assignment-1

# Vehicle Rental System

## Introduction
The Vehicle Rental System is an all-encompassing platform tailored for the efficient handling of vehicle rentals, developed with C++ for functionality and MongoDB for data storage. It caters to the diverse needs of customers, employees, and managers, providing tools for seamless vehicle renting, returns, and management.

## Key Features
- *Customer Interface:* Enables customers to easily rent and return vehicles, alongside accessing their rental history.
- *Employee Interface:* Provides employees with the ability to offer rentals with discounts, manage returns, and review rental records.
- *Vehicle Administration:* Facilitates adding, updating, removing, and querying vehicle information, tracking availability and conditions.
- *Secure Data Handling:* Integrates with MongoDB for robust data management of users and vehicles.
- *Access Control:* Implements authentication processes to safeguard and restrict access based on user roles.

## Requirements
- Operational MongoDB server (either locally or hosted)
- Configured MongoDB C++ Driver in your development environment
- Compiler that supports C++17 or higher

## Configuration & Setup
1. *MongoDB Configuration:*
   - Ensure MongoDB is properly installed and operational, utilizing MongoDB Atlas for a cloud solution if preferred.
   - Construct a carRentalDB database within MongoDB, containing customers, employees, and cars collections.

2. *Development Environment Preparation:*
   - Verify the availability of a C++17 standard-compliant compiler.
   - Install the MongoDB C++ Driver following the instructions provided in the [official documentation](https://mongodb.github.io/mongo-cxx-driver/mongocxx-v3/installation/).

3. *System Configuration:*
   - Adjust the MongoDB connection string within the program's main function to connect to your specific MongoDB setup.

## Execution Instructions
Compile the application with your C++ compiler, for instance, using g++ as shown below:
```bash
g++ -o vehicleRentalSystem main.cpp -std=c++17 -lmongocxx -lbsoncxx
## System Overview
- *Authentication System:* Ensures secure access to the system by verifying the identities of customers, employees, and managers through unique IDs and passwords.
- *Vehicle Handling:* Oversees the entire lifecycle of vehicles within the system, covering aspects such as availability, condition, and the rental process.
- *User Profiles:* Provides comprehensive profiles for customers and employees, showcasing rental transactions, usage limits based on standing, and discounts for employees.
- *Managerial Capabilities:* Grants managers extensive tools for database management, allowing them to affect changes to vehicles, user accounts, and transaction logs.
- *MongoDB Utilization:* Exhibits proficient use of MongoDB for data storage, highlighting CRUD (Create, Read, Update, Delete) operations via a C++ interface.

## Detailed Class Descriptions
- *User:* An abstract base class that represents a generic user within the system, laying the groundwork for more specific user types.
- *Customer & Employee:* Derivatives of the User class, these provide customized functionalities tailored to each role, including unique attributes and mechanisms for managing rentals.
- *Car:* A fundamental class that depicts vehicles in the system, complete with comprehensive attributes and status indicators.
- *Manager:* A specialized user class endowed with administrative privileges for overarching system management tasks.
- *Database:* The pivotal class for database operations, ensuring smooth interaction with MongoDB for data manipulation and user authentication.

## MongoDB C++ Integration
This project harnesses the MongoDB C++ Driver for database interactions, showcasing how to establish connections, manipulate documents, and execute queries within a C++ application.

## Conclusion
The Vehicle Rental Management System project stands as a prime example of leveraging object-oriented programming principles in C++, seamlessly integrated with MongoDB to create a robust and scalable solution for managing vehicle rentals.
