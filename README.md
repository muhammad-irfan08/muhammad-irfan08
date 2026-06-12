# 👋 Hi, I'm Muhammad Irfan

### 🎯 Junior Penetration Tester
Hands-on offensive practitioner focused on executing penetration tests, exploiting vulnerabilities, and writing clear assessment reports for corporate environments. 

---

## 🛠️ Tools & Tech Stack
* **Tools:** Burp Suite Community, Impacket, Responder, BloodHound, GoPhish, Docker, Nmap, Metasploit.
* **Environments:** Active Directory Ranges, Web Applications, REST APIs, Linux/Windows target machines.
* **Automation:** Python & Bash (for adjusting public exploits and custom fuzzing/enumeration scripts).

---

## 🚀 Custom Lab Builds (No Pre-Made Boxes Available)
For vulnerabilities that do not have existing machines on Hack The Box or TryHackMe, I built, dockerized, and configured the target environments locally from scratch to test the exploits.

### 🌐 1. REST API & Web Custom Builds
* **CVE-2020-6950 (Eclipse Mojarra):** Built a local JavaServer Faces (JSF) environment using Tomcat to exploit local file read via path traversal.
* **CVE-2022-21703 (Grafana):** Deployed unpatched Grafana multi-tenant setups via Docker to execute API profile contamination and account takeover.
* **CVE-2023-40028 (Ghost CMS):** Ran an unpatched Node.js Ghost instance locally to exploit arbitrary file read via backend image upload endpoints.
* **CVE-2024-27130 (QNAP QTS) & CVE-2025-10611:** Set up local custom mock instances to trace parameter logic validation flaws and input sanitization issues.
* **What's inside:** My `docker-compose.yml` files, custom Python fuzzing/exploit scripts, and local environment setup notes.
* **🔗 [Go to Custom API Lab Builds](./Rest-Api/)**

### 🏢 2. Active Directory Custom Builds
* **CVE-2022-30216 (Windows Server Service):** Deployed an unpatched Windows Server evaluation ISO inside an isolated VirtualBox host-only range to trace remote execution vectors via RPC components.
* **CVE-2026-25177 & CVE-2026-41089 (Netlogon RCE):** Manually configured active domains with overly permissive Access Control Entries (ACEs) and tracking mechanics to verify modern privilege escalation logic.
* **What's inside:** Local network topology diagrams, PowerShell scripts used to spin up test domain users, and attack path captures.
* **🔗 [Go to Custom AD Lab Builds](./Active-Directory/)**

### 🎣 3. Simulated Phishing Client-Side Custom Builds
* **CVE-2023-3079 & CVE-2023-4863 (WebP Image Flaws):** Built local HTML landing pages hosting weaponized `.webp` files to trigger memory execution flaws on older, portable browser test versions.
* **CVE-2026-11645 (Chrome V8 Engine):** Researched and documented technical defense papers tracking modern browser security boundaries and JavaScript engine bypass methods.
* **What's inside:** GoPhish framework campaign scripts, raw email headers, and custom targeted spear-phishing HTML templates.
* **🔗 [Go to Custom Phishing Builds](./Phishing-simulations/)**

---

## 📄 Penetration Testing Reports Repository
Every single machine or box I hack—whether it's on Hack The Box, TryHackMe, or my own local range—gets a dedicated, professional assessment report. These reports detail the executive risk, the technical step-by-step Proof of Concept (PoC), and the exact remediation steps needed to fix the flaws.

I organize all my reports straight into the main assessment directories. You can browse through the full collection of individual machine reports here:

* **📂 [Active Directory Network Assessment Reports](./Active-Directory/)** — *Includes full walkthrough reports for TryHackMe/HTB boxes (ZeroLogon, PetitPotam, Certifried, sAMAccountName Spoofing) and my custom local ranges.*
* **📂 [REST API & Web Application Security Reports](./Rest-Api/)** — *Includes individual vulnerability assessment reports for machines targeting XStream deserialization, Apache SSRF, Joomla endpoint exposures, and custom Docker apps.*
* **📂 [Phishing & Initial Access Assessment Reports](./Phishing-simulations/)** — *Includes reports detailing credential harvesting metrics, Outlook Moniker Link hash leaks, and Microsoft Office weaponization cases.*

---

## 🤝 Connect with Me
* **LinkedIn:** [linkedin.com/in/muhammad-irfan](https://linkedin.com/in/muhammad-irfan-8368352b4) *(I post updates here whenever I finish a new box or drop a report into this repo)*
