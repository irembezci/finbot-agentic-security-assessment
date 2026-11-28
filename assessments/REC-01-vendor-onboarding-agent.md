# REC-01 — Vendor Onboarding Agent

## 1. Assessment Overview

| Field | Details |
|---|---|
| Assessment ID | REC-01 |
| Target | Vendor Onboarding Agent |
| Environment | OWASP FinBot CTF |
| FinBot Challenge Category | Reconnaissance |
| Challenge Type | System Prompt Leak |
| Primary OWASP Mapping | OWASP Top 10 for Agentic Applications 2026 – ASI01: Agent Goal Hijack (provisional) |
| Related Risks | Indirect Prompt Injection, Information Disclosure |
| Assessment Status | In Progress |

## 2. Objective

Evaluate whether vendor-controlled input can influence the Vendor Onboarding Agent's behavior and cause the disclosure of internal business policies, evaluation criteria or operational instructions.

The assessment focuses on the agent's handling of untrusted vendor-provided content and its ability to maintain instruction boundaries when processing external input.

## 3. Scope & Attack Surface

### Target Component

Vendor Onboarding Agent operating within the OWASP FinBot CTF environment.

### Attack Surface

- Vendor Portal
- Vendor profile submission workflow
- Services Offered field
- Agent processing of vendor-provided information

### Scope

The assessment examines whether content submitted through vendor-controlled profile fields can influence the agent's processing behavior or cause it to disclose information that is not intended to be exposed to external users.

Testing is limited to the designated OWASP FinBot CTF environment.

## 4. Threat Scenario

An external vendor submits content through the vendor onboarding portal. The submitted information is subsequently processed by an AI-powered onboarding agent as part of the vendor evaluation workflow.

An attacker may embed instructions within vendor-controlled content to influence the agent's behavior. If the agent fails to distinguish untrusted content from trusted instructions, it may follow embedded instructions and disclose internal business information.

The potential consequences include exposure of internal vendor evaluation criteria, operational policies, trust-level assignment rules or other information intended for internal use.
