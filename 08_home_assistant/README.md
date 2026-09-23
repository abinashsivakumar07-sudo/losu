# Home Assistant

Domain: **Home Improvement**

This standalone chatbot uses Flask, Gemini 3.1 Flash-Lite, a temporary per-browser Flask session, and a custom branded UI.

## Local

```bash
python -m venv .venv
# Windows: .venv\Scripts\activate
# macOS/Linux: source .venv/bin/activate
pip install -r requirements.txt
python app.py
```

Set `GEMINI_API_KEY` and a strong `FLASK_SECRET_KEY` in `.env`.

## Render

Build command: `pip install -r requirements.txt`
Start command: `gunicorn app:app --workers 1`
Environment variables: `GEMINI_API_KEY`, `FLASK_SECRET_KEY` (and optionally `COOKIE_SECURE=1`). Render provides `PORT`.
