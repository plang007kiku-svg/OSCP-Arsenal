# 🚨 Threat Intelligence Watch: Actively Exploited Vulnerabilities (May 2026)

Verified threat intelligence report tracking vulnerabilities with confirmed active exploitation in the wild.

---

## 🔴 Critical & Urgent (Immediate Mitigation Required)

| CVE | Affected Product | Vulnerability Type | Exploitation Impact / Status | Recommended Action |
| :--- | :--- | :--- | :--- | :--- |
| **CVE-2026-21643** | Fortinet FortiClient EMS (7.4.5, 7.4.6) | SQL Injection | **Pre-auth RCE.** Exploited as a zero-day in targeted attacks before patches were released. | Upgrade to FortiClient EMS v7.4.7 or later immediately. |
| **CVE-2026-35616** | Fortinet FortiClient EMS (7.4.5, 7.4.6) | API Authentication Bypass | **Remote Code Execution (CVSS 9.1).** Used in tandem with memory flaws to compromise servers. | Apply vendor patches; restrict access to the EMS administration API. |
| **CVE-2026-20131** | Cisco Secure Firewall Management Center | OS Command Injection | **Unauthenticated RCE (root).** Actively weaponized by ransomware affiliates (Interlock/Dire Wolf variants). | Apply the official Cisco security update; isolate management interfaces. |
| **CVE-2026-20182** | Cisco Catalyst SD‑WAN | Authentication Bypass | **Admin Takeover.** Attackers are modifying NETCONF configurations and injecting unauthorized SSH keys. | Deploy Cisco fixes; tightly restrict access to SSH/NETCONF ports. |

---

## 🟡 High Alert (Active Campaign Monitoring)

* **CVE-2026-20122** (Cisco SD‑WAN vManage) – Privileged API abuse leading to unauthorized configuration modifications. Actively observed in espionage campaigns.
* **CVE-2026-20133** (Cisco SD‑WAN) – Information disclosure flaw allowing unauthenticated attackers to dump device metadata and path layouts.
* **CVE-2025-29635** (D‑Link DIR-823X) – Command injection in legacy/EoL routers. Heavily targeted by automated Mirai-variant botnets to build proxy networks. *Recommendation: Discontinue product use.*

---
*Sources: CISA Known Exploited Vulnerabilities (KEV) Catalog, Cisco Product Security Incident Response (PSIRT), Fortinet Standard Advisories (Updated: May 2026).*

