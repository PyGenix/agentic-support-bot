# Agentic Support Bot

Python FastAPI agentic customer-support assistant with tool calling.

An LLM agent loop selects tools, queries local data, and returns grounded replies suitable for support-desk demos.

## Stack

- **Backend:** Python 3.11+, FastAPI, Uvicorn
- **AI / Agents:** OpenAI function calling (`gpt-4o-mini`), custom tool loop
- **Frontend (optional demo UI):** React + Vite

## Features

- Multi-step agent loop with visible tool use
- Support-style chat endpoint
- Local tools for lookup / actions during the conversation

## Quick start

```bash
cd backend
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
cp .env.example .env   # set OPENAI_API_KEY
uvicorn main:app --reload --port 8008
```

API docs: http://localhost:8008/docs

```bash
cd frontend
npm install
npm run dev
```

## Author

Pooja Sharma — [Pooja101117](https://github.com/Pooja101117)
