# HabitFlow APK (Capacitor)

## Easiest: build the APK free on GitHub (no installs)
1. Create a new GitHub repo and upload ALL files in this folder (including the hidden `.github` folder).
2. Open the repo's **Actions** tab -> "Build APK" runs automatically (2-4 min).
3. Open the finished run -> **Artifacts** -> download `HabitFlow-apk` (zip) -> extract `app-debug.apk`.
4. Send it to your Android phone, tap it, allow "Install unknown apps" when asked.

## Or build locally
Install Node 20+, JDK 17 and Android Studio (for the SDK), then:
    npm install
    npx cap add android
    npx cap sync android
    cd android && ./gradlew assembleDebug
APK: android/app/build/outputs/apk/debug/app-debug.apk

The app is fully offline (Tailwind, icons, confetti and the Inter font are bundled in www/vendor).
