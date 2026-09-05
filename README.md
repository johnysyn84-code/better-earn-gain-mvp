# Better Earn Gain — MVP

A runnable Kenya-focused investment-platform prototype with landing page, registration/login, customer dashboard, investment products, demo deposits, investment creation, withdrawals, transactions, admin API, and SQLite persistence.

## Important
This MVP deliberately uses **demo payment processing**. It does not move real money and does not contain live M-Pesa credentials.

Before production:
1. Complete applicable Kenyan legal/regulatory review.
2. Obtain the appropriate Safaricom/Daraja business configuration.
3. Store credentials only as server-side secrets.
4. Implement and test verified Daraja callbacks.
5. Complete KYC/AML, client-money/custody, data-protection, security and reconciliation controls.

## Run locally

Requirements: Node.js 18+

```bash
npm install
npm start
```

Open http://localhost:3000

Demo admin:
- Email: admin@betterearngain.test
- Password: Admin123!

Demo customer:
- Email: demo@betterearngain.test
- Password: Demo123!

The database is created automatically at `data/beg.sqlite`.

## Deployment

This repository is ready to deploy on a Node.js host that supports a persistent filesystem. Set `PORT` if required. Do not commit production secrets.
