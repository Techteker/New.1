# Home Workout Pro / FitFlow

A complete mobile-first home workout system built from the supplied fitness-app references. It is a static/PWA web app with a Capacitor Android wrapper.

## Full system
- Onboarding: goal, fitness level and daily workout time
- Personalized home dashboard
- Workout library with 50+ exercises and 5 programs
- Search and category filters
- Exercise detail pages
- Animation / Video-style guided demonstration mode
- Full workout runner with timer, pause/resume, previous, skip and progress
- Workout completion summary
- Calories, minutes, workouts and streak tracking
- Progress chart, weekly goal and achievements
- Profile and editable preferences
- Reminder and dark-theme controls
- LocalStorage persistence for offline use
- Responsive mobile UI
- PWA manifest/service worker
- Capacitor Android wrapper
- GitHub Actions installable debug APK build
- Vercel static deployment configured with `www` as the output directory

## Run on Vercel
Deploy the repository normally. `vercel.json` points Vercel to the `www` directory, so no custom build command is required.

## Android APK
Every push to `main` triggers `.github/workflows/android.yml`. The workflow builds an installable debug APK, uploads it as a GitHub Actions artifact, and copies it to `downloads/Home-Workout-Pro.apk`. `paths-ignore` prevents the APK commit from recursively triggering another build.

## Demonstrations
Exercise demonstrations are original procedural canvas animations designed to work offline. The Video tab is a guided video-style mode; filmed MP4 demonstrations are not bundled because exercise footage requires appropriately licensed media.

## Project
- Web entry: `www/index.html`
- App logic: `www/app.js`
- Styles: `www/styles.css`
- Capacitor config: `capacitor.config.json`

Copyright © 2026 PROXIMAX