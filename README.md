# SmartPrep — Frontend

AI-powered exam preparation platform. Built with **React + Tailwind CSS + Vite**, deployable on **Vercel** in minutes.

## 🚀 Quick Start

```bash
# 1. Install dependencies
npm install

# 2. Copy environment file and configure
cp .env.example .env
# Edit .env — set VITE_API_URL to your backend URL
# Set VITE_USE_MOCK=true to run without a real backend

# 3. Start dev server
npm run dev
# Open http://localhost:5173
```

## 📁 Project Structure

```
src/
├── api/
│   ├── api.js          # All backend API calls (axios)
│   └── mockData.js     # Mock responses for demo/dev
├── components/
│   ├── Navbar.jsx
│   ├── ProtectedRoute.jsx
│   ├── TopicCard.jsx
│   ├── ProgressBar.jsx
│   ├── ResourceCard.jsx
│   ├── Spinner.jsx
│   └── ErrorMessage.jsx
├── context/
│   └── AuthContext.jsx  # Global auth state
├── pages/
│   ├── LoginPage.jsx
│   ├── SignupPage.jsx
│   ├── Onboarding.jsx
│   ├── Dashboard.jsx
│   ├── Notes.jsx
│   ├── Resources.jsx
│   └── NotFound.jsx
├── App.jsx              # Router setup
├── main.jsx
└── index.css            # Tailwind + custom styles
```

## ⚙️ Environment Variables

| Variable | Description | Example |
|---|---|---|
| `VITE_API_URL` | Backend API base URL | `https://smartprep-api.railway.app` |
| `VITE_USE_MOCK` | Use mock data (no backend needed) | `true` / `false` |

## 🔌 API Contract

The backend must implement these endpoints:

| Endpoint | Method | Request Body | Response |
|---|---|---|---|
| `/auth/signup` | POST | `{ name, email, password, examType }` | `{ token, user }` |
| `/auth/login` | POST | `{ email, password }` | `{ token, user }` |
| `/ai/recommend` | POST | `{ examType, subjects[] }` | `{ topics: [{name, priority, timeEst, subject}] }` |
| `/ai/notes` | POST | `{ topic }` | `{ notes: "markdown string" }` |
| `/resources/:topic` | GET | — | `{ resources: [{title, url, source}] }` |
| `/user/progress` | GET | — (auth header) | `{ progress: { subjectName: percent } }` |

All protected routes require `Authorization: Bearer <token>` header.

## 🌐 Deploy to Vercel

1. Push this repo to GitHub
2. Go to [vercel.com](https://vercel.com) → Import project
3. Set environment variables in Vercel dashboard:
   - `VITE_API_URL` = your Railway/Render backend URL
   - `VITE_USE_MOCK` = `false`
4. Click Deploy ✅

**Important:** Tell your backend partner to add your Vercel URL to their CORS allowed origins.

## 🛠️ Build for Production

```bash
npm run build
# Output in /dist — ready to serve
```

## 📦 Dependencies

- `react` + `react-dom` — UI framework
- `react-router-dom` — Client-side routing
- `axios` — HTTP client with interceptors
- `tailwindcss` — Utility-first CSS
- `vite` — Fast build tool
