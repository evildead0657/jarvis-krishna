# JARVIS • Krishna

A standalone HTML voice-assistant interface with browser speech recognition, speech synthesis, local commands, and a cloud AI backend.

## Live site

GitHub Pages: https://evildead0657.github.io/jarvis-krishna/

## Backend

- Health check: `https://jarvis-backend-v9tx.onrender.com/health`
- Chat: `https://jarvis-backend-v9tx.onrender.com/chat`

Backend source: [jarvis-backend](https://github.com/evildead0657/jarvis-backend).

## Run locally

Open `index.html` in a modern browser. For microphone support, use HTTPS or localhost and grant microphone permission. Chrome on Android is recommended for browser speech recognition; availability varies by browser and device.

## Troubleshooting

1. Open the health endpoint above.
2. Confirm it returns `"status":"ok"` and `"api_key_configured":true`.
3. If the page says **CLOUD CONNECTION FAILED**, check that the Render service is awake and deployed.
4. If the page says **SERVER ONLINE · API KEY MISSING**, add `GEMINI_API_KEY` in Render Environment settings.
5. If chat shows a Gemini API error, check Render logs and the key/model configuration.

The API key belongs only in the backend hosting environment, never in this public HTML file.
