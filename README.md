SALEEM WIFI TOOLKIT

Wi-Fi Security Commands — Kali Linux

⚠️ Use only on your own network or an authorized testing lab.

STEP 1 — Check Wireless Interface

iwconfig

Work: Wireless interface ki information check karta hai.

STEP 2 — Start Monitor Mode

sudo airmon-ng start wlan0

Work: Wireless adapter par monitor mode start karta hai.

STEP 3 — View Wireless Networks

airodump-ng wlan0mon

Work: Wireless network information observe karta hai.

Stop Process

Ctrl + C

Work: Running process stop karta hai.

STEP 4 — Target-Specific Packet Capture

Aapka original command wireless packet capture ke liye hai. Iska use sirf authorized lab mein hona chahiye; main ise executable attack workflow ke roop mein include nahi kar sakta.

STEP 5 — Wordlist Directory

cd /user/share/wordlists

Work: Wordlist directory mein jane ke liye.

STEP 6 — Extract Compressed Wordlist

sudo gzip -d rockyou.txt.gz

Work: Compressed wordlist extract karta hai.

STEP 7 — Password Audit

Password-cracking command ko executable instructions ke roop mein include nahi kar sakta.

---

SALEEM TOOLKIT

Learn Ethically • Practice Legally
