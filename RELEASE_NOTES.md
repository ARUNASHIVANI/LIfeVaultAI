# LifeVault AI v5.2.5 — Production Release (Android APK)

> **Tag:** `v5.2.5`  
> **Release Target:** `main`  
> **Package:** `com.theoriongd.lifevault` (LifeVault AI)  
> **Build:** `5.2.5+1`  
> **Asset:** `LifeVault-v5.2.5-release.apk` / `lifevault-release.apk` (88.6 MB)

---

## 🌟 Overview

We are proud to present **LifeVault AI v5.2.5**, featuring enhanced cross-platform audio recording, emergency medical dispatch with GPS coordinates, local background notifications, dedicated Cyber Face ID biometric scanning, instant Amazon-style auto-lock on app switching, and biometric zero-knowledge authentication.

**LifeVault AI** is a zero-knowledge, privacy-first personal document intelligence vault and multimodal security system built with Flutter and Dart. It combines client-side cryptographic storage with multimodal artificial intelligence (**Google Gemini 3.7 Flash** and **Hugging Face Whisper**) to provide automated document OCR, conversational retrieval (RAG), expense and warranty tracking, encrypted voice notes, and instant emergency medical access.

---

## 📦 Binary Assets & Checksums

| File | Type | Size | SHA-256 Checksum |
| :--- | :--- | :--- | :--- |
| **`LifeVault-v5.2.5-release.apk`** | Android Standalone Release APK | `~88.6 MB` (`92,907,655 bytes`) | `5CCF4A1F678798C9CB80E64C005FF4FC0EA30C19D64C4B668CC77C496EE689CC` |
| **`lifevault-release.apk`** | Android Standalone Release APK | `~88.6 MB` (`92,907,655 bytes`) | `5CCF4A1F678798C9CB80E64C005FF4FC0EA30C19D64C4B668CC77C496EE689CC` |

### Checksum Verification

**Windows (PowerShell):**
```powershell
Get-FileHash -Path ".\LifeVault-v5.2.5-release.apk" -Algorithm SHA256
# Expected: 5CCF4A1F678798C9CB80E64C005FF4FC0EA30C19D64C4B668CC77C496EE689CC
```

**Linux / macOS:**
```bash
sha256sum LifeVault-v5.2.5-release.apk
# Expected: 5ccf4a1f678798c9cb80e64c005ff4fc0ea30c19d64c4b668cc77c496ee689cc  LifeVault-v5.2.5-release.apk
```

---

## 🚀 Key Fixes & New Features in v5.2.5

### 👤 1. Dedicated Cyber Face ID Recognition Scanner
- **Immersive Face ID Scanner Viewfinder**: Animated 3D-styled face mesh wireframe, rotating radar rings, and animated laser sweep.
- **Android Front-Camera Face Unlock**: Relaxed biometric restrictions so Android's front camera face recognition triggers seamlessly with custom `AndroidAuthMessages`.
- **Instant Fallback**: Quick access to Fingerprint and 4-digit Master PIN at any time.

### 🔒 2. Amazon Mobile App Style Instant Auto-Lock
- **Background Auto-Lock**: Automatically locks the vault the exact moment you leave or switch to another app.
- **Seamless Biometric Resume**: Returning to LifeVault immediately presents the Face ID / Biometrics prompt without requiring extra button taps.
- **Fixed Landing Page Navigation**: Guaranteed navigation into dashboard upon successful biometric or PIN login.

### ⚡ 3. Android Installation & Startup Optimization
- **Zero Package Parse Errors**: Clean build with `compileSdk = 37`, `targetSdk = 34`, and `minSdk = 24` for 100% installation compatibility.
- **Instant Startup**: Asynchronous notification loading and animation completion listeners so the splash screen and app launch instantaneously without hanging.
