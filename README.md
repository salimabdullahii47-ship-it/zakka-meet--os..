# ZAKKA MEET — Local Development

This repository is a local demo of the ZAKKA MEET desktop-like web UI.

Quick start (requires Node.js):

1. Install dependencies:

```bash
npm install
```

2. Start the local static server (the project includes `server.js`):

```bash
npm start
# then open http://localhost:3001 in your browser
```

What I added/changed:

- Added missing JavaScript helper stubs in `app.js` for UI actions referenced from `index.html`.
- Fixed duplicate script/HTML tag issues in `index.html`.
- Added a camera modal video element (`standaloneLocalVideoNode`) so camera initialization has a target.
- Minor CSS utilities in `style.css` for button layout and responsive videos.
- This README with run instructions.

Notes:
- The app uses the local `server.js` to serve files on port 3001.
- Camera/microphone and screen sharing require a secure context (https) or `localhost` in modern browsers — running locally on `http://localhost:3001` should allow camera/mic access.
- External integrations (Stripe, Zoom SDK) are left as placeholders; the helper stubs show simulated behavior.

If you want, I can:
- Add real handlers for recording downloads and social integrations.
- Convert `server.js` to serve over HTTPS for testing real camera permissions.
- Add unit tests or validate in a headless browser.
