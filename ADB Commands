# 📱 Android Debug Bridge (ADB) Command Reference

A practical collection of commonly used ADB commands for connecting Android devices, transferring files, launching applications, capturing screenshots, viewing logs, and more.

---

## 🔗 Connect Your Android Device

### View Connected Devices
```bash
adb devices
```

### Open Device Shell
```bash
adb shell
```

### Display Device Wi-Fi IP Address
```bash
adb shell ip addr show wlan0
```

### Enable Wireless Debugging
```bash
adb tcpip 5555
```

### Connect Over Wi-Fi
Replace `<DEVICE_IP>` with your Android device's IP address.

```bash
adb connect <DEVICE_IP>:5555
```

---

# 📂 File Management

### Upload a File to Android
```bash
adb push <local_file> <device_destination>
```

**Example**
```bash
adb push image.jpg /sdcard/Pictures/
```

### Download a File from Android
```bash
adb pull <device_file> <local_destination>
```

**Example**
```bash
adb pull /sdcard/Download/example_file.txt ~/Desktop/
```

---

# 🚀 Launch Android Applications

Use the following commands to start common Android applications directly from your computer.

| Application | Command |
|-------------|---------|
| 📷 Camera | `adb shell am start -a android.media.action.IMAGE_CAPTURE` |
| ▶️ YouTube | `adb shell am start -a android.intent.action.VIEW -d https://www.youtube.com` |
| 💬 WhatsApp | `adb shell am start -n com.whatsapp/.HomeActivity` |
| 🌐 Web Browser | `adb shell am start -a android.intent.action.VIEW -d http://www.google.com` |
| 📍 Google Maps | `adb shell am start -a android.intent.action.VIEW -d "geo:0,0?q=1600+Amphitheatre+Parkway,+Mountain+View,+California"` |
| 🛒 Play Store | `adb shell am start -a android.intent.action.VIEW -d "market://details?id=com.example.package"` |
| 📘 Facebook | `adb shell am start -n com.facebook.katana/.LoginActivity` |
| 📸 Instagram | `adb shell am start -n com.instagram.android/.activity.MainTabActivity` |
| ❌ X (Twitter) | `adb shell am start -n com.twitter.android/.StartActivity` |
| 🎵 Spotify | `adb shell am start -n com.spotify.music/.MainActivity` |
| 📧 Gmail | `adb shell am start -n com.google.android.gm/.ConversationListActivityGmail` |
| ⚙️ Settings | `adb shell am start -a android.settings.SETTINGS` |
| ☎️ Dialer | `adb shell am start -a android.intent.action.DIAL` |
| 💬 SMS | `adb shell am start -a android.intent.action.VIEW -d sms:` |
| 👥 Contacts | `adb shell am start -a android.intent.action.VIEW -d content://contacts/people/` |
| 🧮 Calculator | `adb shell am start -n com.android.calculator2/.Calculator` |
| 📅 Calendar | `adb shell am start -n com.google.android.calendar/.LaunchActivity` |
| 🎶 YouTube Music | `adb shell am start -n com.google.android.apps.youtube.music/.activities.MainActivity` |

---

# 📸 Capture Screenshots

### Take a Screenshot
```bash
adb shell screencap /sdcard/screenshot.png
```

### Copy Screenshot to Computer
```bash
adb pull /sdcard/screenshot.png ./screenshot.png
```

### Remove Screenshot from Device (Optional)
```bash
adb shell rm /sdcard/screenshot.png
```

---

# 📜 Android Logcat

### View Live Logs
```bash
adb logcat
```

### Save Logs to a File
```bash
adb logcat -d > logs.txt
```

### Display Only Error Logs
```bash
adb logcat *:E
```

### Filter Logs for a Specific Application
```bash
adb logcat | grep com.example.myapp
```

---

# 📞 Export Call History *(Root Required)*

The following command copies the device's call log database.

```bash
adb pull /data/data/com.android.providers.contacts/databases/calllog.db ./calllog.db
```

> **Note:** Root privileges are required to access this database.

---

# ❌ Disconnect ADB

### Disconnect a Specific Device
```bash
adb disconnect <DEVICE_IP>:5555
```

### Disconnect All Connected Devices
```bash
adb disconnect
```

---

# 💡 Tips

- Enable **Developer Options** on your Android device.
- Turn on **USB Debugging** before connecting.
- Use a trusted USB cable for stable communication.
- Wireless debugging requires both devices to be on the same network.
- Some commands depend on Android version or device manufacturer.

---

## 📖 Quick Command Summary

| Task | Command |
|------|---------|
| Detect devices | `adb devices` |
| Open shell | `adb shell` |
| Connect over Wi-Fi | `adb connect <IP>:5555` |
| Upload file | `adb push` |
| Download file | `adb pull` |
| Launch application | `adb shell am start ...` |
| Take screenshot | `adb shell screencap` |
| View logs | `adb logcat` |
| Disconnect device | `adb disconnect` |

---

⭐ If you found this guide useful, consider giving the repository a **Star**.
