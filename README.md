# Paytm Application

## Project Overview

Develop and deploy a fully functional Paytm-like application with key financial services.

## Objective

Create a comprehensive financial services application featuring user registration, wallet management, money transfers, and bill payments.

## Key Components and Features

### 1. User Registration and Authentication
- **Registration:** Users register with details like name, email, phone number, and password, validated via OTP.
  - **Login:** Users log in with their email/phone number and password.
  - **Password Recovery:** Users reset their password using their registered email or phone number.

### 2. User Profile Management
- Users view and update profile information, including personal details, linked bank accounts, and KYC status.

### 3. Wallet Management
- **Add Money:** Users add money to their wallet using credit/debit cards, net banking, and UPI.
- **Balance Check:** Users check their wallet balance in real-time.

### 4. Money Transfers
- **To Bank Account:** Users transfer money from their wallet to bank accounts.
- **To Another Wallet:** Users transfer money to other users' wallets via phone number or email.

### 5. Bill Payments
- Users pay utility bills (electricity, water, gas) and recharge mobile phones.
- The app supports multiple billers and provides real-time payment status updates.

---

This project aims to provide a seamless and secure financial service experience similar to Paytm. Contributions and feedback are welcome!


- Clone the repo

```jsx
git clone https://github.com/100xdevs-cohort-2/week-17-final-code
```

- npm install
- Run postgres either locally or on the cloud (neon.tech)

```jsx
docker run  -e POSTGRES_PASSWORD=mysecretpassword -d -p 5432:5432 postgres
```

- Copy over all .env.example files to .env
- Update .env files everywhere with the right db url
- Go to `packages/db`
    - npx prisma migrate dev
    - npx prisma db seed
- Go to `apps/user-app` , run `npm run dev`
- Try logging in using phone - 1111111111 , password - alice (See `seed.ts`)
