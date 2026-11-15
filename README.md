# JARVIS Phase 1

This is a mobile-first Progressive Web App (PWA) starter. It includes a futuristic dashboard, text chat, simple local demo replies, speech synthesis, and optional browser speech recognition when supported.

## Important
- The AI model is NOT connected in Phase 1. Replies are local demo responses.
- iOS Safari support for browser speech recognition varies. If the mic button cannot start recognition, use the microphone on the iPhone keyboard to dictate into the text field.
- Speech output depends on iOS/browser voice settings.
- The app needs to be hosted over HTTPS for reliable PWA installation and service-worker support.
- Never put an OpenAI API key in `index.html` or any browser-side file. Phase 2 will use a secure backend.

## Files
- `index.html`: app interface and client-side behavior
- `manifest.webmanifest`: install metadata
- `sw.js`: offline caching service worker
- `icon-192.png`, `icon-512.png`: app icons

## Easiest iPhone-only hosting path
1. Create a GitHub account if you do not already have one.
2. In Safari, open GitHub and create a new **public** repository named `jarvis-phase1`.
3. Use **Add file → Upload files** and upload all six files from this folder.
4. Commit the upload.
5. In the repository, open **Settings → Pages**.
6. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, then save.
7. Wait for GitHub Pages to publish. Your site address will look like `https://YOUR-USERNAME.github.io/jarvis-phase1/`.
8. Open that address in Safari. Tap **Share → Add to Home Screen → Add**.

GitHub Pages publishes a public static website. Do not upload private information or API keys. If GitHub's mobile layout hides a setting, use Safari's **aA → Request Desktop Website**.

## Test
- Type `What can you do?`
- Try the quick-command buttons.
- Tap the mic button; if unsupported, use the iOS keyboard dictation microphone.
- Check whether the spoken response plays.

## Next phase
Phase 2 will connect a secure backend to an AI model. Keep API keys on the server, not in this app.
