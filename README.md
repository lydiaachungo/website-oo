# 🛡️ Lydia Achungo | Cybersecurity Operations Portfolio

## About This Portfolio
This repository presents a functional demonstration of competencies across the **Cybersecurity Kill Chain**, integrating hands-on experience in **Offensive (Red Team)** tactics with robust **Defensive (Blue Team)** strategy. The projects are interactive, built from the ground up to model complex security threats, systems, and countermeasures.

**Core Expertise:** Application Security (AppSec), Threat Detection & Response (TDR), Cloud/Infrastructure Security, and Cryptography.

---

## 🔬 Featured Operations: Deep Dive Analysis

This section provides a highly detailed breakdown of the six featured projects, emphasizing the security principles, technical implementation, and industry relevance of each.

### 1. Fortress WAF Simulator (OWASP Top 10 Defense)
**Domain:** Blue Team | Web Application Firewall (WAF) | Defensive Architecture
**Concept:** **Input Validation** and **Threat Surface Reduction** at the network edge (Layer 7).

* **Objective:** To model a high-performance WAF capable of real-time payload inspection against the **OWASP Top 10 (2021)**.
* **Implementation Depth:** The system utilizes robust **JavaScript regular expressions (RegEx)** to identify and neutralize attack vectors based on their signatures. 
    * **A03 (Injection):** Strict RegEx filtering for SQL keywords (`UNION SELECT`, `--`), HTML tags (`<script>`), and OS command separators (e.g., `&`, `|`).
    * **A01 (Access Control):** Checks for **Path Traversal** sequences (`../`, `..\`) attempting unauthorized file access (`/etc/passwd`).
    * **A07 (SSRF):** Blocks payloads containing internal network identifiers (`127.0.0.1`, `192.168.x.x`) to prevent **back-end pivoting**.
* **Demonstrates:** Expertise in **Application Security (AppSec)** defense, understanding of **HTTP filtering logic**, and protecting against the most critical web vulnerabilities.

---

### 2. Sentinel IDS v2.0
**Domain:** Blue Team | Network Intrusion Detection System (NIDS) | Threat Hunting
**Concept:** **Signature-Based Detection** and **Log Correlation**.

* **Objective:** To simulate a packet inspection engine, demonstrating the core functions of products like **Snort** or **Suricata** in identifying known network threats.
* **Implementation Depth:** The engine ingests simulated network traffic snippets (payloads) and rapidly compares them against a custom library of **intrusion signatures**.
    * **Rule Engine:** The rules are structured similar to Snort signatures, defining action, protocol, ports, and payload content.
    * **Detection Mechanism:** Uses advanced **string matching algorithms (RegEx)** to achieve high fidelity detection of shellcode patterns, specific HTTP headers, or unusual data exfiltration attempts.
* **Demonstrates:** Deep skills in **Threat Detection and Response (TDR)**, **pattern recognition using RegEx**, and the fundamental logic behind **SIEM/SOAR** alerting mechanisms.

---

### 3. Global Intel Map (Cyber Threat Visualization)
**Domain:** Security Monitoring | Security Operations Center (SOC) | Situational Awareness
**Concept:** **Threat Intelligence** visualization and **Risk Metric Reporting**.

* **Objective:** To visualize security events in a high-density, low-latency format, mimicking a **SOC dashboard** or a **Threat Intelligence Platform (TIP)**.
* **Implementation Depth:** Utilizes geographical data and dynamic data points to plot simulated real-time attacks.
    * **Data Aggregation:** Shows simulated volume, source locations, and attack types (e.g., DDoS, Ransomware).
    * **Metric Reporting:** Features a **dynamic DEFCON status**, based on the severity and frequency of incoming simulated attacks, which is a key component in **security posture management**.
* **Demonstrates:** Proficiency in **Security Monitoring**, translating raw event data into **actionable intelligence**, and dashboard design for rapid incident assessment.

---

### 4. WAF Defense Lab (Brute Force/Auth Bypass)
**Domain:** Blue Team | Red Team | Authentication Resilience
**Concept:** **Rate Limiting** and **Automated Response** for account protection (A07: Identification and Authentication Failures).

* **Objective:** To simulate the lifecycle of a high-volume **Dictionary Attack** and the effectiveness of **anti-automation controls**.
* **Implementation Depth:** The system simulates sending hundreds of login attempts per second.
    * **Countermeasures:** Allows activation of an **IP Ban List** and a **Throttle/Rate Limiter** that monitors login frequency from a single source.
    * **Analysis:** The tool outputs log data showing successful vs. failed attempts and the **latency impact** of throttling, demonstrating resource utilization during an attack.
* **Demonstrates:** Understanding of **Authentication protocols**, the necessity of **session management controls**, and implementing defensive logic to prevent account takeover (ATO).

---

### 5. SecureGen Pro (Client-Side Cryptography)
**Domain:** Security Development (DevSecOps) | Cryptography
**Concept:** **Cryptographic Strength** and **Entropy Calculation**.

* **Objective:** To provide a demonstrably secure password generator with transparent security metrics, focusing on entropy rather than simple length.
* **Implementation Depth:** Generates random strings using character sets and employs a robust algorithm to calculate **Shannon Entropy** and provide a corresponding **crack-time estimate**.
    * **Entropy Calculation:** The system calculates $log_2(\text{character\_set\_size}^\text{length})$ to accurately measure the strength in bits.
    * **Security Principle:** The implementation is entirely **client-side** (browser-based) to ensure the generated keys never leave the user's local machine, adhering to the principle of **Confidentiality**.
* **Demonstrates:** Expertise in **Applied Cryptography**, understanding of **information theory in security**, and secure code design for sensitive operations.

---

### 6. Phishing Simulation (Social Engineering)
**Domain:** Red Team | Social Engineering | Security Awareness
**Concept:** **Identity and Access Management (IAM)** failure through deceit.

* **Objective:** To build a realistic **credential harvesting** tool to demonstrate the efficacy of social engineering as a threat vector, which is often successful even with strong technical controls.
* **Implementation Depth:** Creates a convincing, multi-step **Clone Phishing** scenario.
    * **Attack Vector:** Simulates capturing credentials upon submission to a fake back-end service.
    * **Logging:** Logs the attempted username and password, showing the attacker's gained intelligence.
* **Demonstrates:** Proficiency in **Red Team methodology**, understanding of **human factors in security**, and the importance of **security awareness training** as a defensive layer.

---

## 🛠️ Technical Stack & Expertise

* **Core Languages:** HTML5, CSS3, **Vanilla JavaScript** (All core logic for simulations is implemented directly without relying on heavy frameworks).
* **Security Concepts Mastered:** OWASP Top 10 (2021), Regular Expressions for Signature Matching, Shannon Entropy, IP Blacklisting, Command & Control (C2) Traffic Analysis, Defense-in-Depth.
* **Tools:** Git/GitHub, VS Code.

---

