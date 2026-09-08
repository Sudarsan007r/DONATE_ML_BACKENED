# Donate ML — Payment Backend

A minimal Express backend for a "round-up donation" feature — rounding up a purchase/transaction amount and forwarding the difference as a donation.

## Tech Stack

Node.js, Express, CORS, dotenv. Razorpay is included as a dependency for payment processing integration.

## What it does

- `GET /health` — health check endpoint
- `POST /roundup-donation` — accepts a donation amount and source, currently logs the request (payment processing via Razorpay is not yet wired up)

## How to Run

```bash
npm install
# create a .env file with PORT and any Razorpay credentials
node server.js
```

The server starts on the port set in `.env` (defaults to 4000).
