# 🚀 Full Stack Developer Challenge

Thanks for applying!  
This short challenge will test your ability to build a small **full-stack app** with **React (frontend)** and **FastAPI (backend)**.  
We expect this to take **~2–3 hours**. Please don’t over-engineer — focus on clean, working solutions.

---

## 🎯 Goal

Build a **mini social feed** where users can:

1. **Sign up / Log in** (with authentication).
2. **Create posts** (short text).
3. **View all posts** (feed, newest first).

---

## ⚙️ Requirements

### Backend (FastAPI + Python)

- Implement APIs:
  - `POST /auth/signup` → create user.
  - `POST /auth/login` → return JWT token.
  - `POST /posts` → create post (authenticated).
  - `GET /posts` → list posts.
- Database: SQLite (simple and local is fine).
- Use **Pydantic models** for validation.
- Store passwords securely (hash them).

### Frontend (React + TypeScript)

- Build a simple UI with two pages:
  - **Login/Signup Page** (form calling backend).
  - **Feed Page** (view posts, create post).
- Use **React Router** for navigation.
- Use **Axios or Fetch** for API calls.
- Show loading & error states.

---

## 🔐 Security Basics

Please follow these minimal security practices:

- Store passwords securely (`bcrypt` or `argon2`).
- Use JWTs with expiry; load secret from environment variables.
- Validate inputs with Pydantic; don’t return raw stack traces.
- Use ORM/parameterized queries (no raw SQL).
- Provide a `.env.example` with config values (no secrets in git).

⭐ Bonus (optional): rate limiting, refresh tokens, role-based access.

---

## 🚀 Bonus (Optional)

- Search posts by keyword.
- Styling with TailwindCSS or Material UI.
- Dockerfile for backend.

---

## 🧪 What We’re Looking For

- **Backend (30%)**: API correctness, JWT auth, clean code.
- **Frontend (30%)**: UI clarity, state management, error handling.
- **Integration (20%)**: Frontend ↔ backend works smoothly.
- **Code Quality (10%)**: Readability, structure, git commits.
- **Bonus (10%)**: Extras like search, styling, Docker.

---

## 📦 Submission

When you are finished, please submit your solution as a **zip file** containing your project.

- Include both the `frontend/` and `backend/` folders.
- If possible, also include the `.git` folder so we can see your commit history.
- Do **not** publish your solution in a public GitHub repo.

## ▶️ How to Run Your Project

Please provide clear instructions in your `README` for how to run both frontend and backend.

At minimum, include:

1. Backend setup:

   - Required Python version
   - How to install dependencies (`pip install -r requirements.txt`)
   - How to run (`uvicorn app.main:app --reload`)
   - Any required environment variables (`.env.example` recommended)

2. Frontend setup:
   - Required Node.js version
   - How to install dependencies (`npm install` or `yarn install`)
   - How to run (`npm run dev` or `npm start`)

👉 We should be able to unzip your folder, follow the instructions, and run your app locally without issues.

---

⏱ Core challenge: ~2 hours  
✨ Bonus tasks: optional
