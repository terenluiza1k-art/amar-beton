# আমার বেতন (Amar Betan)

একটি mobile-first, offline-first Bengali salary/attendance/OT tracker.

## Features
- Monthly salary, transport, food bill and attendance bonus
- Full monthly attendance calendar
- উপস্থিত / অনুপস্থিত
- Editable OT rate (default ৳50/hour)
- OT rate snapshot stored with each saved day
- One absence in a month makes the whole attendance bonus ৳0
- Monthly income breakdown
- Salary slip + Print/Save PDF
- Local Backup / Restore
- Custom reminder ON/OFF and time
- PWA/offline app shell using Service Worker
- LocalStorage persistence; no backend required for core features

## GitHub Pages
1. Create a GitHub repository, e.g. `amar-betan`.
2. Upload all files in this folder to the repository root.
3. Go to Settings → Pages.
4. Deploy from the `main` branch and `/root` folder.
5. Open the published HTTPS URL on Android Chrome.
6. Use Chrome menu → Add to Home screen / Install app.

## Important reminder limitation
A browser/PWA cannot guarantee an exact background notification after the browser/app is fully terminated on every Android/device configuration. The app includes notification permission support and an in-app timer while the page is active. For guaranteed native Android background reminders, package this project as a native Android app or use a suitable Android wrapper with native alarm/notification APIs.

## Data
Core data is stored locally on the device. Use Backup regularly before clearing browser data or uninstalling the app.

## License
Private/project use.

## Android APK build

See `README_APK.md`. GitHub Actions automatically creates a debug APK using Capacitor.
