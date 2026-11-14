# CCTV Expert Android App — Build Instructions

This is a native Android WebView app wrapper around the offline CCTV Expert billing system.

## Included features
- Offline storage using Android WebView local storage
- Invoice numbering
- Bill History: view/open/edit/delete saved bills
- Item rows, discount, paid amount, balance calculation
- WhatsApp bill sharing
- Android Print Framework for Save as PDF / printing

## Build an installable APK using GitHub Actions (Chrome + GitHub account required)

1. Extract this ZIP on your phone or computer.
2. Open https://github.com in Chrome and sign in.
3. Create a new **public or private** repository, for example `cctv-expert-android`.
4. Upload the *contents* of this extracted folder to the repository. Make sure `.github/workflows/android-apk.yml` is included.
5. Open the repository's **Actions** tab. If prompted, allow GitHub Actions.
6. Wait for the workflow named **Build CCTV Expert APK** to finish successfully.
7. Open that completed workflow run, scroll to **Artifacts**, and download `CCTVExpert-debug-apk`.
8. Extract the downloaded artifact ZIP and tap `app-debug.apk` to install it. Android may ask you to allow installation from Chrome or Files.

## Notes
- This project ZIP is source code, not an APK.
- The GitHub Actions workflow compiles the debug APK. It is suitable for installing/testing on your own Android phone; it is not a Play Store release-signed APK.
- Saved bills remain on the same app installation/device. Clearing app data or uninstalling the app can erase local bills. Export/backup is not yet included.
- PDF: tap **Save / Print as PDF** in the app, choose **Save as PDF** in Android's print screen, then select a folder.
- For privacy, do not upload customer data; only upload the source-code project.
