# PersonaVault — Web Deploy

## Deploy on Railway (free)

1. Go to https://railway.app and sign in with GitHub
2. Click **New Project → Deploy from GitHub repo**
   - Upload this folder as a GitHub repo (or use Railway's drag-and-drop)
3. In project settings → **Variables**, add:
   ```
   ANTHROPIC_API_KEY = sk-ant-...your key...
   ```
4. Railway auto-detects Python and deploys. Done.

## Deploy on Render (free)

1. Go to https://render.com → **New Web Service**
2. Connect GitHub repo with these files
3. Settings:
   - **Runtime:** Python 3
   - **Build Command:** *(leave empty)*
   - **Start Command:** `python app.py`
4. Add environment variable:
   ```
   ANTHROPIC_API_KEY = sk-ant-...your key...
   ```
5. Click **Create Web Service**

## Get your Anthropic API key

1. Go to https://console.anthropic.com
2. API Keys → Create Key
3. Copy and paste into Railway/Render environment variables

## Local run

```bash
ANTHROPIC_API_KEY=sk-ant-... python app.py
```
Then open http://localhost:8080
