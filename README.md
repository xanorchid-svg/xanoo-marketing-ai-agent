# xanoo-marketing-ai-agent

**Repository:** `xanoo-marketing-ai-agent` · **Owner:** xanorchid-svg  

An AI-powered marketing agent that learns your brand and generates Instagram & Facebook content (captions, hashtags, strategy) with preview and scheduling.

---

## What this project is

A **production-bound** platform that acts like:

- **Creative director** — understands your visual identity and voice  
- **Social media manager** — generates captions, hashtags, and posting strategy  
- **Growth strategist** — (later) scheduling and insights  

**MVP scope:** Upload brand assets and media → generate captions + hashtags → preview in UI.  
No auto-posting, payments, or multi-user permissions in MVP.

---

## Tech stack

| Layer   | Choice              | Notes                          |
|--------|---------------------|--------------------------------|
| Frontend | **Next.js** (React) | Simple, clean UI               |
| Backend  | **Python + FastAPI**| REST API only, clear structure |
| AI       | **OpenAI APIs**     | Text, vision, embeddings       |
| Brand memory | Vector embeddings | Stored and used for consistency |

---

## Project structure

```
xanoo-marketing-ai-agent/
│
├── frontend/              # Next.js app (dashboard)
├── backend/               # FastAPI app (API + logic)
├── ai/                    # Prompts, embeddings, brand memory
├── media/                 # Image & video processing
├── docs/                  # Architecture + product notes
│
├── .env.example           # Example environment variables
└── README.md              # This file
```

- **frontend/** — User-facing dashboard (upload, preview, schedule UI).  
- **backend/** — REST API, business logic, orchestration.  
- **ai/** — Prompt templates, embedding logic, brand memory.  
- **media/** — Processing for uploaded images and videos.  
- **docs/** — Architecture decisions and product notes.

---

## Getting started

1. **Clone** the repo (if you haven’t already).
2. **Copy** `.env.example` to `.env` and set `OPENAI_API_KEY` (and any other vars you need).
3. **Backend:** From `backend/`, install deps and run the FastAPI app (see `backend/README.md` when added).
4. **Frontend:** From `frontend/`, install deps and run the Next.js app (see `frontend/README.md` when added).

---

## MVP scope (current focus)

- [x] Repo structure and docs  
- [ ] Upload brand info  
- [ ] Upload photos/videos  
- [ ] Generate Instagram caption + hashtags  
- [ ] Preview content in UI  

**Not in MVP:** Auto-posting, payments, multi-user permissions, analytics dashboards. These are flagged for later.

---

## Development rules

- **Beginner-friendly:** Clear names, comments, minimal clever shortcuts.  
- **Incremental:** One feature at a time, then explain and commit.  
- **No silent assumptions:** If unclear, ask or state the assumption.

When in doubt: optimize for **clarity**, **simplicity**, and **momentum**.
