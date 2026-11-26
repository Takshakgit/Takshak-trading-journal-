# TAKSHAK TRADING JOURNAL — Android Studio project

This is an Android WebView app wrapper around the responsive journal UI.

## Build an APK
1. Install Android Studio (latest stable) on a computer.
2. Open this `TAKSHAK_Android_Project` folder in Android Studio.
3. Allow Gradle sync and install Android SDK Platform 35 if prompted.
4. Select Build > Build Bundle(s) / APK(s) > Build APK(s).
5. Find the debug APK at `app/build/outputs/apk/debug/app-debug.apk`.
6. Transfer it to your iQOO 9 SE (Android 14) and install. If Android asks, allow installing unknown apps for the app you used to open it.

## Current app functionality
- Local trade journal, BUY/SELL gross P&L less entered charges
- Local history, win-rate dashboard and CSV export
- Image selection from Android gallery through the system picker
- Data stored in this app's WebView local storage on this device

## Limitations
- This package is Android Studio source, not a compiled APK. A build machine with Android Studio/SDK is required to produce the APK.
- Data is local to this installation; no account/cloud sync or backup is configured.
- AI chart analysis is a placeholder; no AI service is connected.
- Zerodha is not connected. Broker API integration requires a secure backend and authorized Kite Connect setup. Never place API secrets in the APK.
- P&L is simplified and does not include all exchange fees, taxes, lot-size rules or slippage.
