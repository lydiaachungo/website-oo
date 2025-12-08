# 🛡️ Lydia Achungo | Cybersecurity Operations Portfolio

## About This Portfolio
This repository presents a functional demonstration of competencies across the **Cybersecurity Kill Chain**, integrating hands-on expertise in **Offensive (Red Team)** tactics with robust **Defensive (Blue Team)** strategy. The projects are interactive, built from the ground up to model complex security threats, systems, and countermeasures.

**Core Expertise:** Application Security (AppSec), Threat Detection & Response (TDR), **Digital Forensics and Incident Response (DFIR)**, and Cryptography.

---

## 🔬 Featured Operations: Deep Dive Analysis (Projects 1-7)

This section provides a highly detailed breakdown of all seven projects, emphasizing the security principles, technical implementation, and industry relevance of each.

### 1. Chronos Forensics 2.0 (Automated Attack Reconstruction)
**Domain:** Blue Team | Digital Forensics & Incident Response (DFIR) | SIEM Correlation
**Concept:** **Log Normalization**, **Risk Scoring**, and **Attack Path Reconstruction**.

* **Objective:** To model an interactive **Incident Response Platform** that can ingest disparate log sources (Web, Auth, Firewall) and automatically reconstruct the entire attack timeline.
* **Implementation Depth:** The engine performs **data normalization** on varied log formats and implements a **risk scoring algorithm** to triage events. It correlates entries by IP and time to establish the sequence of compromise, moving beyond simple alerting into **Root Cause Analysis (RCA)**. 
* **Demonstrates:** Advanced competence in **DFIR methodology**, **SIEM correlation logic** (similar to Splunk or Elastic), and the ability to process high-volume, unstructured security data into actionable intelligence.

***

### 2. Fortress WAF Simulator (OWASP Top 10 Defense)
**Domain:** Blue Team | Web Application Firewall (WAF) | Defensive Architecture
**Concept:** **Input Validation** and **Threat Surface Reduction** at the network edge (Layer 7).

* **Objective:** To model a high-performance WAF capable of real-time payload inspection against the **OWASP Top 10 (2021)**.
* **Implementation Depth:** The system utilizes robust **JavaScript regular expressions (RegEx)** to identify and neutralize attack vectors based on their signatures.
    * **A03 (Injection):** Strict RegEx filtering for SQL keywords, HTML tags, and OS command separators.
    * **A01 (Access Control):** Checks for **Path Traversal** sequences (`../`, `..\`) attempting unauthorized file access.
    * **A07 (SSRF):** Blocks internal network identifiers (`127.0.0.1`, `192.168.x.x`) to prevent **back-end pivoting**.
* **Demonstrates:** Expertise in **Application Security (AppSec)** defense and implementation of high-fidelity defensive controls.

***

### 3. Sentinel IDS v2.0
**Domain:** Blue Team | Network Intrusion Detection System (NIDS) | Threat Hunting
**Concept:** **Signature-Based Detection** and **Log Analysis**.

* **Objective:** To simulate a packet inspection engine, demonstrating the core functions of products like **Snort** or **Suricata** in identifying known network threats.
* **Implementation Depth:** The engine processes raw "log data" against a configurable rule set containing known attack signatures.
    * **Rule Engine:** The rules are structured similar to Snort signatures, defining action, protocol, and payload content.
    * **Detection Mechanism:** Uses advanced **string matching algorithms (RegEx)** to achieve high fidelity detection of shellcode patterns or unusual data exfiltration attempts.
* **Demonstrates:** Proficiency in **RegEx for pattern matching**, network traffic analysis, and developing effective **security signatures** for threat detection and triage.

***

### 4. Global Intel Map (Cyber Threat Visualization)
**Domain:** Security Monitoring | Security Operations Center (SOC) | Situational Awareness
**Concept:** **Threat Intelligence** visualization and **Risk Metric Reporting**.

* **Objective:** To visualize security events in a high-density, low-latency format, mimicking the centralized monitoring interfaces used in **SIEM** tools.
* **Implementation Depth:** Displays simulated attack origins, target regions, and attack types on a geographic map, alongside a **DEFCON status indicator** based on simulated threat severity.
* **Demonstrates:** Data aggregation, **threat intelligence** visualization, and developing front-end solutions for complex security data analysis.

***

### 5. WAF Defense Lab (Brute Force/Auth Bypass)
**Domain:** Red Team & Blue Team | Authentication Resilience
**Concept:** **Rate Limiting** and **Automated Response** for account protection (A07: Identification and Authentication Failures).

* **Objective:** To simulate the lifecycle of a high-volume **Dictionary Attack** against a login form, featuring blue team countermeasures.
* **Implementation Depth:** Simulates high login frequency and allows the user to activate controls like **IP blocking** and **Rate Limiting** logic to analyze traffic response and halt the attack.
* **Demonstrates:** Understanding of authentication vulnerabilities and implementing defensive logic to prevent account takeover (ATO).

***

### 6. SecureGen Pro (Client-Side Cryptography)
**Domain:** Security Development (DevSecOps) | Cryptography
**Concept:** **Cryptographic Strength** and **Entropy Calculation**.

* **Objective:** To provide a demonstrably secure password generator with transparent security metrics, focusing on entropy rather than simple length.
* **Implementation Depth:** Generates secure passwords and provides **real-time crack-time estimation** based on **Shannon Entropy** calculations ($log_2(\text{character\_set\_size}^\text{length})$).
* **Demonstrates:** Practical application of **cryptographic principles**, secure user interface design, and client-side implementation of security best practices.

***

### 7. Phishing Simulation (Social Engineering)
**Domain:** Red Team | Social Engineering | Security Awareness
**Concept:** **Identity and Access Management (IAM)** failure through deceit.

* **Objective:** To build a realistic **credential harvesting** tool to demonstrate the efficacy of social engineering as a threat vector.
* **Implementation Depth:** Creates a convincing, multi-step **Clone Phishing** scenario to capture and log credentials upon submission, showing the attacker's gained intelligence.
* **Demonstrates:** **Red Team methodology**, understanding of **human factors in security**, and the importance of **security awareness training**.

---

## 🛠️ Technical Stack & Expertise

* **Core Languages:** HTML5, CSS3, **Vanilla JavaScript** (All core logic for simulations is implemented directly without relying on heavy frameworks).
* **Security Concepts Mastered:** OWASP Top 10 (2021), **Digital Forensics & Incident Response (DFIR)**, **SIEM Log Correlation**, Regular Expressions (RegEx) for Pattern Matching, Cryptography, and Threat Intelligence.
* **Tools:** Git/GitHub, VS Code.

