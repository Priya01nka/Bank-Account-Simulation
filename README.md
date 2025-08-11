# Bank-Account-Simulation
This project simulates a simple banking system using Java (Spring Boot) for the backend and HTML, CSS, and JavaScript for the frontend. It allows a user to perform basic banking operations such as deposit and withdraw, while maintaining the account balance and transaction history in a database.

Key Features
Deposit & Withdraw
Users can deposit and withdraw money from their account. Withdrawals are only allowed if there is a sufficient balance.

Transaction Recording
Every transaction (deposit or withdrawal) is saved with:

Transaction type
Amount
Date and time
Associated account

Real-time Updates
After each operation, the backend returns a status (OK or INSUFFICIENT) to the frontend, ensuring immediate feedback to the user.
Backend Logic (Spring Boot)
Account entity stores account details and balance.
Transaction entity stores details of each operation.
BankService handles deposit/withdraw logic and interacts with the database.
BankController exposes REST endpoints (/deposit, /withdraw) for frontend communication.
Frontend (HTML, CSS, JavaScript)
Simple form to enter deposit or withdrawal amounts.
Buttons trigger AJAX requests to backend endpoints.
Status messages displayed for success or failure.

Database Integration
Uses JPA with a database (H2 or PostgreSQL) to store accounts and transactions persistently.



Database Integration
Uses JPA with a database (H2 or PostgreSQL) to store accounts and transactions persistently.
