# 🛡️ The Ultimate Privacy & OPSEC Toolkit

![Privacy](https://img.shields.io/badge/Privacy-100%25-4CAF50?style=for-the-badge&logo=shield&logoColor=white)
![Security](https://img.shields.io/badge/Security-Max-D32F2F?style=for-the-badge&logo=hackthebox&logoColor=white)
![OpenSource](https://img.shields.io/badge/Open_Source-True-1976D2?style=for-the-badge&logo=open-source-initiative&logoColor=white)

Welcome to the ultimate guide for reclaiming your digital privacy. This repository breaks down the most secure browsers, essential extensions, and the fundamental rules of OPSEC (Operations Security) you need to survive on the modern web.

> **⚠️ REALITY CHECK:** There is no such thing as "100% secure" or "completely anonymous" on the clear web. If a three-letter agency wants to find you, they will. The goal of this toolkit is to stop mass surveillance, prevent corporate data harvesting (Google, Meta, data brokers), and protect yourself from malicious hackers. 

---

## 🌐 Tier 1: The Browsers

Choosing the right browser is the foundation of your privacy. **Google Chrome is a data-harvesting tool—ditch it.** As of 2026, Chrome's Manifest V3 update has heavily restricted ad-blockers, making Chromium browsers inherently worse for privacy unless heavily modified.

### 🥇 1. LibreWolf (Best Out-of-the-Box Privacy)
![LibreWolf](https://img.shields.io/badge/LibreWolf-0E141A?style=for-the-badge&logo=librewolf&logoColor=white)
* **What it is:** A custom, independent fork of Firefox.
* **Why use it:** It removes all telemetry (tracking) from Mozilla, forces strict tracking protection, pre-installs uBlock Origin, and deletes cookies automatically when closed.
* **Best for:** Daily driving for privacy maximalists.

### 🥈 2. Mozilla Firefox (Best for Customization)
![Firefox](https://img.shields.io/badge/Firefox-FF7139?style=for-the-badge&logo=firefox-browser&logoColor=white)
* **What it is:** The only major browser engine not controlled by Google or Apple.
* **Why use it:** Unlike Chrome, Firefox still supports Manifest V2, meaning powerful adblockers work perfectly. It requires some manual tweaking (hardening) to be fully private.
* **Best for:** Power users who want to tweak their `about:config` (Arkenfox user.js).

### 🥉 3. Brave (Best for Normies / Speed)
![Brave](https://img.shields.io/badge/Brave-FF2000?style=for-the-badge&logo=brave&logoColor=white)
* **What it is:** A privacy-focused Chromium browser.
* **Why use it:** It blocks ads and trackers natively without needing extensions (which bypasses Chrome's Manifest V3 restrictions). 
* **Best for:** People who want Chrome-like speed and compatibility without the Google tracking. *(Turn off "Brave Rewards/Crypto" in settings).*

### 🕵️‍♂️ 4. Tor Browser (Ultimate Anonymity)
![Tor](https://img.shields.io/badge/Tor_Browser-7D4698?style=for-the-badge&logo=tor-project&logoColor=white)
* **What it is:** The gateway to the Onion routing network.
* **Why use it:** Routes your traffic through three encrypted, randomized nodes globally.
* **Rule of thumb:** Do NOT use Tor for logging into your personal accounts (Bank, real email, social media). It is for research and remaining untraceable. Never add extensions to Tor.

---

## 🧩 Tier 2: Essential Extensions

Do not overload your browser with extensions. Every extension you add increases your "browser fingerprint" (how unique you look to tracking algorithms). Stick to these essentials:

| Extension | Purpose | Badge |
| :--- | :--- | :--- |
| **uBlock Origin** | The undisputed king of blocking ads, trackers, and malicious scripts. *(Note: If using Chrome/Edge in 2026, you are forced to use uBlock Origin Lite, which is significantly weaker. Use Firefox/LibreWolf for the full version).* | ![uBO](https://img.shields.io/badge/uBlock_Origin-800000?style=for-the-badge&logo=ublock-origin&logoColor=white) |
| **Bitwarden** | Open-source, encrypted password manager. Never use your browser's built-in password saver. | ![Bitwarden](https://img.shields.io/badge/Bitwarden-175DDC?style=for-the-badge&logo=bitwarden&logoColor=white) |
| **Privacy Badger** | Developed by the EFF. Learns to block invisible trackers automatically. | ![Privacy Badger](https://img.shields.io/badge/Privacy_Badger-FFCC00?style=for-the-badge&logo=eff&logoColor=black) |
| **CanvasBlocker** | Spoofs your browser's fingerprint so websites can't identify your machine based on hardware/software configurations. | ![Canvas](https://img.shields.io/badge/CanvasBlocker-333333?style=for-the-badge&logo=fingerprint&logoColor=white) |
| **SponsorBlock** | Skips sponsored segments, intros, and filler in YouTube videos automatically. | ![SponsorBlock](https://img.shields.io/badge/SponsorBlock-FF0000?style=for-the-badge&logo=youtube&logoColor=white) |

---

## ⚙️ Tier 3: Browser Hardening Settings

If you are using Firefox or Brave, go into your settings right now and change these:

### 🦊 Firefox Essential Tweaks
1. Go to Settings > **Privacy & Security**.
2. Set Enhanced Tracking Protection to **Strict**.
3. Enable **"Send websites a 'Do Not Track' signal"**.
4. Disable **Telemetry** (Allow Firefox to send technical data to Mozilla).
5. Change default search engine to **DuckDuckGo**, **Brave Search**, or **SearxNG**.
6. Set DNS over HTTPS (DoH) to **Max Protection** (use NextDNS or Mullvad DNS).

### 🦁 Brave Essential Tweaks
1. Go to Settings > **Shields**.
2. Set Trackers & ads blocking to **Aggressive**.
3. Set Fingerprinting blocking to **Strict**.
4. Go to **Web3 / Crypto** settings and turn everything OFF.
5. Go to **Brave Rewards** and turn it OFF.

---

## 🧠 Tier 4: The OPSEC Bible (How to Actually Be Secure)

A secure browser means nothing if your personal habits are terrible. Follow these rules to protect your identity and data:

### 1. Compartmentalization (Don't put all your eggs in one basket)
* **Stop using one email for everything.** Have one email for banking/government, one for personal contacts, and a "burner" email (like SimpleLogin or DuckDuckGo Email Protection) for random website signups.
* **ProtonMail** or **Tuta** are the gold standards for encrypted email. Don't use Gmail for sensitive data.

### 2. Passwords & 2FA (Two-Factor Authentication)
* **Never reuse passwords.** A data breach on a random forum could give hackers the password to your bank.
* Use **Bitwarden** to generate 20+ character random passwords for every site.
* Turn on 2FA for *everything*. **Do not use SMS for 2FA** (SIM-swapping is incredibly easy). Use an authenticator app like **Aegis** (Android), **Ente Auth**, or a hardware key like a **YubiKey**.

### 3. The Truth About VPNs
* VPNs do **not** make you anonymous. They simply shift trust from your Internet Service Provider (ISP) to the VPN company. 
* If you use a free VPN, **you are the product**. They sell your data.
* Use trusted, zero-log, independently audited VPNs like **Mullvad** or **ProtonVPN**. 

### 4. Secure Your DNS
* Your ISP can see every website you visit via DNS requests. 
* Change your router and browser DNS to **NextDNS**, **Quad9 (9.9.9.9)**, or **Mullvad**. This encrypts your traffic requests and blocks malware/ads at the network level.

## 5. My setup

* i personally use libre wolf with alot of the seetiing i have implement in this repository dns over https with mullvad custom dns which is this right here https://family.dns.mullvad.net/dns-query it block mallware ads trackers adult content and even gambling so everything all around. For extension i have uBlock , CSS Exfil , CanvasBlocker,
ClearURLs , First Party Isolation , Port Authority . I curently dont have a vpn but if i am planning in the near feature mullvad is my prefrence but there are alot of other option too i suggest as iam saying above to use a vpn that has a zero log policy. This is all for my setup i am on windows with extra stuff for security but that all with all this i feel safer and more secure and i am not afraid of seeing myself in a data leak or anything particullar.
--- 
*Stay safe. Trust no one. Verify everything.*
