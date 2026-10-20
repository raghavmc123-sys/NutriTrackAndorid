# Build NutriTrack APK using only your Android phone

This project ZIP is prepared for a cloud build. It does **not** already contain a compiled APK.

## Steps

1. Download and extract `NutriTrack_Cloud_Build_Package.zip` on your Android phone.
2. Open GitHub in your browser and sign in (create an account if needed).
3. Create a **new repository** named `NutriTrackAndroid`. For the easiest setup, make it **Public** so GitHub Actions is available without extra configuration. Do not add a README, license, or `.gitignore` during repository creation.
4. In the new empty repository, use **Add file → Upload files**. Upload the *contents* of the extracted `NutriTrackAndroid` folder, including the hidden `.github` folder and its `workflows/build-apk.yml` file. If your phone's file picker hides dot-folders or makes folders difficult to upload, use GitHub's mobile browser in desktop mode, or a GitHub-compatible mobile app that can upload folders. The `.github/workflows/build-apk.yml` file is required for the automated build.
5. Commit the uploaded files to the `main` branch.
6. Open the repository's **Actions** tab. Choose **Build NutriTrack APK**. If it has not started automatically, tap **Run workflow → Run workflow**.
7. Wait for the workflow to finish with a green check mark. Open that successful run, scroll to **Artifacts**, and download **NutriTrack-debug-APK**.
8. Extract the downloaded artifact ZIP. Tap `app-debug.apk` and install it. If Android asks, allow your browser or file manager to **install unknown apps** for this installation, then retry.

## If the build fails

Open the failed run in Actions and read the first red error step. The build log can be copied here and I can help troubleshoot it.

## Notes

- This produces a **debug APK** for personal testing, not a Play Store release.
- GitHub may show slightly different mobile menus. Uploading folders including the hidden `.github` directory can be awkward on a phone.
- Only upload this project to an account/repository you control.
