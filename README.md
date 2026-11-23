
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>SALEEM WIFI TOOLKIT</title>
<style>
body {
  background: #10131c;
  color: #fff;
  font-family: Arial, sans-serif;
  padding: 20px;
}
h1 { color: #00e5ff; text-align: center; }
.step {
  background: #1c2230;
  padding: 15px;
  margin: 15px 0;
  border-radius: 12px;
}
.command {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 10px;
  background: #080b11;
  padding: 12px;
  border-radius: 8px;
}
code {
  overflow-wrap: anywhere;
  color: #80ffb0;
}
button {
  background: #00a8cc;
  color: white;
  border: 0;
  border-radius: 6px;
  padding: 9px 12px;
  cursor: pointer;
  flex-shrink: 0;
}
p { color: #c5cbd5; }
</style>
</head>
<body>

<h1>亗 SALEEM WIFI TOOLKIT 亗</h1>
<p style="text-align:center">Wi-Fi Security Commands — Kali Linux</p>
<p>Use only on your own network or an authorized lab.</p>

<div class="step">
<h3>STEP 1 — Check Wireless Interface</h3>
<div class="command">
<code>iwconfig</code>
<button onclick="copyCommand(this)">COPY</button>
</div>
<p>Wireless interface ki information check karta hai.</p>
</div>

<div class="step">
<h3>STEP 2 — Start Monitor Mode</h3>
<div class="command">
<code>sudo airmon-ng start wlan0</code>
<button onclick="copyCommand(this)">COPY</button>
</div>
<p>Wireless adapter par monitor mode start karta hai.</p>
</div>

<div class="step">
<h3>STEP 3 — View Wireless Networks</h3>
<div class="command">
<code>airodump-ng wlan0mon</code>
<button onclick="copyCommand(this)">COPY</button>
</div>
<p>Wireless network information observe karta hai.</p>
</div>

<div class="step">
<h3>STOP PROCESS</h3>
<div class="command">
<code>Ctrl + C</code>
<button onclick="copyCommand(this)">COPY</button>
</div>
<p>Running process ko stop karta hai.</p>
</div>

<div class="step">
<h3>STEP 4 — Packet Capture</h3>
<p>Authorized wireless lab mein packet capture ke concept ka educational overview.</p>
</div>

<div class="step">
<h3>STEP 5 — Wordlist Directory</h3>
<div class="command">
<code>cd /user/share/wordlists</code>
<button onclick="copyCommand(this)">COPY</button>
</div>
<p>Wordlist directory mein jane ka command.</p>
</div>

<div class="step">
<h3>STEP 6 — Extract Compressed Wordlist</h3>
<div class="command">
<code>sudo gzip -d rockyou.txt.gz</code>
<button onclick="copyCommand(this)">COPY</button>
</div>
<p>Compressed wordlist extract karta hai.</p>
</div>

<div class="step">
<h3>STEP 7 — Password Audit</h3>
<p>Wi-Fi password auditing ke liye authorized lab ka educational concept.</p>
</div>

<script>
function copyCommand(button) {
  const command = button.parentElement.querySelector("code").innerText;
  navigator.clipboard.writeText(command).then(() => {
    button.innerText = "COPIED!";
    setTimeout(() => button.innerText = "COPY", 1500);
  }).catch(() => {
    button.innerText = "COPY FAILED";
  });
}
</script>

</body>
</html>
