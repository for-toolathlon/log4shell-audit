# Log4Shell Audit — SECURITY-NOTES.md

- **CVE identifier:** CVE-2021-44228
- **Common name:** Log4Shell
- **What it is:** Critical remote code execution (RCE) vulnerability in Apache Log4j 2 via the JNDI lookup feature. An attacker sending specially crafted log messages can execute arbitrary code on affected systems.
- **Severity:** CVSS 3.x base score **10.0 / Critical** (vector `CVSS:3.1/AV:N/AC:L/PR:N/UI:N/S:C/C:H/I:H/A:H`)
- **Affected versions:** Apache Log4j 2.0-beta9 through 2.15.0 (excluding the security releases 2.12.2, 2.12.3, and 2.3.1). From Log4j 2.15.0 onward, the vulnerable behavior was disabled by default; from 2.16.0 functionality was removed. Certain Java 7 environments (log4j 2.12.2, 2.12.3) and Java 6 (2.3.2) remain vulnerable — see vendor guidance for tier-2 fix versions.
- **Fixed versions:** Apache Log4j 2.16.0+ (completely removes the JNDI lookup behavior); for Java 7, 2.12.2–2.12.3; for Java 6, 2.3.2. Log4j 2.15.0 addressed the most severe vulnerability but had incomplete fixes in some non-default configurations (DoS).
- **Sources:**
  - CVE Record: https://www.cve.org/CVERecord?id=CVE-2021-44228
  - CISA Advisory / Apache Logging Security: https://www.cisa.gov/news-events/news/apache-log4j-vulnerability-guidance
  - ACSC cyber.gov.au alert (10 Dec 2021): https://www.cyber.gov.au/alert/critical-remote-code-execution-vulnerability-found-log4j2-library
  - Wikipedia: https://en.wikipedia.org/wiki/Log4Shell
  - CISA Mitigation Guidance: https://www.cisa.gov/news-events/apache-log4j-vulnerability-guidance
