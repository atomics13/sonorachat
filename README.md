# sonorachat-project

# Sonora.Chat Android App

A Trusted Web Activity (TWA) Android application wrapping the Sonora.Chat web app.

Check in: https://sonora.chat 
Install App: https://sonora.chat/installsonora.php

## 📱 About

This project wraps the SonoraChat web application as an Android app using **Bubblewrap**, Google's tool for building Trusted Web Activities. It provides a native Android experience for the web-based chat platform.

## 🛠️ Prerequisites

- Node.js (v14 or later)
- Java Development Kit (JDK) 11 or later
- Android SDK
- Bubblewrap CLI

## 📦 Installation

### Install Bubblewrap globally

```bash
npm install -g @bubblewrap/cli

### Clone the repository
git clone https://github.com/atomics13/sonorachat.git
cd sonorachat

Common Commands

### Update TWA manifest
nano twa-manifest.json

### Build the Android project
bubblewrap update & bubblewrap build
 
### Generate Debug APK
./gradlew assembleDebug

### Generate Release APK (signed)
./gradlew assembleRelease

⚠️ Important Notes

    Never commit android.keystore to version control

    Never commit .apk or .aab files to version control

    Keep your signing keys secure and backed up

    Test the app thoroughly after each bubblewrap update

🐛 Troubleshooting

Digital Asset Links error

Ensure your web domain has the proper assetlinks.json file at /.well-known/assetlinks.json
Build fails
bash

./gradlew clean
./gradlew assembleRelease --stacktrace

Update Bubblewrap to latest version
bash

npm update -g @bubblewrap/cli

📚 Resources

    Bubblewrap Documentation

    Trusted Web Activity Guide

    Digital Asset Links

📄 License

MIT License

