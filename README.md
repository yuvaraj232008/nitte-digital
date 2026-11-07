# Nitte Digital – Android app

This folder is a complete Android project. The app shows the Nitte Digital page
(`app/src/main/assets/index.html`) full screen, with camera access for HTS scanning
and Excel files saved to the phone's Downloads folder.

## Option A: build on GitHub (no installs needed)
1. Create a new repository on github.com and upload everything in this folder
   (including the hidden `.github` folder).
2. Open the **Actions** tab. The "Build APK" workflow starts by itself (or click **Run workflow**).
3. When it finishes (about 3–5 minutes), go to the repository's **Releases** (right side of the
   main page) and download **NitteDigital.apk**. On a phone, this downloads the APK directly.

## Option B: build with Android Studio
1. Install Android Studio, then **File → Open** this folder.
2. Wait for the Gradle sync to finish.
3. **Build → Build App Bundle(s) / APK(s) → Build APK(s)**.
4. Click **locate** in the pop-up. The file is `app/build/outputs/apk/debug/app-debug.apk`.

## Install on the phone
Download or copy `NitteDigital.apk` to the phone, tap it, and allow "Install unknown apps" for your
file manager when asked.

## Updating the app
Replace `app/src/main/assets/index.html` with the new version of the page and build again.
Raise `versionCode` in `app/build.gradle` (1 → 2) so the phone installs it as an update.
