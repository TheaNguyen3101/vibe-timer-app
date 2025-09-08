# Vibe Timer (Starter)

A beginner-friendly Next.js app that implements:
- Morning goals
- Pomodoro timer with post-session note prompt
- End-of-day summary (goals vs notes)
- "Vibe" appearance using gradients + generated ambient noise (WebAudio)
- LocalStorage persistence per day (no database required)

> This is the **no-AI** starter. You can add AI image/audio later using serverless routes and providers like Replicate/ElevenLabs.

## Quick Deploy (No Coding)

### Option A — Deploy on Vercel (Upload)
1. Download this folder as a ZIP.
2. Go to vercel.com → **Add New… → Project** → **Import** → **Upload** → select the ZIP.
3. Vercel auto-detects Next.js → click **Deploy**.
4. Open the URL → use the app.

### Option B — Run locally
1. Install Node.js (>=18) from nodejs.org.
2. In terminal:
   ```bash
   npm install
   npm run dev
   ```
3. Open http://localhost:3000

## How to Use
- Add goals (left panel).
- Start the timer (center). When a focus session ends, a note modal appears.
- Set your vibe (right panel) with presets or custom text (affects gradient + ambient sound filter).
- Click **End Work Day** to view the summary.

## Next Steps (Optional Upgrades)
- Replace LocalStorage with Supabase (tables: goals, sessions, notes, vibes).
- Add `/api/vibe/generate` to call AI providers for background images and audio.
- Add auth so each user has their own data.
- Export a daily report as Markdown or PDF.
