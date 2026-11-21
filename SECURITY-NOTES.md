# Log4Shell (CVE-2021-44228) — Quarterly Security Briefing Notes

**CVE:** CVE-2021-44228
**Title:** Log4Shell
**Severity:** CVSS 3.1 score 10.0 CRITICAL
**Components affected:** `log4j-core`

## Affected versions
Apache Log4j 2 versions affected: **[2.0-beta9, 2.3.1) ∪ [2.4, 2.12.2) ∪ [2.13.0, 2.15.0)** (i.e., up to and including 2.14.1, plus earlier 2.0-beta9/2.3.1/2.4/2.13.0).

## Fixed versions
Fixed in **2.3.1** (Java 6), **2.12.2** (Java 7), and **2.15.0** (Java 8 and later). Current recommended versions: **2.16.0** (Java 8 and later), **2.12.3 / 2.12.4** (Java 7), **2.3.2 / 2.3.1** (Java 6).

## Impact
Log4j's JNDI features used in configurations, log messages, and parameters do not protect against attacker-controlled LDAP and other JNDI related endpoints. An attacker who can control log messages or log message parameters can execute arbitrary code loaded from LDAP servers. Unauthenticated remote actor could take control of an affected system.

## Main sources
- Apache Logging Services Security page: https://logging.apache.org/security.html (CVE-2021-44228 details)
- CISA guidance: https://www.cisa.gov/news-events/news/apache-log4j-vulnerability-guidance
- GitHub Advisory Database: https://github.com/advisories/GHSA-JFH8-C2JP-5V3Q
- CVE Record: https://www.cve.org/CVERecord?id=CVE-2021-44228
- Wikipedia: https://en.wikipedia.org/wiki/Log4Shell
- ASF blog: https://news.apache.org/foundation/entry/apache-log4j-cves
