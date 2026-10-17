# WinDroid KeyMaster ⌨️ -> 📱

Ultra-lightweight Android background accessibility service to bring **all standard Windows physical keyboard shortcuts** to your Android tablet!

### Why this exists:
When connecting a physical or Bluetooth keyboard to an Android tablet (Samsung Galaxy Tab, Xiaomi Pad, Lenovo Tab, Pixel Tablet), users constantly press `Win+D`, `Alt+Tab`, `Alt+F4`, `Win+E`, `Win+L`, `Win+Shift+S`.

This project implements a native, zero-bloat Android Accessibility Service that runs completely in the background, consuming **0% CPU** and **<50KB APK size**.

---

### Shortcuts Supported:
| Windows Shortcut | Android Tablet Action |
|---|---|
| **Win + D** or **Win + M** | Show Desktop / Home |
| **Alt + Tab** | App Switcher (Recents carousel) |
| **Alt + F4** | Back / Close Active Window |
| **Win + E** | File Explorer / Files App |
| **Win + L** | Lock Screen & Display Off |
| **Win + Shift + S** / **PrintScreen** | Take Screenshot |
| **Win + A** | Action Center / Quick Settings |
| **Win + N** | Notification Shade |
| **Win + I** | Android Settings |
| **Win + B** | Launch Default Web Browser |
| **Win + Left / Right** | Toggle Split Screen |
| **Ctrl + Shift + Esc** | Task Manager / Recents |

---

### Easy Build Options:

#### Option 1: Zero-Setup Cloud Build (GitHub Actions) - 1 Minute!
1. Create a free new private or public GitHub repo.
2. Push or upload these project files.
3. Click the **Actions** tab in GitHub -> Click **"Build WinDroid APK"** -> **"Run workflow"**.
4. Within 45 seconds, download your compiled `app-debug.apk` from the artifact box!

#### Option 2: Android Studio (Computer)
1. Open Android Studio -> **Open Folder** -> Select this project folder.
2. Click **Build** -> **Build Bundle(s) / APK(s)** -> **Build APK(s)**.
3. Copy `app-debug.apk` to your tablet and install!

#### Option 3: Build directly on your Android Tablet using Termux!
```bash
pkg update && pkg install -y openjdk-17 git
chmod +x ./gradlew
./gradlew assembleDebug
# APK will be in: app/build/outputs/apk/debug/app-debug.apk
```

---

### Activation on Tablet:
1. Install the APK on your Android tablet.
2. Open **WinDroid KeyMaster**.
3. Tap **"1. Open Accessibility Settings"** and switch **WinDroid KeyMaster** to **ON**.
4. Connect your physical keyboard and enjoy seamless Windows shortcuts!
