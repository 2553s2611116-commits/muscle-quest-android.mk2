# MUSCLE QUEST Android (offline)

Offline-first personal Android app built as a WebView shell around local HTML/JSON assets. No internet permission, login, backend, or ad SDK is included. Exercise library data is bundled in `app/src/main/assets/data.json`; app UI is `index.html`.

## Build APK without installing Android Studio locally
1. Create a GitHub repository and upload the contents of this folder to its root.
2. Commit/push to `main` (or `master`). GitHub Actions runs `.github/workflows/build-apk.yml`.
3. In the repository, open **Actions → Build MUSCLE QUEST APK → latest successful run**.
4. Download artifact `muscle-quest-debug-apk` and unzip it to get `app-debug.apk`.
5. Transfer the APK to Android and open it. If prompted, allow installing apps from that source.

You can also use **Actions → Run workflow** to build manually. This workflow produces a debug APK for personal testing, not a signed Play Store release.

## Notes
- App content works offline. `localStorage` stores favorites, routines, and completed routine history on the device.
- Backup screen creates JSON text to copy and restore by pasting JSON back in. Keep an external copy before uninstalling or changing phones.
- Muscle map and movement art are schematic educational illustrations, not medically precise anatomical maps or video demonstrations.
- Exercise instructions are general educational information. Adjust loads and stop if pain occurs.
