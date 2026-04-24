# Graph Analyzer

Full-stack graph analysis application with a Next.js frontend and Express backend.

## Live Deployment

- Frontend: https://graph-analyzer-bajaj.vercel.app/
- Backend: https://punitjoshi-bfhl.onrender.com

## What It Does

- Accepts directed edges in format like A->B
- Validates invalid and duplicate inputs
- Builds hierarchy trees for valid components
- Detects cyclic components
- Shows summary metrics and raw JSON output

## Repository Structure

- backend: Express API server
- frontend-next: Next.js user interface

## Local Setup

### 1. Start Backend

From the backend folder:

npm install
npm start

Backend runs on port 4000 by default.

### 2. Start Frontend

From the frontend-next folder:

npm install
npm run dev

Frontend runs on port 3000 by default.

## Frontend Environment Variable

Create frontend-next/.env.local and set:

NEXT_PUBLIC_API_URL=http://localhost:4000

For deployed usage, set:

NEXT_PUBLIC_API_URL=https://punitjoshi-bfhl.onrender.com

## API Endpoint

Base URL:

- Local: http://localhost:4000
- Deployed: https://punitjoshi-bfhl.onrender.com

Route:

POST /bfhl

Content-Type must be application/json.

Example request body:

{
	"data": ["A->B", "A->C", "B->D"]
}

## Deployed App Links

- Frontend App: https://graph-analyzer-bajaj.vercel.app/
- Backend API: https://punitjoshi-bfhl.onrender.com
