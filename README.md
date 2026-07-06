# SportesHub Frontend

Sports discovery platform — find venues, academies, coaches, tournaments and communities.

## Tech Stack
- **Framework:** Next.js 16 (App Router)
- **Styling:** Tailwind CSS v4
- **Runtime:** Node.js 22+
- **Deployment:** Railway (Docker)

## Local Development

```bash
# Install dependencies
npm install

# Start dev server
npm run dev
# Open http://localhost:3000
```

## Demo Login
- Email: `demo@sporteshub.com`
- Password: `demo123`

## Build & Run with Docker

```bash
docker build -t sporteshub-frontend .
docker run -p 3000:3000 sporteshub-frontend
```

## Deploy to Railway
1. Push to GitHub
2. Connect repo on railway.app
3. Railway auto-detects the Dockerfile
4. Click Deploy

## Environment Variables
No required environment variables for local dev. For production, add as needed via Railway dashboard.

## API Routes
| Route | Method | Description |
|-------|--------|----------|
| `/api/health` | GET | Health check |
| `/api/auth/login` | POST | User login |
| `/api/auth/register` | POST | User registration |
| `/api/venues` | GET | List venues |
| `/api/venues/[id]` | GET | Single venue |
| `/api/shops` | GET | List shops |
| `/api/events` | GET | List events |
| `/api/coaches` | GET | List coaches |
| `/api/bookings` | POST/GET | Bookings |
| `/api/contact` | POST | Contact form |
| `/api/business/register` | POST | Business listing |