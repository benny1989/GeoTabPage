
# GeoTab Dashboard Add-In

This repository contains a MyGeotab Add-In that sends the currently logged-in user info to an API.

## ✅ How to Deploy on GitHub Pages

1. Fork or clone this repository to your GitHub account.
2. Push the contents to your repo (e.g. `GeoTabDashboardAddin`).
3. Go to your GitHub repository > **Settings** > **Pages**
   - Source: Select `main` branch and `/ (root)`
   - Click Save
4. Your GitHub Pages site will be live at:
   ```
   https://<your-username>.github.io/<repo-name>/
   ```

## ✅ Update Your `manifest.json` in MyGeotab

Use this as your `manifest.json`:

```json
{
  "name": "SendLoggedInUser",
  "supportEmail": "support@yourdomain.com",
  "version": "1.0",
  "items": [
    {
      "page": "https://<your-username>.github.io/<repo-name>/index.html",
      "title": {
        "en": "Send User"
      },
      "icon": "https://<your-username>.github.io/<repo-name>/images/icon.svg",
      "order": 100,
      "path": "Dashboard"
    }
  ]
}
```

✅ Done! Now it will show in the Dashboard menu of MyGeotab.
