NutriTrack Android project (source)

This project wraps the NutriTrack nutrition tracker in an Android WebView. Food logs/settings use browser local storage on the phone. Meal photos can be selected through Android's file picker.

How to build an APK:
1. Install Android Studio on a computer.
2. Extract this project ZIP.
3. In Android Studio choose Open and select the NutriTrackAndroid folder.
4. Allow Android Studio to sync/download the Android Gradle Plugin and SDK platform 35.
5. Select Build > Build Bundle(s) / APK(s) > Build APK(s).
6. Android Studio will show the APK location, usually app/build/outputs/apk/debug/app-debug.apk.
7. Transfer that APK to your Android phone and install it. Android may ask you to allow installs from that file manager.

Important limitations:
- This environment cannot run Android SDK/Gradle, so it cannot honestly provide a compiled, tested APK binary directly.
- This is a local/offline wrapper; AI meal photo recognition is not implemented. Uploaded photos are journal attachments only.
- Nutrition values are estimates, not medical advice.
- Keep the APK private unless you review app security, privacy, data backup, and release signing.
