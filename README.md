# Flutter CI/CD Template for Android & Windows

This project includes a complete CI/CD pipeline using GitHub Actions to:

✅ Build and sign APK for Android  
✅ Build EXE for Windows  
✅ Distribute APK via Firebase App Distribution  
✅ Publish builds to GitHub Releases

---

## 🔧 Requirements

- Flutter 3.19.0 or higher
- Firebase Project with App ID
- Generated Android keystore (JKS)
- GitHub Secrets configured

---

## 📁 Requirements GitHub Secrets to Add

| Name                     | Description                          |
|--------------------------|--------------------------------------|
| ANDROID_KEYSTORE_BASE64 | Base64 content of keystore           |
| ANDROID_KEYSTORE_PASSWORD | Keystore password                  |
| ANDROID_KEY_ALIAS       | Alias name (e.g., upload)            |
| ANDROID_KEY_PASSWORD    | Key password                         |
| FIREBASE_APP_ID         | App ID from Firebase Console         |
| FIREBASE_SERVICE_ACCOUNT| Raw JSON of Firebase service account |

---


## 🛠️ How to use CI/CD
1. Fork this repo.
2. Replace app ID and credentials.
3. Push to `master` to trigger build.
---

## 📂 Outputs

- `app-release.apk` → GitHub Releases + Firebase testers
- `app-release.exe` → GitHub Releases




