# EcoSwap Registry: Sustainable Fashion Exchange DBMS Mini Project

This project demonstrates a basic relational database system designed to track users, clothing items, and completed swap transactions for a sustainable fashion community.

## Project Overview

The **EcoSwap Registry** uses a three-table structure (`Users`, `Items`, `Swaps`) to ensure data normalization and integrity.

The project consists of two main components:
1.  **Database Schema (`ecoswap_schema.sql`):** The complete SQL code for table creation and sample data insertion.
2.  **Frontend UI (`ecoswap_dashboard.html`):** A modern, attractive, and responsive dashboard that visually represents the data using HTML and Tailwind CSS (no live database connection required for this visual demonstration).
3.  **Simulated Login (`simulated_db_login.html`):** A separate file demonstrating a secure login flow using JavaScript to simulate checking credentials against the `Users` table.

## Project Structure
EcoSwap-Registry/ ├── ecoswap_schema.sql <- The complete SQL code (Tables, FKs, Sample Data) ├── ecoswap_dashboard.html <- The main frontend UI to display item inventory and stats ├── simulated_db_login.html <- Separate file demonstrating login/password check simulation ├── requirements.txt <- List of required non-standard dependencies (Minimal for this project) └── README.md <- This documentation file

## 🛠️ How to Run

### 1. Database Setup

1.  **Prerequisites:** Install a relational DBMS (MySQL, PostgreSQL, or MariaDB).
2.  **Execution:** Connect to your database console or client (e.g., MySQL Workbench).
3.  Execute the entire contents of the `ecoswap_schema.sql` file. This will create the necessary database structure and populate it with sample data.

### 2. Frontend Demonstration

* **Dashboard:** Open `ecoswap_dashboard.html` directly in any web browser (Chrome, Firefox, etc.) to view the static visualization of the sample data.
* **Login Simulation:** Open `simulated_db_login.html` to test the login success/failure pages.
    * **Success Credentials:** Username: `EcoChic`, Password: `eco123`

## ⚙️ Key Database Concepts Demonstrated

* **Normalization:** Separating data into Users, Items, and Swaps tables.
* **Foreign Keys (`FOREIGN KEY`):** Linking `Items` to `Users` (owner) and `Swaps` to two `Items` (transaction).
* **Data Constraints:** Using `PRIMARY KEY`, `NOT NULL`, `UNIQUE`, and `ENUM` types to enforce data integrity.
* **Demonstration Queries:** Simple JOIN and GROUP BY queries are included in the SQL file for analysis.
