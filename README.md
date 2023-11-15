# Employee Tracker

## Description

This command-line application allows business owners to view and manage departments, roles, and employees in their company. It provides functionalities such as viewing all departments, roles, and employees, adding departments, roles, and employees, and updating employee roles.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Database Schema](#database-schema)
- [Walkthrough Video](#walkthrough-video)
- [Contributing](#contributing)
- [License](#license)

## Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/your-username/employee-tracker.git
Usage
Follow the prompts to interact with the application.
Use arrow keys and follow the menu options to view and manage departments, roles, and employees.
Database Schema
The application uses the following MySQL database schema:

department

id (INT PRIMARY KEY)
name (VARCHAR(30) NOT NULL)
role

id (INT PRIMARY KEY)
title (VARCHAR(30) NOT NULL)
salary (DECIMAL(10,2) NOT NULL)
department_id (INT NOT NULL, FOREIGN KEY REFERENCES department(id))
employee

id (INT PRIMARY KEY)
first_name (VARCHAR(30) NOT NULL)
last_name (VARCHAR(30) NOT NULL)
role_id (INT NOT NULL, FOREIGN KEY REFERENCES role(id))
manager_id (INT, FOREIGN KEY REFERENCES employee(id))
Walkthrough Video
Link to Walkthrough Video

Include a video demonstrating the functionality of the application. Make sure to cover all the acceptance criteria mentioned in the assignment.

Contributing
Contributions are welcome! If you find any issues or have suggestions for improvement, please open an issue or create a pull request.

License
This project is licensed under the MIT License.
