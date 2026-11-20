# Practice 4 — Android Debug APK with GitHub Actions

Minimal Hello World Android app. The GitHub Actions workflow in
`.github/workflows/android-debug.yml` builds a debug APK on every push to
`main` and uploads it as the `app-debug` artifact.

No local Android SDK, JDK, or Gradle installation is required: the runner
provides JDK 17 and the Android SDK, and the Gradle wrapper pins the Gradle
version.

- Build command: `./gradlew assembleDebug`
- Output APK: `app/build/outputs/apk/debug/app-debug.apk`
