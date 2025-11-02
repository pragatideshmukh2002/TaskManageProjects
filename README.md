# Task Manager

# Task Management System

## Tech stack
- Frontend: React (create-react-app)
- Backend: Node.js + Express
- Database: PostgreSQL
- Auth: JWT + bcrypt

## Setup (local)

### Backend
1. cd backend
2. cp .env.example .env (edit values)
3. npm install
4. Start Postgres (or use Docker)
5. Run schema: psql -U postgres -d taskmanagerdb -f sql/schema.sql
6. npm run seed  # creates test user testuser@example.com / Test@1234
7. npm run dev

### Frontend
1. cd frontend
2. cp .env.example .env (edit REACT_APP_API_URL)
3. npm install
4. npm start

## Deployment
- Build frontend: `npm run build` and deploy to Vercel/Netlify
- Backend: deploy to Render/Railway/Heroku (ensure DATABASE_URL and JWT_SECRET set in environment)
- Point frontend API calls to the deployed backend URL.

## Test user
Email: testuser@example.com
Password: Test@1234
