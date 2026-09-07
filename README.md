# Dev Cheatsheet

Personal reference built while developing Scribtive OS — real commands, real mistakes, real fixes.

## What's inside

### Language & Tool Reference
| Section | Contents |
|---|---|
| **Git & GitHub** | Workflow, mistake recovery, CI/CD, worktrees |
| **Docker** | Flags explained, container management, ephemeral storage warning |
| **SQL / PostgreSQL** | Queries, pgvector, advisory locks, Alembic migrations, SQLAlchemy |
| **Python** | Sync vs async, generators, asyncio thread safety, Windows event loops (DriverHandle) |
| **TypeScript** | Type-only imports (TS1484), interfaces, async patterns |
| **React** | Class vs function components, hooks (useState/useEffect/useCallback/useMemo/useRef/useReducer), Error Boundaries |

### Architecture & Patterns
| Section | Contents |
|---|---|
| **Patterns** | SSE streaming, FastAPI routes & Depends(), hybrid vector search, Microsoft OAuth (AMR), prompt caching, security rules |

### Local Dev & Operations
| Section | Contents |
|---|---|
| **Dev Setup** | Python venv on Windows, `.env` vs `os.environ`, pydantic-settings gotcha, PowerShell session-only `$env:`, docker-compose vs docker run |
| **Running the App** | Backend (FastAPI/uvicorn) + frontend (Vite/React) startup, troubleshooting table |

## Run locally

Just open `index.html` in a browser — no build step, no server needed.

## Deploy to GitHub Pages

1. Create a new repo on GitHub (e.g. `dev-cheatsheet`)
2. Push this folder to it:
   ```bash
   git init
   git add .
   git commit -m "initial cheatsheet"
   git remote add origin https://github.com/YOUR_USERNAME/dev-cheatsheet.git
   git push -u origin main
   ```
3. Go to repo Settings → Pages → Source: **Deploy from branch** → Branch: `main` / `/(root)` → Save
4. Your site will be live at `https://YOUR_USERNAME.github.io/dev-cheatsheet/`
