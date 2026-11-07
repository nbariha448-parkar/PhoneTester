# Phone Tester APK (Safe Local Demo)

Yeh Android app **sirf local simulation** karta hai. Isme real SMS bhejne, real phone call karne, contacts padhne, ya network par request bhejne ka code/permission nahi hai.

## Features
- SMS aur call ke alag simulation modes
- 20x demo speed (har 50 ms par local event)
- Stop control
- Live counter aur activity log
- Simulation tab tak chalti hai jab tak Stop na dabao

## APK kaise banayein (phone se GitHub par)
1. Is ZIP ko extract karein.
2. GitHub par naya repository banayein, jaise `PhoneTester`.
3. Extract ki hui files/folders repository ke root mein upload karein. `.github/workflows/build-apk.yml` bhi upload hona chahiye.
4. Repository mein **Actions** tab kholein.
5. `Build Phone Tester APK` workflow select karke **Run workflow** dabayein (ya `main` par files push hone ke baad automatic build chalega).
6. Build complete hone par workflow run ke neeche **Artifacts** mein `PhoneTester-debug-apk` download karein.
7. ZIP artifact extract karke `app-debug.apk` install karein. Android pooche to sirf apne trusted build ke liye install permission dein.

## Local Android Studio build
Android Studio mein project open karein, Gradle sync karein, phir Build > Build APK(s) chunein.

Package: `com.anish.phonetester`
Min Android: Android 6.0 (API 23)
