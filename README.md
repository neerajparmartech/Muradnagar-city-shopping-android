# Muradnagar City Shopping — Android app project

This Android WebView app opens the existing live Google Apps Script shopping application. It does not replace or modify the website, Apps Script deployment, or spreadsheet.

## Build an APK with GitHub Actions

1. Create a new GitHub repository (for example `muradnagar-city-shopping-android`).
2. Upload the **contents** of this folder to the repository root.
3. Open the repository's **Actions** tab and enable Actions if prompted.
4. Choose **Build Android APK** and click **Run workflow** (or push to `main`).
5. When the run finishes, open the run and download the artifact named `Muradnagar-City-Shopping-APK`.
6. Extract the downloaded ZIP. The APK inside is `app-debug.apk`. Transfer it to the Android phone and install it. Android may ask to allow installation from that source.

## Notes

- This is a debug APK for testing/private distribution. A Play Store release needs a separately signed release build and Play Console setup.
- The app needs internet access and loads the existing live web app.
- Website sound/polling can work while the app is open. Android WebView does not provide the same browser Web Notifications API as Chrome, so native push notifications/background alerts are not included in this first build.
- The app does not contain admin credentials or change any backend data.
