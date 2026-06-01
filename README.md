# Bank Management System

## Overview

This is a simple **Bank Management System** developed in Python. The project allows users to create bank accounts, deposit money, withdraw money, view account details, update account information, and delete accounts. User data is stored locally in a JSON file (`data.json`).

## Features

* Create a new bank account
* Generate unique account numbers automatically
* Deposit money into an account
* Withdraw money from an account
* View account details
* Update account information
* Delete an account
* Store account data in JSON format

## Project Structure

```
Bank-Management-System/
│
├── main.py        # Main application file
├── data.json      # Database file for storing account details
└── README.md      # Project documentation
```

## Requirements

* Python 3.x

No external libraries are required. The project uses Python's built-in modules:

* json
* random
* string
* pathlib

## Installation

1. Clone the repository:

```bash
git clone https://github.com/yourusername/bank-management-system.git
```

2. Navigate to the project directory:

```bash
cd bank-management-system
```

3. Ensure that `data.json` exists in the project folder.

## Running the Project

Run the following command:

```bash
python main.py
```

or

```bash
python3 main.py
```

## Menu Options

| Option | Description            |
| ------ | ---------------------- |
| 1      | Create Account         |
| 2      | Deposit Money          |
| 3      | Withdraw Money         |
| 4      | Show Account Details   |
| 5      | Update Account Details |
| 6      | Delete Account         |

## Sample Account Record

```json
{
    "name": "Renish",
    "age": 35,
    "email": "rexbc@gamil.com",
    "pin": 1212,
    "accountNo.": "4S3n$6n",
    "balance": 5500
}
```

## Known Issues

1. Invalid account number or PIN validation may not work correctly because checks like:

```python
if userdata == False:
```

should be replaced with:

```python
if not userdata:
```

2. The application does not handle invalid user input (letters instead of numbers).

3. PINs are stored in plain text and should be encrypted in a real banking application.

4. No transaction history is maintained.

5. Multiple users can potentially receive duplicate account numbers (rare but possible).

## Future Improvements

* Add a graphical user interface (GUI) using Tkinter
* Add login/logout functionality
* Add transaction history
* Implement password hashing
* Improve error handling and validation
* Add money transfer between accounts
* Use SQLite or MySQL instead of JSON storage

## Author

Developed as a Python learning project for practicing:

* Object-Oriented Programming (OOP)
* File Handling
* JSON Data Storage
* Basic Banking Operations

## License

This project is intended for educational purposes only.
