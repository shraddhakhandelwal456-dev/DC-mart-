# DC Mart – Android project (app is bundled inside)

The whole DC Mart web app is in app/src/main/assets/index.html. MainActivity.java shows it in a WebView and
makes the photo "Choose photos" buttons open the phone's file picker.

## Build a test app (APK) – about 10 minutes
1. Install Android Studio (free): developer.android.com/studio
2. File > Open > choose this DCMart-Android folder. Wait for "Gradle sync" to finish.
   If Studio offers to upgrade the Android Gradle Plugin or Gradle, accept.
3. Plug in an Android phone with USB debugging on (or start an emulator) and press the green Run button.
   Or: Build > Build Bundle(s) / APK(s) > Build APK(s), then copy the .apk to your phone and install it.

## Build the file for Google Play (AAB)
1. Change applicationId in app/build.gradle to your own ID, for example in.yourstore.dcmart.
2. Build > Generate Signed App Bundle / APK > Android App Bundle > Create new keystore.
   KEEP the keystore file and passwords safe and backed up. Lose them and you cannot update the app.
3. Choose "release" and finish. Upload app/release/app-release.aab in Play Console.
4. Use play-store-icon-512.png as the Play Store icon.

## Important
This is the DEMO app: data stays on each phone, the OTP is shown on screen, and there are no real payments.
It is fine for testing and showing people, but not for real customers until a server is added.
