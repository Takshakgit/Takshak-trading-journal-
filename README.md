# TAKSHAK TRADING JOURNAL — starter project

## Included
- Responsive website / installable Progressive Web App (PWA)
- Add BUY/SELL trades and calculate gross P&L less entered charges
- Local trade history, search, CSV export
- Multiple screenshot attachments per trade (stored in this browser's localStorage)
- Dashboard, win rate and a bilingual AI-review placeholder

## Run locally
Use a local static server from this folder, for example:
`python -m http.server 8000`
Then open `http://localhost:8000`.

## Install on Android
1. Deploy this folder to an HTTPS host (for example, your own hosting provider).
2. Open the deployed URL in Chrome on Android.
3. Use Chrome menu → Install app / Add to Home screen.

This is the same responsive PWA for desktop and Android. A signed native APK is not included.

## Important limitations
- Trades and screenshots are stored only in the current browser/device. Clearing site data can delete them. Export CSV regularly.
- No account login, cloud sync, database backup or multi-device sync is configured.
- Zerodha is shown as the intended broker, but no Kite Connect/API credentials or broker integration are included. Never put API secrets in browser code.
- AI chart analysis is a placeholder. To enable it, create a secure backend that authenticates users, stores images safely, and calls a vision model without exposing API keys in the app. AI output must be checked manually.
- P&L calculation is a simplified gross calculation based on entry, exit, quantity and user-entered charges. It does not calculate taxes, contract-specific lot sizes, slippage or all exchange/broker fees.
- This starter is not financial advice or an execution/trading system.

## Android APK path
For a native Android package, wrap the deployed web app with Capacitor in a separate Android build environment, configure the Android project, then build and sign the APK/AAB. This source zip does not contain a compiled APK.
