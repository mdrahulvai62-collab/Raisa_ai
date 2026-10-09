# RAISA AI — Cloud Build Starter

This starter project can be built in GitHub Actions without installing Android Studio on your PC.

## Important limitations
- This is an early demo APK project, not a finished commercial product.
- The demo license key `RAISA-DEMO-2026` is hard-coded and is NOT secure.
- Do not sell this demo build. Server-backed license validation and a protected admin panel must be implemented before commercial use.
- Voice output uses Android Text-to-Speech; naturalness and Bangla voice availability depend on voices installed on the phone.
- This version does not yet implement speech recognition, always-on hotword, call answering, app installation, payment processing, or offline AI.

## Build online
1. Create/sign in to a GitHub account.
2. Create a new repository named `raisa-ai`.
3. Upload the contents of this ZIP (upload the files inside the folder, not the outer folder).
4. Open the repository's **Actions** tab.
5. If asked, enable Actions.
6. Choose **Build RAISA AI APK** and click **Run workflow**. Alternatively, push to the `main` branch.
7. Wait for the workflow to finish successfully.
8. Open the successful workflow run and download the `RAISA-AI-debug-APK` artifact.
9. Extract the downloaded artifact ZIP to get `app-debug.apk`, then transfer it to your Android phone and install it. You may need to allow installs from that source.

## Next stage
Replace the demo license with server validation (for example Firebase Authentication + a secure backend/Cloud Function or another server-side service), then add an admin dashboard. Never put admin secrets or service credentials inside the APK.
