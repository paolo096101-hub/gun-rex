# Gun Rex

A pixel-art runner: jump, duck and shoot through 6 worlds with natural disasters and 6 bosses.
Plays in any browser and installs on Android as an app (PWA), fullscreen and offline.

## Put it on GitHub and play it

1. Create a new repository on GitHub (public).
2. Upload everything in this folder to it (drag the files into the web page, **including the hidden `.github` folder and `.nojekyll`**), then commit.
3. Go to **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**, branch **main**, folder **/(root)**, then Save.
4. After a minute your game is live at `https://YOUR-USERNAME.github.io/YOUR-REPO/`.

## Install on Android

1. Open the link above in **Chrome** on your phone.
2. Tap the menu (⋮) → **Install app** (or **Add to Home screen**).
3. Open **Gun Rex** from your home screen: it runs fullscreen in landscape and works offline.

## Optional: build a real APK

1. In your repo open the **Actions** tab → **Build Android APK** → **Run workflow**.
2. When it finishes (about 5 to 10 minutes), open the run and download the **gun-rex-apk** artifact (a zip containing `app-debug.apk`).
3. Copy the APK to your phone and open it. Android will ask you to allow installing from this source.

This is a debug APK for sideloading and testing. To publish on Google Play you need a signed release build.

## Updating the game

Replace `index.html`, then change `VERSION` in `sw.js` (for example `gun-rex-v2`) so players receive the new version.

## Files

| File | What it is |
| --- | --- |
| `index.html` | The whole game |
| `manifest.json` | Makes it installable (name, icons, fullscreen, landscape) |
| `sw.js` | Offline support |
| `icon-*.png` | App icons |
| `.github/workflows/apk.yml` | Builds the Android APK |
