# 🛡️ Network Attack & Defense Simulator

An interactive, browser-based cybersecurity simulator that visualizes real-time network attacks and defensive responses — built with pure HTML, CSS, and JavaScript. No dependencies, no frameworks, no backend.

![Preview](https://img.shields.io/badge/demo-live-brightgreen) ![HTML](https://img.shields.io/badge/HTML-pure-orange) ![License](https://img.shields.io/badge/license-MIT-blue)

---

---

## 📸 Preview

```
┌─────────────┐     ┌──────────────┐     ┌─────────────────────────┐
│  INTERNET   │     │     DMZ      │     │    INTERNAL NETWORK     │
│             │  🔥 │              │     │                         │
│ Attacker 1  │────▶│  Web Server  │────▶│  Core Router            │
│ Attacker 2  │────▶│  Load Balancer     │  DB Server              │
│ Botnet ×500 │────▶│  IDS / IPS   │     │  Auth Server            │
└─────────────┘     └──────────────┘     │  Admin PC               │
                                         └─────────────────────────┘
```

---

## ⚔️ Attack Types

| Attack | Description | Blocked by |
|---|---|---|
| ⚡ Brute Force | Repeated login attempts against Auth Server | Firewall rate-limiting |
| 💥 DDoS Flood | Volumetric SYN flood from botnet | Firewall + traffic shaping |
| 💉 SQL Injection | Malicious queries via web app to dump DB | IDS payload inspection |
| 👁 Man-in-the-Middle | ARP spoofing to intercept internal traffic | IDS duplicate MAC detection |
| 🕷 XSS | Script injection to steal session cookies | IDS signature matching |

---

## 🛡️ Defense Controls

- **Firewall** — blocks volumetric and rate-based attacks at the network perimeter
- **IDS/IPS** — inspects packet payloads and raises alerts on known attack signatures

Toggle each defense on/off to compare protected vs. unprotected outcomes in real time.

---

## 🚀 Features

- Animated packets traveling across network topology
- 3 network zones: Internet, DMZ, Internal Network
- 7 nodes: Attacker ×3, Web Server, Load Balancer, IDS/IPS, Core Router, DB, Auth, Admin PC
- Real-time event log with timestamps
- Live stats: blocked / detected / breached / packets
- Toggle firewall and IDS independently
- Zero dependencies — single HTML file, works offline

---

## 📦 How to Run

**Option 1 — Open locally:**
```bash
# Just open the file in any browser
open index.html
```

**Option 2 — GitHub Pages:**
1. Fork this repo
2. Go to **Settings → Pages**
3. Source: `main` branch → `/ (root)`
4. Access at `https://your-username.github.io/network-attack-simulator`

---

## 🗂️ Project Structure

```
network-attack-simulator/
├── index.html   # Entire simulator — self-contained single file
└── README.md
```

---

## ⚠️ Disclaimer

This tool is intended for **educational purposes only**. It simulates attack and defense concepts in a completely safe, offline environment. No real network traffic is generated.

---

## 📄 License

MIT © [amanda4ferreira](https://github.com/amanda4ferreira)