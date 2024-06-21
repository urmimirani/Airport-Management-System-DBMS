# Airport Management System - DBMS

## Overview

The Airport Management System is designed to manage the operations of airports, airlines, flights, and passengers. It provides a comprehensive view of all aspects related to airport management, ensuring efficient handling of information.

### Contributors
- Urmi Mirani, 22BCE363
- Tvisha Patel, 22BCE361

## Features

- **Airlines**: Uniquely identified by a two-letter and three-digit code.
- **Flights**: Identified by a flight code consisting of the airline code and a four-digit number. Includes details like arrival and departure times, duration, and class types.
- **Passengers**: Identified by a passenger ID and passport number, including personal details.
- **Tickets**: Contain information about the passenger, airline, source, destination, journey date, seat number, class, and fare.
- **Employees**: Identified by their SSN with personal information and salary details.

## Project Structure

- **Tables**: Definitions and structures of all tables used in the system.
- **SQL Queries**: A set of SQL queries to retrieve and manipulate data.
- **Data Dictionary**: Detailed description of each table and its columns.
- **ER Diagram**: Entity-Relationship diagram representing the database schema.
- **Normalization**: Steps to normalize the database up to 3NF.

## Tables

The database consists of several tables including:
- `CITY`
- `AIRPORT`
- `AIRLINE`
- `FLIGHT`
- `PASSENGER`
- `TICKET`
- `EMPLOYEE`
- `SERVES`

## SQL Queries

Some key SQL queries included in the project:
1. Retrieve passenger details sorted by age in descending order.
2. Retrieve tickets with non-null cancellation dates.
3. Retrieve passengers whose last name starts with 'S'.
4. Retrieve passengers who booked a ticket but haven't traveled yet.
5. Find the total price of tickets booked by passengers aged 30 or younger.
6. Retrieve the top 3 destinations with the highest number of booked tickets.
7. Retrieve employees along with their job type and the number of employees in the same job type.

## Data Dictionary

The data dictionary provides detailed descriptions of each table and its attributes, ensuring clarity and understanding of the database structure.

## ER Diagram

The ER Diagram showcases the relationships between different entities in the database, including cardinalities such as:
- City has Airport (1:1)
- Airport contains Airline (m:n)
- Airport has Employee (1:n)
- Airline has Flight (1:n)
- Flight carries Passengers (1:n)
- Employee serves Passengers (m:n)
- Passenger books Ticket (1:n)
- Passenger cancels Ticket (1:n)

## Normalization

The database tables are normalized to the Third Normal Form (3NF) to eliminate redundancy and ensure data integrity. The process involves:
- Ensuring all tables have primary keys.
- Removing partial and transitive dependencies.

## Functional Dependencies

The project identifies and addresses several functional dependencies to comply with normalization rules, ensuring a robust and efficient database design.

## How to Use

1. Clone the repository: 
    ```sh
    git clone https://github.com/yourusername/Airport-Management-System-DBMS.git
    ```
2. Set up your database and import the provided SQL scripts.
3. Run the queries to interact with the database.

## License

This project is licensed under the MIT License.

## Contact

For any questions or collaboration, please contact:
- [Urmi Mirani](mailto:urmimirani27841@gmail.com)
