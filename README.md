# SimpleChat - minimal Android app

This is a minimal Android project that displays a simple chat-like UI.
It includes a GitHub Actions workflow (.github/workflows/android-build.yml) that will build a debug APK
when you push the full project to your GitHub repository's main branch.

## How to use
1. Create a new GitHub repository (public or private).
2. Upload all files and folders from this project into the repository root.
3. Push to GitHub (or upload via web UI). The workflow triggers on push to main/master.
4. After workflow runs (Actions tab), download the artifact named `app-debug-apk`.

## Notes
- No Firebase or external services required.
- If the build fails due to Gradle plugin versions, edit build.gradle files in the repo to match tools on the runner.
