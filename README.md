# 🦉 OApkscan

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-OForensics-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-2.0-cyan?style=flat-square"/>
</p>

> **OApkscan** — APK/IPA forensics — permissions, secrets, malware, certs, entropy

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

OApkscan is a static analysis engine for Android (APK/AAB) and iOS (IPA) application packages. It inspects permissions, secrets, certificates, intents, deep links and network-security configuration, and applies malware, stalkerware and obfuscation heuristics to score each app. It runs on a single file or batches an entire directory in parallel, and can optionally enrich results with a VirusTotal hash lookup.

---

## ✨ Features

- Static analysis of APK, AAB and IPA packages (no execution)
- Permission, secret, certificate, intent and deep-link extraction
- Entropy, obfuscation, packer and C2/stalkerware/trojan heuristics
- Batch scanning of a directory with configurable threads and min-score filter
- Optional VirusTotal hash lookup via VT_API_KEY
- Export reports to JSON, TXT, HTML or CSV

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OApkscan -f app.apk
./OApkscan -d ./apps/ --threads 8 --min-score 50
./OApkscan -f app.ipa --format html -o report.html
./OApkscan --help
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
