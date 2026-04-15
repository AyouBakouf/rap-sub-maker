# RAP SUB MAKER 字

Tout-en-un pour tes TikToks traduction : **Decode → Sync → Export .SRT**

## Flow

1. **DECODE** — entre artiste + titre → Gemini 3 Flash cherche les paroles + traduit ligne par ligne
2. **SYNC** — importe l'audio, tape espace à chaque ligne → timings calés en temps réel
3. **EXPORT** — télécharge le .srt → importe dans CapCut

## Setup

```bash
cp .env.example .env
# Ajoute ta clé Gemini dans .env
npm install
npm run dev
```

## Deploy

Push sur GitHub → connecte sur Vercel → ajoute `VITE_GEMINI_API_KEY` dans les Environment Variables → Deploy.

## Stack

- Vite + vanilla JS
- Gemini 2.0 Flash + Google Search
- Zéro dépendance runtime
