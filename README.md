# Shashi AI — starter prototype

This is a first, free-to-run web prototype that can be published as a website and installed on Android as a Progressive Web App (PWA).

## What works now
- Responsive chat interface with demo responses (not connected to a live AI model)
- Quick prompts for English practice, study plans, and interview answers
- Local notes and task list saved in the browser on this device
- PWA manifest and basic offline cache

## Run it
Open `index.html` in a modern browser. For full PWA/offline support, serve it over HTTPS or localhost.

## Publish for free
1. Create a GitHub account if you do not already have one.
2. Create a **public** repository named `shashi-ai`.
3. Upload `index.html`, `manifest.json`, `sw.js`, and `README.md` to the repository root.
4. In the repository, open **Settings → Pages**.
5. Under the build/deploy section, select **Deploy from a branch**, choose `main` and `/ (root)`, then Save.
6. Wait for GitHub Pages to publish your site. The published URL will be shown in Pages settings.
7. On Android, open the published HTTPS site in Chrome, tap the browser menu, then choose **Add to Home screen** or **Install app** if shown.

## Next steps to make it a real AI
1. Create a small backend (for example, a free-tier serverless function) to call an AI API.
2. Keep the API key as a server-side secret. Never place a private API key in `index.html` or a public GitHub repository.
3. Add rate limiting and a clear privacy notice.
4. Connect chat first, then add features one by one: web search, file analysis, image generation, voice, user accounts, and secure storage.
5. Test usage limits and current provider terms before sharing publicly.

## Important limitations
- The chat replies in this version are pre-written demo logic. It is not a competitor to ChatGPT/Gemini yet.
- Notes/tasks use browser localStorage, so they stay in that browser/device and may be lost if site data is cleared.
- No login, cloud sync, API integration, or real AI model is included.
- Free AI API quotas and hosting terms can change. The Gemini API free tier has limits; review the official pricing and terms before production use.
