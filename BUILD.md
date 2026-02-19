# Build guide

## Local (Android)
```bash
npm install
cd android
./gradlew clean
./gradlew assembleDebug
./gradlew assembleRelease
```

## GitHub Actions
A workflow is included at `.github/workflows/android.yml` and will build:
- app-debug.apk
- app-release-unsigned.apk

To produce a signed release, add a keystore and signing config (recommended in CI secrets).
