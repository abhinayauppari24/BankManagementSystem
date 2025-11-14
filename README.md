Bank Management System

Simple console-based Bank Management System built with Java and MySQL.
Supports user registration, login, account creation, deposit/withdraw, and basic transaction management.

1. Project Summary
This project demonstrates a simple banking application using JDBC for database access and follows a modular OOP design (Account, Customer, User, DBConnection, etc.). It is intended as a learning/demo project.

2. Features

User registration and login

Account creation with dynamic account number generation

Deposit and withdraw operations

View account balance

Uses PreparedStatement for secure queries (prevents SQL injection)

Persistent storage with MySQL


3. Tech Stack

Java (JDK 11/17+ recommended)

MySQL 8.x (or compatible)

JDBC (mysql-connector-j)

VS Code (Extension Pack for Java)


4. Folder structure
BankManagementSystem/
├─ src/
│  └─ BankManagementSystem/
│     ├─ BankingApp.java
│     ├─ DBConnection.java
│     ├─ User.java
│     ├─ Account.java
│     └─ ... other classes
├─ config/
│  └─ db.properties         # NOT checked into git (contains DB credentials)
├─ lib/
│  └─ mysql-connector-j-<ver>.jar   # local dependency (ignored)
├─ .gitignore
└─ README.md

5. Prerequisites

Java JDK installed (java -version, javac -version)

MySQL server running (mysql -u root -p)

MySQL Connector/J JAR (download from MySQL website)

(Optional) VS Code with Extension Pack for Java


6. Running the app
A) Command line (compile & run)

From project root:

Compile

javac -cp "lib/mysql-connector-j-<ver>.jar;src" src/BankManagementSystem/BankingApp.java


Run

java -cp "lib/mysql-connector-j-<ver>.jar;src" BankManagementSystem.BankingApp


On macOS/Linux replace ; with : in -cp.

B) Run inside VS Code (recommended)

Ensure .vscode/settings.json contains:

{
  "java.project.referencedLibraries": [
    "lib/**/*.jar"
  ]
}


Open BankManagementSystem folder in VS Code.

Open BankingApp.java and click the green Run button (or use Run/Debug).











