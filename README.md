# MONITOR MODE for Samsung Galaxy A03 Core (SM-A032F S9 Binary)

## Overview

This project provides precompiled kernel modules that enable Wi-Fi monitor mode support on the Samsung Galaxy A03 Core (SM-A032F, S9 binary base).

This setup was tested on my own device using a **MT7601U USB Wi-Fi adapter**.

---

## ⚠️ Important Warnings

* This is **experimental**
* Incorrect module versions (vermagic mismatch) may cause loading failure
* Bootloader must be unlocked
* Root access is required
* Kernel mismatch may lead to instability or reboot issues

Proceed only if you understand kernel module handling and recovery methods.

---

## 📦 Included Modules

* cfg80211.ko
* mac80211.ko
* mt7601u.ko

Additional adapters may require recompilation using Samsung Open Source kernel sources (S8 binary base may also be compatible depending on vermagic match).

---

## 🧪 Installation (Root Required)

Run in a root shell (Termux or ADB):

```sh
su
insmod /sdcard/Download/cfg80211.ko
insmod /sdcard/Download/mac80211.ko
insmod /sdcard/Download/mt7601u.ko
```

Adjust paths depending on your file location.

---

## 🔧 Notes for Developers

* Ensure module vermagic matches your running kernel exactly
* If using other Wi-Fi adapters, compile modules against matching Samsung kernel source
* S8 binary sources may be used in some cases, but compatibility is not guaranteed

---

## 📌 Status

* Experimental build
* Successfully tested on SM-A032F (S9 binary)
* Monitor mode support achieved via MT7601U adapter







<meta name="google-site-verification" content="UgRoZlu2K4hkawSEUIRvL9rbMSmgradulZBW3oWGJYY" />
