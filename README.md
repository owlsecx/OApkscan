# 📱 OApkscan

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux%20%2F%20Windows-informational?style=flat-square&logo=linux&logoColor=white&color=0a0c10"/>
  <img src="https://img.shields.io/badge/Category-OStatic%20Analysis%20%2F%20Mobile%20Security-cyan?style=flat-square"/>
  <img src="https://img.shields.io/badge/Dependencies-None%20(Standalone)-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-Proprietary-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-v1.0-cyan?style=flat-square"/>
</p>

> **OApkscan** is a powerful static analysis engine for Android APK / AAB / XAPK and iOS IPA files. It extracts permissions, detects hardcoded secrets, malware signatures, obfuscation, suspicious libraries, and ad/tracking SDKs — without running the app.

---

## 📌 Overview

OApkscan performs deep static analysis on mobile application packages. It identifies dangerous permission combinations, stalkerware indicators, hardcoded credentials, embedded URLs/IPs, suspicious native libraries, and many other red flags. It works offline and requires no emulator or root.

**Supports**: `.apk`, `.xapk`, `.aab`, `.ipa`

---

## 🖥️ Modules

| # | Module                  | Description |
|---|-------------------------|-------------|
| **[1]** | **Scan APK / IPA**          | Full static analysis of a single app file |
| **[2]** | **Batch Scan**              | Analyze all APK/IPA files in a directory |
| **[3]** | **Permission Reference**    | Browse all tracked dangerous permissions |
| **[4]** | **Secret Patterns**         | View all detected secret/key patterns |

---

## 📊 Key Features

- **Risk Scoring** (0-100) with clear verdicts (CLEAN → MALICIOUS)
- **30+ Dangerous Permissions** with stalkerware combo detection
- **Secret Extraction** — API keys, tokens, private keys, passwords
- **Malware Signature Database** — known stalkerware & RAT packages
- **Obfuscation Detection** — ProGuard, short class names, low strings
- **Native Library Analysis** — Frida, Xposed, Riru, root libs, etc.
- **Ad/Tracking SDK Detection** — 18+ known SDKs (AdMob, AppsFlyer, etc.)
- **Certificate Analysis** — Debug cert, self-signed, anomalies
- **Embedded URLs & IPs** — Hardcoded C2 infrastructure
- **Privacy & Entitlements** (for IPA) — TCC bypass, sandbox disable, etc.

---

## ⚙️ Requirements

- **Linux or Windows**
- **No additional dependencies** — pure Python (optional: androguard, cryptography for extra features)

---

## 🚀 Usage

```bash
./OApkscan

📁 Output

Rich Terminal Report — Risk score, verdict, colored findings, detailed breakdown
JSON Export — Full structured analysis (findings, secrets, permissions, etc.)
Session History — All analyzed apps kept in memory during the session


📦 Part of OwlSec Toolkit
This tool is part of the OwlSec suite — a collection of 300+ security and privacy tools.
🔗 owlsec.org

©️ License
Proprietary — © Khaled S. Haddad
Tools are distributed as pre-built executables. Source code is proprietary.

AUTHORISED MOBILE APPLICATION SECURITY ANALYSIS USE ONLY
