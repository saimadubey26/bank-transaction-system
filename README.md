# Bank Transaction System

A backend banking application built using Node.js, Express.js, and MongoDB. It provides secure user authentication, account management, fund transfers, and ledger-based transaction tracking.

## Features

- User registration and JWT authentication
- Account creation and balance management
- Secure account-to-account fund transfers
- Double-entry ledger system
- Idempotency to prevent duplicate transactions
- MongoDB transactions for atomic operations
- Email notifications using Nodemailer

## Tech Stack

- Node.js
- Express.js
- MongoDB
- Mongoose
- JWT
- Nodemailer

## Installation

```bash
git clone https://github.com/saimadubey26/bank-transaction-system.git
cd bank-transaction-system
npm install
```

## Create a .env file with the required database, JWT, and email credentials.

Start the server:
```bash
node server.js
```

Server runs on 
```bash 
http://localhost:3000
```

## API

### Authentication

POST `/api/auth/register` — Register user  
POST `/api/auth/login` — Login user  
POST `/api/auth/logout` — Logout user  

### Accounts

POST `/api/accounts/` — Create account  
GET `/api/accounts/` — Get user accounts  
GET `/api/accounts/balance/:accountId` — Get account balance  

### Transactions

POST `/api/transactions/` — Transfer funds  
POST `/api/transactions/system/initial-funds` — Add initial funds


Author:
Saima Dubey
