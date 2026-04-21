# Pixora TikTok Analytics API

API server for Pixora Chrome Extension analytics feature.

## Deploy to Render (Free)

1. Fork or push this repo to your GitHub
2. Go to [render.com](https://render.com) and create a new **Web Service**
3. Connect your GitHub repo
4. Set these settings:
   - **Build Command:** `pip install -r requirements.txt`
   - **Start Command:** `uvicorn my_api:app --host 0.0.0.0 --port $PORT`
5. Click Deploy

## Endpoints

- `GET /` — Health check
- `GET /api/analyze?username=yourtiktok` — Fetch last 30 videos with stats

## Local Run

```bash
pip install -r requirements.txt
python my_api.py
```

Server runs at `http://localhost:8000`
