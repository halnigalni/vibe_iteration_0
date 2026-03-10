# 사주 (Saju) — Korean Destiny Reading App

English-language Korean Saju fortune-telling web app powered by Claude AI.

## Features
- 사주 풀이 — Full Four Pillars destiny reading
- 궁합 — Compatibility reading for two people
- 오늘의 운세 — Daily fortune with location detection & date picker

---

## Deploy to Vercel

### 1. Push to GitHub
```bash
git init
git add .
git commit -m "initial commit"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/saju-app.git
git push -u origin main
```

### 2. Deploy on Vercel
1. Go to [vercel.com](https://vercel.com) → Log in with GitHub
2. Click **"Add New Project"** → Select your `saju-app` repo
3. Under **"Environment Variables"**, add:
   - Name: `ANTHROPIC_API_KEY`
   - Value: `sk-ant-...` (your key from console.anthropic.com)
4. Click **Deploy**

Your app will be live at `https://saju-app.vercel.app` 🎉

---

## Project Structure
```
saju-app/
├── api/
│   └── chat.js        ← Serverless function (API key lives here)
├── public/
│   └── index.html     ← Frontend app
├── vercel.json        ← Vercel config
└── package.json
```

## Get your Anthropic API Key
→ [console.anthropic.com](https://console.anthropic.com) → API Keys → Create Key
