PHARMACY MANAGER — INSTALLABLE OFFLINE WEB APP

This folder is a Progressive Web App (PWA). It must be published on a secure HTTPS website before Chrome will offer Install app / Add to Home screen. Opening index.html directly from Downloads (content:// or file://) is not sufficient.

Files:
- index.html: pharmacy inventory app
- manifest.webmanifest: app name, icon and standalone display settings
- sw.js: offline app-shell caching
- icons/: app icons

After publishing to HTTPS:
1. Open the website URL in Google Chrome on Android.
2. Wait for it to finish loading once while online.
3. Open Chrome menu (three dots).
4. Tap Install app or Add to Home screen, then confirm.
5. Open the new Pharmacy icon from the home screen. After first successful load, the app shell can open offline.

IMPORTANT DATA SAFETY:
- Medicine records are stored in the browser's IndexedDB for that website origin on that device.
- Export a Full backup regularly and keep a copy somewhere safe.
- Do not clear Chrome site data for the hosted app; doing so can erase local medicine records.
- A backup made while using the old local-file version will not automatically appear in the hosted version. Use Full backup in the old app, then Restore backup in the installed app if you have records.
- This app is an inventory and price record tool, not a prescribing or clinical decision tool.
