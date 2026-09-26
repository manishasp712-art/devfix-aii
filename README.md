# DevFix AI

An AI-powered developer assistant that explains and fixes code errors.
Built as an MVP for a 48-hour hackathon. Runs fully in **mock mode** — no API key required.

## Quick Start

```bash
# 1. Start the backend (port 3001)
cd server && npm install && npm run dev

# 2. Start the frontend (port 5173) — new terminal
cd client && npm install && npm run dev

# 3. Open browser
open http://localhost:5173
```

## Enabling Real OpenAI

1. `cp .env.example .env`
2. Set `OPENAI_API_KEY=sk-...` and `USE_MOCK=false`
3. Uncomment the OpenAI block in `server/services/openai.js`

## Stack
- **Frontend**: React 18 + Vite + Tailwind CSS + CodeMirror 6
- **Backend**: Node.js + Express
- **AI**: Mock (swap for OpenAI `gpt-4o-mini`)
