# Gaming Hub (Android)

A lightweight dark/neon game-discovery app for Android. It includes a searchable library, category filters, quick picks, a download center, and links that open official store/search pages in the browser.

## Build an APK using GitHub Actions (phone-friendly)

1. Create a **public or private** GitHub repository named `GamingHub`.
2. Upload all files and folders from this project, preserving their paths. Make sure `.github/workflows/build-apk.yml` is included.
3. Commit the files to the `main` branch.
4. Open the repository's **Actions** tab. Select **Build Gaming Hub APK** and tap **Run workflow** if it hasn't started automatically.
5. Wait for the workflow to finish with a green check.
6. Open that workflow run, scroll to **Artifacts**, and download `GamingHub-debug-apk`.
7. Extract the ZIP artifact and install `app-debug.apk` on your Android device. Android may ask you to allow installation from the app/browser you used to download it.

## Important notes

- The included APK is a **debug build** suitable for testing, not a signed release for Play Store publishing.
- Game buttons open official Google Play search pages; the app does not host game APKs.
- No game publisher affiliation is implied.
- The project needs internet access to open external game pages.
- Application ID: `com.gaminghub.app`.
- Minimum Android version: Android 6.0 (API 23).

## Project structure

- `app/src/main/java/.../MainActivity.kt` — Android WebView shell
- `app/src/main/assets/index.html` — app UI and library
- `app/src/main/AndroidManifest.xml` — app configuration
- `.github/workflows/build-apk.yml` — cloud APK build workflow
