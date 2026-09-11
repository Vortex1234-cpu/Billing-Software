# Shop Billing

A simple offline billing app for a bakery / tea & snacks shop.
No server, no database, no login — everything is stored on the device it's used on.

## Files in this folder

| File | Purpose |
|---|---|
| `index.html` | The whole app (HTML + CSS + JS, self-contained) |
| `manifest.json` | Lets the phone install it as a real app icon |
| `sw.js` | Lets it keep working with no internet after first load |
| `icon-192.png`, `icon-512.png` | App icons |

## Deploy it free on GitHub Pages

1. Go to [github.com](https://github.com) and create a **new repository** (e.g. `shop-billing`). Keep it Public.
2. Click **Add file → Upload files**, and upload all 5 files above into the root of the repo (not inside a folder).
3. Commit the changes.
4. Go to the repo's **Settings → Pages**.
5. Under "Build and deployment", set **Source: Deploy from a branch**, **Branch: main / (root)**, then **Save**.
6. Wait about a minute, then refresh — GitHub will show your live URL, something like:
   `https://your-username.github.io/shop-billing/`

That URL is your real billing software. No further setup, no server costs, no maintenance.

## Install it on the shop's phone

1. Open the GitHub Pages URL in Chrome (Android) or Safari (iPhone).
2. Tap the browser menu → **Add to Home Screen** (or you may see an automatic "Install" prompt on Android).
3. It now behaves like a normal app icon — opens full-screen, works with no internet, no browser bar.

## Updating the app later

Whenever you want changes, just re-upload the updated file(s) to the same GitHub repo (or ask me to make the change and re-share the files) — GitHub Pages updates automatically within a minute or two of a new commit. The person using the app doesn't need to do anything except have internet the next time they open it once, so the new version can download and cache.

## Setting this up for a new shop (reselling)

The item list ships with a generic starter menu (teas, coffee, snacks) that any shop can tweak.

1. Deploy as normal (steps above) and hand the phone/link to the new shop owner.
2. In the app, they set their own **Shop name** (Settings) and add/edit/delete items from the **Add Item** tab — tap an existing item to edit its name, Tamil name, price, photo, or stock status.
3. If they'd rather start over with the sample menu instead of the one you left in there, Settings → **Reset Menu to Sample Items** brings back the starter list without touching sales history.
4. Each phone/browser keeps its own separate data — nothing is shared between shops even if they use the same GitHub Pages link.

## Important things to know

- **All data (products, sales history, QR code, PIN) is stored only on that one phone/browser.** Nothing is sent anywhere or shared between devices.
- Clearing that browser's site data, or switching to a new phone, wipes everything. **Download the CSV report regularly** (Reports tab) as a backup.
- If a PIN is set and forgotten, the only recovery is Settings → Erase All Data, which wipes everything — pick something the owner/staff will remember.
- The app works fully offline after the very first successful load. It only needs internet again when you deploy an update.