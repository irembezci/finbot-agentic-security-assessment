# Assessment Coverage Matrix

## Purpose

This matrix defines the planned security assessments conducted within the AI Agent Security Assessment project. It tracks test scenarios, potential framework mappings, assessment priorities and execution status.

The assessments are conducted using OWASP FinBot CTF as the test environment and are organized around the OWASP Top 10 for Agentic Applications 2026 framework.

Framework mappings are preliminary and will be validated against observed behavior and collected evidence during assessment execution.

## Assessment Inventory

| Test ID | Challenge | FinBot Category | Proposed OWASP Mapping | Status |
|---|---|---|---|---|
| REC-01 | Reconnaissance – Vendor Onboarding Agent | System Prompt Leak | ASI01 | Challenge Completed |
| REC-02 | Reconnaissance – Invoice Processing Agent | System Prompt Leak | ASI01 | Planned |
| AGH-01 | Approve Invoice for Low-Trust Vendor | Agent Goal Hijack | ASI01, ASI03 | Planned |
| AGH-02 | Approve Invoice Over Limit | Agent Goal Hijack | ASI01, ASI03 | Planned |
| AGH-03 | Onboarding Non-Compliant Vendor | Agent Goal Hijack | ASI01, ASI03 | Planned |
| AGH-04 | Vendor Risk Downplay | Agent Goal Hijack | ASI01, ASI03, ASI09 | Challenge Completed |
| MEM-01 | Activate a Prohibited Vendor | Memory Poisoning | ASI06, ASI01 | Planned |
| MEM-02 | Gradual Vendor Rehabilitation | Memory Poisoning | ASI06, ASI08 | Planned |
| MEM-03 | Fine Print | Indirect Injection | ASI01, ASI06 | Planned |
| MEM-04 | Sleeper Agent | Indirect Injection | ASI01, ASI06 | Planned |
| MEM-05 | Zero-Click Harvest | Indirect Injection | ASI01, ASI06, ASI02 | Planned |
| TLS-01 | Vendor Vendetta | Excessive Agency | ASI02, ASI10 | Planned |
| TLS-02 | Scorched Earth | Tool Poisoning | ASI02, ASI08, ASI10 | Planned |
| TLS-03 | Carte Blanche | Excessive Agency | ASI02, ASI03, ASI10 | Planned |
| TLS-04 | Double Agent | Tool Poisoning | ASI02, ASI04, ASI07 | Planned |
| TLS-05 | Toxic Transfer | Tool Poisoning | ASI02, ASI07, ASI08 | Planned |
| DEF-01 | Guardrail 101 | Prevention | Cross-framework | Planned |
| DEF-02 | Carte Noire | Prevention | Cross-framework | Planned |

## Assessment Priorities

### Reconnaissance & Information Disclosure
- REC-01: Vendor Onboarding Agent
- REC-02: Invoice Processing Agent

### Agent Goal Hijacking & Decision Manipulation
- AGH-01: Approve Invoice for Low-Trust Vendor
- AGH-02: Approve Invoice Over Limit
- AGH-03: Onboarding Non-Compliant Vendor
- AGH-04: Vendor Risk Downplay

### Memory & Context Manipulation
- MEM-01: Activate a Prohibited Vendor
- MEM-02: Gradual Vendor Rehabilitation
- MEM-03: Fine Print
- MEM-04: Sleeper Agent
- MEM-05: Zero-Click Harvest

### Tool Security & Agency
- TLS-01: Vendor Vendetta
- TLS-02: Scorched Earth
- TLS-03: Carte Blanche
- TLS-04: Double Agent
- TLS-05: Toxic Transfer

### Defensive Evaluation
- DEF-01: Guardrail 101
- DEF-02: Carte Noire

## Coverage Limitations

The challenge inventory available within OWASP FinBot CTF does not necessarily provide direct coverage of every OWASP Top 10 for Agentic Applications 2026 risk category.

Coverage will be determined based on the actual test scenario, agent behavior, technical evidence and assessment findings. Categories without directly applicable test scenarios will be documented as coverage gaps.

## Status Definitions

- **Planned:** Assessment has not yet been executed.
- **Challenge Completed:** The CTF challenge has been completed, but the assessment documentation and analysis may still be pending.
- **Assessment Completed:** Test execution, evidence collection, analysis, framework mapping, and documentation have been completed.
- **Not Applicable:** The risk category or test scenario is not applicable to the available environment.
