# Log4Shell Security Notes

## Core Facts

- **Log4Shell:** A critical remote code execution (RCE) vulnerability in Apache Log4j 2 (CVE-2021-44228).
- **CVE identifier:** CVE-2021-44228.
- **Severity:** CVSS 10.0 (Critical).
- **Affected versions:** All Apache Log4j 2 versions below 2.15.0.
- **Fixed version:** Apache Log4j 2.15.0 and later (recommended 2.15.0 or 2.17.1+).
- **Discovery:** 2021 by Jon Oberheide.

## Affected vs Fixed

- Affected: Log4j 2.0 through < 2.15.0.
- Fixed: Log4j 2.15.0 (and later, including 2.17.1+).

## Remediation

1. Upgrade Log4j to 2.15.0+.
2. Detect vulnerable deployments via automated dependency scanning (OWASP Dependency-Check, Snyk).
3. Disable JNDI lookups / harden Log4j (e.g., set `ldap.disabled: true`).
4. Replace all vulnerable instances.

## Sources

- NVD: https://nvd.nist.gov/vuln/detail/CVE-2021-44228
- CVE database: https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2021-44228
- Wikipedia: https://en.wikipedia.org/wiki/Log4Shell_zero-day
