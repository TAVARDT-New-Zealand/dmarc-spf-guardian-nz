# DMARC, SPF and DKIM Guardian

[![Technical Audit](https://img.shields.io/badge/TAVARDT-Email%20Security-5b3cf5.svg)](https://tools.tavardt.com/nz/dmarc-checker/)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

DNS email authentication auditor for spoofing prevention, sender validation, and alignment with NZISM and CERT NZ defensive guidance.

***

## Features and Verification Capabilities

* **DMARC Policy Enforcement**: In-depth inspection of enforcement directives (reject, quarantine, and none), subdomain policy (sp), and percentage enforcement rate (pct).
* **SPF Record Audit**: Validation of authorized sender mechanisms, DNS query lookup limits, and strict enforcement qualifiers (-all vs ~all).
* **DKIM Signature Verification**: Cryptographic public key verification across specified DNS selectors.
* **Forensic and Aggregate Reporting**: Verification of aggregate (rua) and forensic (ruf) feedback loops.
* **Regulatory and Standards Compliance**: Designed in alignment with New Zealand Information Security Manual (NZISM) and CERT NZ Cyber Guidance.

***

## Installation and Quick Start

Requires Python 3.8 or higher. Built strictly using the Python standard library with zero external dependencies.

```bash
git clone https://github.com/TAVARDT-New-Zealand/dmarc-spf-guardian-nz.git
cd dmarc-spf-guardian-nz
python guardian.py enterprise.co.nz
```

To test a specific DKIM selector or export results in structured JSON format:

```bash
python guardian.py enterprise.co.nz -selector mail -json
```

***

## Enterprise Defense Consulting

For dedicated cybersecurity architecture, threat modeling, and incident readiness in New Zealand, contact **TAVARDT**.

***

## Useful Links

* **Corporate Portal:** https://ag.tavardt.com/nz/
* **Diagnostic Suite:** https://tools.tavardt.com/nz/
* **Technical Contact:** https://ag.tavardt.com/nz/contact/

***

### License
Released under the MIT License.

***

© 2026 TAVARDT. All rights reserved.
