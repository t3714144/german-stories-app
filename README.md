# Geschichten: a German reading app (A1 to C1)

Read short German stories by CEFR level, listen to them, and tap any word to save it.
Saved words are highlighted automatically in every future story where they appear again.

Goals of this repo:
1. Build a real full-stack app (React + TypeScript, FastAPI, SQLite/PostgreSQL, spaCy).
2. Use the finished app daily to improve your German.

## How to use this scaffold
- Every file contains comments that say WHAT must be coded and in WHICH milestone.
- Follow `docs/ROADMAP.md` in order. Finish one milestone before starting the next.
- Search the code for `TODO(M3)` to find all tasks of milestone 3.
- Design reference: see `docs/DESIGN.md` (Figma link inside).

## Folder map
```
docs/       overview, architecture, data model, API spec, roadmap, design, learning resources
frontend/   React + TypeScript + Vite app (pages, components, hooks, api client)
backend/    FastAPI app (routers, models, schemas, services, seed scripts, tests)
content/    story source files (JSON) and the story template
.github/    CI workflow (lint + tests)
```

## Quick start (after you implement M0)
```
# backend
cd backend && python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python -m spacy download de_core_news_md
uvicorn app.main:app --reload

# frontend (new terminal)
cd frontend && npm install && npm run dev
```

## Git habits
Small commits, one per feature: `git commit -m "M2: story list page"`.
Branch per milestone: `git checkout -b m2-reader-ui`.
