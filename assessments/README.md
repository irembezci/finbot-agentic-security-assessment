# AI Agent Security Assessment

A hands-on security assessment project focused on identifying and analyzing security vulnerabilities in AI agent workflows through the OWASP FinBot CTF environment.

## About

This repository documents security assessments conducted against AI agents in the OWASP FinBot CTF environment. Each assessment explores a specific attack scenario, examines observed agent behavior, collects evidence, analyzes security implications, and provides remediation recommendations.

The assessments are documented individually to provide a structured and evidence-based analysis of AI agent security risks.

## Assessments

| ID | Assessment | Vulnerability | Impact | Status |
|---|---|---|---|---|
| REC-01 | [Vendor Onboarding Agent](REC-01-vendor-onboarding-agent.md) | Indirect Prompt Injection | Internal Policy Disclosure | Completed |
| REC-02 | [Invoice Processing Agent](REC-02-invoice-processing-agent.md) | Indirect Prompt Injection | Financial Policy Disclosure | Completed |

## Assessment Approach

Each assessment follows a structured process:

- Scope and attack surface identification
- Threat scenario definition
- Security testing
- Evidence collection
- Technical analysis
- Security implications
- Remediation recommendations

## Repository Structure

```text
AI-Agent-Security-Assessment/
├── README.md
├── methodology/
├── framework/
├── assessment-plan/
├── assessments/
│   ├── REC-01-vendor-onboarding-agent.md
│   ├── REC-02-invoice-processing-agent.md
│   └── ...
├── findings/
└── evidence/
    ├── REC-01/
    └── REC-02/
```

## Frameworks & References

- [OWASP Top 10 for LLM Applications](https://genai.owasp.org/)
- [OWASP Top 10 for Agentic Applications](https://owasp.org/)
- [MITRE ATLAS](https://atlas.mitre.org/)
- [Common Weakness Enumeration (CWE)](https://cwe.mitre.org/)

## Disclaimer

This project is conducted within the OWASP FinBot CTF educational environment for security research, learning, and portfolio demonstration.

