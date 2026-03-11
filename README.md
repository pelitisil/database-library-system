# database-library-system
SQL-based database system designed to manage users, books, and transactions in a library kiosk.
# Library Table Management Database System

## Project Description

This project is a relational database system developed using **Oracle SQL** to manage a library study area table system. The database tracks users, user types, table locations, and seating sessions.

The system allows users to sit at a table for a limited time and automatically updates the table status through triggers and procedures.

## Features

* Management of different **user types** (student, staff, guest)
* Tracking **library tables and their locations**
* Automatic **table status updates using triggers**
* **Seating procedure** for assigning users to tables
* **Session tracking** with start and end times
* Automatic table release after a specified duration

## Database Structure

The system consists of the following main tables:

* **KULLANICI_TIPLERI** – Stores different types of users
* **KULLANICILAR** – Stores user information
* **KONUMLAR** – Stores library floor or location information
* **MASALAR** – Stores table information and current status
* **FIS_KAYITLARI** – Stores table usage sessions

## Automation

The system uses **triggers and procedures** to automate operations:

### Triggers

* Automatically updates table status when a new session is created
* Clears table information when the session time expires

### Procedure

`OTURT_KULLANICI`

This procedure assigns a user to a table and ensures that the user does not already have an active session.

## Technologies Used

* Oracle SQL
* PL/SQL
* Relational Database Design

## Sample Data

The database includes:

* Multiple user types
* Over 100 tables distributed across different floors
* Sample users and table session records for testing

## Purpose of the Project

The aim of this project is to demonstrate **database design, relational modeling, and database automation using SQL and PL/SQL**.

## Author

Database project developed as part of a university coursework.
