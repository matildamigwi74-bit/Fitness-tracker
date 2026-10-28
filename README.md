# Fit & Flourish
Mobile-first offline-friendly personal fitness tracker.

## Run locally
In this folder run `python -m http.server 8000 --bind 0.0.0.0` and visit http://localhost:8000 on your laptop.

On your Android phone, while on the same Wi-Fi, open `http://LAPTOP_LAN_IP:8000` (replace with the laptop's local IP). The laptop must stay running for this URL to work. Some networks block device-to-device access. If Windows Firewall prompts, allow Python on private networks only.

For a proper installable Android PWA, serve the folder over **HTTPS** (e.g., static hosting). Open it once online, then use Chrome > Add to Home screen / Install app. The service worker caches the app for offline use. Plain HTTP LAN addresses usually cannot install a service worker or work offline.

All entries are stored in browser localStorage on that device; there is no account or sync. Export JSON backups regularly. Browser storage can be cleared by the OS or user. Imported backup files should come from trusted sources.
