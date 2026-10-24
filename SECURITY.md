# Security Policy & Vulnerability Disclosure

Omnesight designs and deploys sovereign operational intelligence and autonomous execution infrastructure for mission-critical enterprise environments. We maintain rigorous security standards to safeguard core telemetry pipelines, data sovereignty, and transactional integrity.

---

## Supported Versions

Security updates, integrity patches, and hotfixes are maintained across active enterprise releases:

| Version | Status | Security Support Level |
| :--- | :--- | :--- |
| **v2.x (Current)** | Stable Production | Critical & High Priority Patches (< 24h SLA) |
| **v1.x** | Enterprise LTS | Maintenance Security Patches |
| **< 1.0** | Deprecated | Unsupported |

---

## Reporting a Vulnerability

We treat all security vulnerability disclosures with utmost urgency and confidentiality.

If you believe you have discovered a vulnerability, security flaw, or potential exposure across Omnesight infrastructure, APIs, or libraries:

1. **Do NOT report security vulnerabilities via public GitHub issues, discussions, or pull requests.**
2. Send an encrypted advisory directly to our Directorate of Security:
   * **Direct Security Email:** [security@omnesight.com](mailto:security@omnesight.com)
   * **Subject Line:** `[Vulnerability Advisory] - Component / Scope - Severity`

### Information to Include in Your Report
To accelerate validation and mitigation, please provide:
* **Description:** A detailed explanation of the issue and potential operational impact.
* **Reproduction Steps:** Step-by-step instructions, minimal proof-of-concept (PoC) payload, or reproducible script.
* **Affected Components:** Specific endpoints, worker pipelines, telemetry listeners, or client libraries.
* **Scope & Attack Vector:** Authentication bypass, privilege escalation, telemetry spoofing, data leakage, or injection.

---

## Response Timeline & SLA Commitments

Our security response team adheres to the following protocol:

* **Initial Acknowledgment:** Within **24 hours** of submission.
* **Triage & Risk Assessment:** Within **48 hours**, including severity rating (CVSS v3.1).
* **Remediation & Patch Deployment:** Critical vulnerabilities are hotfixed within **72 hours** and synchronized across air-gapped and VPC deployments under active SLAs.
* **Coordinated Disclosure:** We adhere to responsible disclosure practices and request that reporters refrain from sharing details publicly until mitigations have been deployed.

---

## Institutional Data Sovereignty & Isolation Guarantees

* **Single-Tenant VPC / On-Premise Boundaries:** Omnesight infrastructure deploys into client-isolated VPCs or air-gapped on-premise clusters.
* **Zero Model Training on Customer Data:** Customer telemetry, transactional streams, and ERP records are strictly isolated and never ingested into multi-tenant frontier model weights.
* **Cryptographic Traceability:** Every automated operational execution is recorded with immutable audit logs and SHA-256 cryptographic provenance.

For general inquiries regarding compliance, SOC 2 / ISO 27001 readiness, and institutional architecture whitepapers, contact:  
**Direct:** [security@omnesight.com](mailto:security@omnesight.com) | [compliance@omnesight.com](mailto:compliance@omnesight.com)
