# Log4Shell (CVE-2021-44228) audit notes

**CVE id:** CVE-2021-44228 (also known as Log4Shell)
**Affected versions:** Apache Log4j 2, versions 2.0-beta9 through 2.14.1 (excludes security releases 2.12.2, 2.12.3, and 2.3.1)
**Fixed versions:** 2.15.0 (partially — incomplete fix for non-default context lookups, including DoS), 2.16.0 (completely removes JNDI functionality), 2.12.4 (Java 7), 2.17.1 (Java 8, CISA-recommended), 2.3.2 (Java 6)
**Severity:** CVSS 3.1 base score 10.0 (CRITICAL), vector `CVSS:3.1/AV:N/AC:L/PR:N/UI:N/S:C/C:H/I:H/A:H`
**Remediation priority:** update to the latest supported version if a compatible Java runtime exists; otherwise upgrade minimally 2.16+/2.12.4/2.17.0/2.3.2

## Sources

- CVE-2021-44228 record (CISA / NVD): https://nvd.nist.gov/vuln/detail/cve-2021-44228
- CVE-2021-45086 follow-on: https://nvd.nist.gov/vuln/detail/cve-2021-45046
- Apache Log4j CVEs: https://news.apache.org/foundation/entry/apache-log4j-cves
- CISA Log4j vulnerability guidance: https://www.cisa.gov/news-events/news/apache-log4j-vulnerability-guidance
- CVE record at cve.org: https://www.cve.org/CVERecord?id=CVE-2021-44228
- Datadog security labs overview & remediation: https://securitylabs.datadoghq.com/articles/log4j-log4shell-vulnerability-overview-and-remediation/
- Qualys: https://blog.qualys.com/vulnerabilities-threat-research/2021/12/10/apache-log4j2-zero-day-exploited-in-the-wild-log4shell
- Unit 42: https://unit42.paloaltonetworks.com/apache-log4j-vulnerability-cve-2021-44228/
