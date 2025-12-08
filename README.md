# 🛡️ Lydia Achungo | Cybersecurity Portfolio

**Live Deployment:** [View Live Site](https://cyber-portfolio.vercel.app)

## 📋 Mission Brief
This repository hosts a suite of interactive security tools designed to demonstrate core competencies in **Offensive Security**, **Defensive Hardening**, and **Threat Analysis**.

Unlike static portfolios, these tools are **live simulations** running in the browser, demonstrating real-world attack vectors and defense mechanisms.

---

## 🛠️ Operational Modules

### 1. [SecureGen Pro (Cryptography)](./password_generator.html)
A client-side encryption tool demonstrating high-entropy password generation.
- **Tech Stack:** JavaScript Crypto API (CSPRNG), Math.log2 for Entropy Calculation.
- **Features:**
  - Real-time "Crack Time" estimation based on current GPU hash rates.
  - Visual "Matrix" decryption animation.
  - Browser fingerprinting awareness.

### 2. [WAF Defense Lab (Blue Team)](./bruteforce_sim.html)
A simulated Security Operations Center (SOC) dashboard monitoring a live brute-force attack.
- **Concept:** Demonstrates Rate Limiting and WAF (Web Application Firewall) logic.
- **Key Features:**
  - **Live Telemetry:** Visualizes HTTP traffic spikes.
  - **Active Defense:** Includes manual "Kill Switch" and adjustable threshold sliders.
  - **Packet Inspection:** Displays raw HTTP headers of the attacker (Hydra/9.1).

### 3. [Phishing Simulation (Social Engineering)](./phishing_sim.html)
A controlled environment simulating an Adversary-in-the-Middle (AiTM) attack.
- **Concept:** Educates users on MFA Bypass techniques (Evilginx2 logic).
- **Forensics:**
  - Captures and displays "Exfiltrated" credentials locally (Safe Mode).
  - Performs **Device Fingerprinting** (OS/Browser Detection) to demonstrate metadata theft.

---

## 💻 Technical Architecture
- **Frontend:** HTML5, CSS3 (Cyber-Warfare UI Theme), Vanilla JavaScript (ES6+).
- **Deployment:** Vercel Edge Network.
- **Security:** All logic is client-side; no data is actually transmitted or stored.

## 👤 Author
**Lydia Achungo**
*Cybersecurity Analyst & Pentester*

> "You cannot defend what you do not understand."