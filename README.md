# Penny Counter — Capacitor Android App

This is the Penny Counter web app packaged as a Capacitor project. Capacitor lets an existing HTML/CSS/JavaScript app run inside a native Android application.

## Easiest way to build without Android Studio: GitHub Actions

1. Create a new GitHub repository.
2. Upload every file in this folder to the repository.
3. Open the repository's **Actions** tab.
4. Select **Build Penny Counter APK**.
5. Run the workflow.
6. When it finishes, open the workflow run and download the `penny-counter-debug-apk` artifact.
7. Unzip that artifact. The APK inside can be installed on an Android phone.

The workflow generates the Android project with Capacitor and builds the debug APK on GitHub's servers, so Android Studio is not required on your computer.

## Local build (optional)

If you later install Node.js and the Android SDK/Gradle tooling, you can run:

```bash
npm install
npx cap add android
npx cap sync android
cd android
./gradlew assembleDebug
```

The APK will be under `android/app/build/outputs/apk/debug/`.

## App details

- App name: Penny Counter
- Package ID: `com.pennycounter.app`
- Maximum pennies: 3
- Starting count: 3
