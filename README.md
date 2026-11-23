
# 亗 SALEEM WIFI TOOLKIT 亗

**Wi-Fi Security Commands — Kali Linux**

> ⚠️ Use these commands only on your own network or an authorized testing lab.

## STEP 01 — Check Wireless Interface

```bash
iwconfig
```

**Work:** Wireless interface ki information check karta hai.

## STEP 02 — Start Monitor Mode

```bash
sudo airmon-ng start wlan0
```

**Work:** Wireless adapter par monitor mode start karta hai.

## STEP 03 — View Wireless Networks

```bash
airodump-ng wlan0mon
```

**Work:** Wireless network information observe karta hai.

### Stop Process

```text
Ctrl + C
```

**Work:** Running process ko stop karta hai.

## STEP 04 — Target-Specific Packet Capture

**Original command:** Aapke diye hue command ka operational capture workflow yahan include nahi kiya gaya hai.

**Work:** Authorized wireless lab mein packet-capture concepts samjhata hai.

## STEP 05 — Wordlist Directory

```bash
cd /user/share/wordlists
```

**Work:** Wordlist directory mein jane ke liye.

## STEP 06 — Extract Compressed Wordlist

```bash
sudo gzip -d rockyou.txt.gz
```

**Work:** Compressed wordlist extract karta hai.

## STEP 07 — Password Audit

**Work:** Authorized lab mein Wi-Fi password auditing ke concepts samjhata hai.

---

## PROJECT INFORMATION

- **Project:** SALEEM WIFI TOOLKIT
- **Platform:** Kali Linux
- **Category:** Wi-Fi Security
- **License:** MIT

**亗 LEARN ETHICALLY • PRACTICE LEGALLY 亗**
