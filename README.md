# Al Baqali Android APK Project

This package wraps the Al Baqali HTML app as an Android APK using Capacitor.

## Option A: Build APK locally

Requirements:
- Node.js 20+
- Android Studio
- Java 17+

Commands:

```bash
npm install
npx cap add android
npx cap sync android
npx cap open android
```

In Android Studio:
- Build > Build Bundle(s) / APK(s) > Build APK(s)

APK output is usually:

```text
android/app/build/outputs/apk/debug/app-debug.apk
```

## Option B: Build APK using GitHub Actions

1. Upload all files in this folder to your GitHub repository.
2. Go to the repository on GitHub.
3. Open Actions > Build Android APK > Run workflow.
4. Download the APK from workflow artifacts.

## Update app later

Replace:

```text
public/index.html
```

Then run:

```bash
npx cap sync android
```
