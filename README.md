# Car Dealership Database Management System

## Overview
This project is a comprehensive database management system for a car dealership. It includes the creation of tables, sequences, and triggers, as well as procedures and functions to manage and query the data effectively.

## Features
- **Table Creation**: Defines tables for clients, addresses, engines, options, showrooms, employees, vehicles, invoices, and phone numbers.
- **Data Population**: Inserts sample data into the tables for testing and demonstration purposes.
- **Stored Procedures**: Implements procedures to solve specific business problems, such as calculating total sales by employees and listing vehicles sold in a specific year.
- **Triggers**: Includes triggers to automatically update prices and prevent the deletion of critical tables.
- **Exception Handling**: Handles various exceptions to ensure the robustness of the database operations.

## Table Structure
The database includes the following tables:
- `CLIENTI`: Stores client information.
- `ADRESE_SHOWROOMURI`: Stores showroom addresses.
- `MOTOARE`: Stores engine details.
- `OPTIUNI`: Stores vehicle options.
- `SHOWROOMURI`: Stores showroom details.
- `ANGAJATI`: Stores employee details.
- `VEHICULE`: Stores vehicle details.
- `FACTURI`: Stores invoice details.
- `NUMERE_TELEFON_SHOWROOMURI`: Stores showroom phone numbers.
- `NUMERE_TELEFON_CLIENTI`: Stores client phone numbers.
- `SHOWROOMURI_ANGAJATI`: Stores the relationship between showrooms and employees.
- `VEHICULE_OPTIUNI`: Stores the relationship between vehicles and options.

## Key Procedures and Functions
### `cerinta_6`
Displays the total sales and the number of invoices issued by each employee in descending order of total sales.

### `cerinta_7`
Lists vehicles owned by clients that were sold in 2024, along with the employee who made the sale and the total sales amount for that year.

### `cerinta_8`
Returns a client's phone number and the number of vehicles they have purchased based on the client's name. Handles cases where the client does not exist or there are multiple clients with the same name.

### `cerinta_9`
Displays detailed information about a vehicle, including its manufacturing year, price, engine details, extra options, and owner (client or showroom). Handles cases where the vehicle does not exist or has no extra options.

## Triggers
### `trigger_cerinta_10`
Applies a 1% discount to all other vehicles in a showroom when a new vehicle is added, except for the newly added vehicle.

### `trigger_cerinta_11`
Updates the vehicle price when an option is added or removed.

### `trigger_cerinta_12`
Prevents the deletion of the `VEHICULE` table by raising an exception.

## Usage
To use this database management system, execute the SQL scripts in the provided order. Ensure that the database is properly set up and that all sequences and tables are created before running the procedures and triggers.

## Documentation
For detailed information about the database schema, procedures, and triggers, refer to the PDF documentation included in this repository.

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Author
[andreiOpran](https://github.com/andreiOpran)

<br>

_Last Updated: 14-01-2025_
