# DMARC, SPF and DKIM Guardian | TAVARDT New Zealand

[![Technical Audit](https://img.shields.io/badge/TAVARDT-Email%20Security-5b3cf5.svg)](https://tools.tavardt.com/nz/dmarc-checker/)
[![Jurisdiction](https://img.shields.io/badge/Jurisdiction-New%20Zealand-00C853.svg)](https://ag.tavardt.com/nz/)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)

DNS email authentication auditor for spoofing prevention, sender validation, and alignment with NZISM and CERT NZ defensive guidance.

Developed and maintained by the cybersecurity and infrastructure defense division of **[TAVARDT New Zealand](https://ag.tavardt.com/nz/)**.

---

## Features and Verification Capabilities

* **DMARC Policy Enforcement**: In-depth inspection of enforcement directives (reject, quarantine, and none), subdomain policy (sp), and percentage enforcement rate (pct).
* **SPF Record Audit**: Validation of authorized sender mechanisms, DNS query lookup limits, and strict enforcement qualifiers (-all vs ~all).
* **DKIM Signature Verification**: Cryptographic public key verification across specified DNS selectors.
* **Forensic and Aggregate Reporting**: Verification of aggregate (rua) and forensic (ruf) feedback loops.
* **Regulatory and Standards Compliance**: Designed in alignment with New Zealand Information Security Manual (NZISM) and CERT NZ Cyber Guidance.

---

## Installation and Quick Start

Requires Python 3.8 or higher. Built strictly using the Python standard library with zero external dependencies.

```bash
git clone https://github.com/TAVARDT-New-Zealand/dmarc-spf-guardian-nz.git
cd dmarc-spf-guardian-nz
python guardian.py enterprise.co.nz
```

To test a specific DKIM selector or export results in structured JSON format:

```bash
python guardian.py enterprise.co.nz --selector mail --json
```

---

## Online Web Diagnostics

For continuous perimeter monitoring and graphical reporting, access the official web diagnostic suite:

* **[DMARC and Email Authentication Checker](https://tools.tavardt.com/nz/dmarc-checker/)**
* **[TAVARDT New Zealand Corporate Portal](https://ag.tavardt.com/nz/)**

---

## Enterprise Defense Consulting

For dedicated cybersecurity architecture, threat modeling, and incident readiness in New Zealand, contact **[TAVARDT New Zealand](https://ag.tavardt.com/nz/contact/)**.
