# Odo Budget — Full Starter (Frontend + Backend)

This repository is a starter for a mobile-friendly budgeting tool. It includes:
- React frontend (Vite)
- Node + Express backend with SQLite (local file)
- JWT auth, password hashing (bcrypt)
- Email signup + confirmation (nodemailer) — sender example: xani@trade-line.com.au (configure SMTP in .env)
- Sample seed data (accounts + transactions)
- CSV export endpoint
- PWA manifest and service-worker stub for offline caching

**Important:** This project is a starter. **Do not** connect to bank APIs from the client. Implement secure server-side integrations when you add real banking connections.

## Quick start (local)
1. Install Node.js (v18+ recommended).
2. In the project root run:
   ```bash
   npm install
   npm run setup  # creates sqlite DB and seeds sample data
   npm run dev    # starts backend (port 4000) and frontend (vite on 5173)
   ```
3. Open http://localhost:5173

## Environment
Copy `.env.example` to `.env` and fill values (JWT secret, SMTP creds, etc).

## Folders
- `frontend/` — React app (src/, public/)
- `backend/` — Express app, database, migrations, mailer, auth
