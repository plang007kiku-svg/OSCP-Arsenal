# 🚨 Threat Intelligence Watch: Actively Exploited Vulnerabilities

## 🔴 Urgent (Patch or Mitigate Now)

| CVE | Product | Impact | Exploitation Status | Recommended Action |
| :--- | :--- | :--- | :--- | :--- |
| **CVE-2026-20131** | Cisco Secure Firewall Management Center | Unauthenticated RCE (root) | Active exploitation by Interlock ransomware (since Jan 2026) | Upgrade to fixed version; see Cisco advisory |
| **CVE-2026-21643** | FortiClient EMS (7.4.5, 7.4.6) | SQL injection → RCE | Active exploitation (zero‑day before patch) | Upgrade to 7.4.7 or restrict API access |
| **CVE-2026-35616** | FortiClient EMS (7.4.5, 7.4.6) | Pre‑auth API bypass → RCE (CVSS 9.1) | Active exploitation | Same as above |
| **CVE-2026-20182** | Cisco Catalyst SD‑WAN | Authentication bypass → admin takeover | Active exploitation (SSH keys added, NETCONF modified) | Apply patches / block management interfaces |
| **CVE-2026-1340** | Ivanti EPMM | Code injection → unauthenticated RCE | Listed in CISA KEV (active) | Apply vendor hotfixes / isolate EPMM from internet |
| **CVE-2026-42897** | Microsoft Exchange Server | XSS (remote code execution) | Active exploitation, no official patch yet (zero‑day) | Apply Microsoft mitigations (ECP restriction, URL rewrite) |

---

## 🟡 Additional Critical Vulnerabilities (Monitor Closely)

* **CVE-2026-20122** (Cisco SD‑WAN) – Privileged API abuse, active exploitation  
* **CVE-2026-20133** (Cisco SD‑WAN) – Information disclosure, active exploitation  
* **CVE-2026-32201** (Microsoft SharePoint) – Spoofing, active exploitation  
* **CVE-2025-29635** (D‑Link DIR-823X) – Command injection, EoL product → discontinue use  

---
*Sources: CISA KEV, Vendor Security Advisories, Trusted Security Researchers (May 2026).*

