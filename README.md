# Employee-Tracker
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)

## Description 

The employee tracker is an applicaiton for business owners to add departments, roles and employees in order to update their business. Using the command line the business owner will be able to add, view and update departments, roles and employees. In addition, the business owner will have the option to update employee managers, view employees by manager, delete department roles and employees and view total utilized budget of the department. 

## Table of Contents

* [Installation](#installation)
* [Usage](#usage)
* [License](#license)


## Installation

Design the following database schema containing three tables:
* **department**:

  * **id** - INT PRIMARY KEY
  * **name** - VARCHAR(30) to hold department name

* **role**:

  * **id** - INT PRIMARY KEY
  * **title** -  VARCHAR(30) to hold role title
  * **salary** -  DECIMAL to hold role salary
  * **department_id** -  INT to hold reference to department role belongs to

* **employee**:

  * **id** - INT PRIMARY KEY
  * **first_name** - VARCHAR(30) to hold employee first name
  * **last_name** - VARCHAR(30) to hold employee last name
  * **role_id** - INT to hold reference to role employee has
  * **manager_id** - INT to hold reference to another employee that manages the employee being Created. This field may be null if the employee has no manager
  
Build a command-line application that at a minimum allows the user to:

  * Add departments, roles, employees

  * View departments, roles, employees

  * Update employee roles

  * Update employee managers

  * View employees by manager

  * Delete departments, roles, and employees

  * View the total utilized budget of a department -- ie the combined salaries of all employees in that department

Delivery Options:

* Use the [MySQL](https://www.npmjs.com/package/mysql) NPM package to connect to your MySQL database and perform queries.

* Use [InquirerJs](https://www.npmjs.com/package/inquirer/v/0.2.3) NPM package to interact with the user via the command-line.

* Use [console.table](https://www.npmjs.com/package/console.table) to print MySQL rows to the console. There is a built-in version of `console.table`, but the NPM package formats the data a little better for our purposes.

* Use [dotenv](https://www.npmjs.com/package/dotenv) NPM package to separate your password from your source code. 

## Usage

The following gif displays how the application is ran:
![Employee Tracker](Assets/employee-tracker.gif)

The following image displays the data base schema: 
![Database Schema](Assets/schema.png)

## License

[MIT](https://opensource.org/licenses/MIT)