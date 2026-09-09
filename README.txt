SCPS Discipline App - PWA Wrapper

This folder is the installable phone wrapper for the existing Google Apps Script discipline app.

Files
-----
index.html             Main PWA wrapper
manifest.webmanifest   App name, icon and standalone settings
service-worker.js      Caches only the small wrapper files
icon-192.png           Android/PWA icon
icon-512.png           Android/PWA icon
apple-touch-icon.png   iPhone/iPad home-screen icon

IMPORTANT
---------
The learner and incident data are NOT stored in this PWA package.
The real app and database remain in Google Apps Script / Google Sheets.

The wrapper currently points to:
https://script.google.com/macros/s/AKfycbzy-vzBco0LJpzhniHpaU1G1DiRXf-KRbmdvN69gdwkTe7aSzoZQZN4Xt4f8st7q01REA/exec

Hosting
-------
The folder must be hosted over HTTPS for proper PWA installation.
A free static host such as GitHub Pages can host these files.

After hosting:
1. Open the hosted PWA URL on Android Chrome.
2. Use Chrome menu -> Install app / Add to Home screen.
3. On iPhone Safari, use Share -> Add to Home Screen.
4. The SCPS logo should be used as the app icon.
5. When opened from the installed icon, it should use standalone app-style display.

Do not share the /dev Apps Script URL. The wrapper uses the stable /exec URL.
