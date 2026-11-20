# Jarvis AI Assistant

A small, mobile-friendly assistant designed to run in Android Chrome. It includes a chat interface, browser speech input/output, a few built-in commands, optional AI-provider connectivity, and installable/offline PWA support.

## Run it

Serve these files from a static HTTPS host (GitHub Pages works), then open the site in Chrome on your Android phone. For GitHub Pages, open **Settings → Pages**, choose the `main` branch and `/ (root)` as the publishing source, and save. Once published, visit the Pages URL and use Chrome's **Install app** / **Add to Home screen** option.

Microphone recognition requires browser support, an HTTPS origin, and microphone permission. Browser speech recognition may use the browser's speech service and may require an internet connection. Text chat and built-in commands work without an AI-provider key.

## AI replies (optional)

Open **Settings** inside Jarvis and enter an OpenAI-compatible chat-completions endpoint, model name, and (if required) API key. The credentials are stored in that browser's local storage and sent to the configured provider with each request. Use only a provider and device you trust; local storage is not encrypted. Provider pricing and free quotas vary, so check the provider's terms. Without a configured endpoint, Jarvis responds to simple built-in requests (time, date, greeting, joke, help, and web search).

This is a static front-end: do not put a private or production API key in a public deployment. For a shared/public app, use a backend proxy that protects credentials and applies rate limits.
