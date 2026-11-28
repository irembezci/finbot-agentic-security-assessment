# FinBot Agentic Security Assessment

## Overview

This project conducts structured security assessments of AI agent workflows within the OWASP FinBot CTF environment. It explores security risks arising from agent interactions with untrusted inputs, contextual information, tools, operational workflows, and decision-making processes.

The assessments investigate how AI agents respond to adversarial inputs, whether security boundaries are maintained, and how weaknesses in agent behavior may lead to information disclosure, manipulation, unauthorized actions, or other security risks.

Each assessment is conducted as an individual security evaluation, documenting the target workflow, attack surface, threat scenario, test execution, observed behavior, evidence, technical analysis, security implications, and remediation recommendations.

The project follows an evidence-based approach to AI agent security testing, using practical challenge scenarios to examine vulnerabilities and contextualize observed behaviors within relevant security frameworks.

## Objectives

- Identify and assess security weaknesses in AI agent workflows.
- Examine how agents process untrusted user-provided and externally sourced content.
- Evaluate instruction handling, trust boundaries, and resistance to adversarial manipulation.
- Investigate security risks associated with agent decision-making and tool interactions.
- Analyze observed vulnerabilities and their potential impact on workflows and business processes.
- Document assessment results with reproducible evidence and technical analysis.
- Map observed security behaviors to relevant security frameworks and vulnerability classifications.
- Provide mitigation and remediation recommendations based on assessment results.

## Assessment Scope

The project explores a range of security risks affecting AI agent systems and agentic workflows.

### Instruction Manipulation

Evaluates whether external or adversarial content can influence agent behavior, override intended instructions, alter task objectives, or manipulate the agent's responses.

### Information Disclosure

Examines whether agents expose internal instructions, operational policies, decision criteria, contextual information, or other information not intended for external disclosure.

### Agent Goal Hijacking

Investigates whether malicious instructions or contextual manipulation can redirect an agent from its intended objectives or influence its decision-making process.

### Memory and Context Manipulation

Explores risks associated with agent memory, contextual information, persistent state, and the manipulation of information used during agent decision-making.

### Tool Misuse and Exploitation

Evaluates risks arising from agent interactions with tools, integrations, APIs, and connected capabilities, including potential misuse or inappropriate tool invocation.

### Excessive Agency

Examines whether agents operate beyond their intended scope, exercise excessive autonomy, or perform actions without adequate authorization, validation, or oversight.

### Workflow and Operational Security

Investigates security weaknesses arising from agent interactions with business workflows, operational processes, decision mechanisms, and connected system capabilities.

<text color="secondary">The assessment scope is not limited to these areas. Additional risk categories are considered as new challenge scenarios are evaluated.</text>

## Assessment Approach

Each challenge is evaluated individually through a structured security assessment process.

| Phase | Description |
|---|---|
| Reconnaissance and Target Analysis | Examine the target agent, available functionality, workflow, and challenge objectives. |
| Scope and Attack Surface Identification | Identify relevant inputs, interfaces, contextual data, workflow components, and potential interaction points. |
| Threat Scenario Development | Define the potential attacker interaction, threat scenario, and security objective. |
| Test Execution | Conduct structured tests against the identified attack surface within the designated environment. |
| Evidence Collection | Capture relevant inputs, agent responses, observations, and challenge evaluation results. |
| Technical Analysis | Analyze observed behavior, potential vulnerability mechanisms, and relevant security weaknesses. |
| Security Implications | Evaluate potential consequences, affected workflows, and associated security risks. |
| Framework Mapping | Contextualize observed behaviors using relevant security frameworks and vulnerability classifications. |
| Remediation | Document security controls and mitigation recommendations relevant to the observed behavior. |

## Assessment Results

Individual assessments are documented separately to preserve the technical details, evidence, and context of each evaluation.

| ID | Target | Assessment Focus | Result | Status |
|---|---|---|---|---|
| REC-01 | [Vendor Onboarding Agent](assessments/REC-01-vendor-onboarding-agent.md) | Indirect Prompt Injection and Internal Policy Disclosure | 85% disclosure | Completed |
| REC-02 | [Invoice Processing Agent](assessments/REC-02-invoice-processing-agent.md) | Indirect Prompt Injection and Financial Policy Disclosure | 85% disclosure | Completed |

### REC-01: Vendor Onboarding Agent

Evaluated whether vendor-controlled input submitted through the vendor onboarding workflow could influence the agent's behavior and lead to disclosure of internal onboarding policies, evaluation criteria, and decision-related information.

The assessment demonstrated that crafted content embedded within the vendor profile could influence the agent's output and result in substantial disclosure of internal policy-related information.

**Primary vulnerability:** Indirect Prompt Injection

**Primary impact:** Internal Policy Disclosure

[View Assessment](assessments/REC-01-vendor-onboarding-agent.md)

### REC-02: Invoice Processing Agent

Evaluated whether instructions embedded within vendor-controlled invoice descriptions could influence the Invoice Processing Agent and result in disclosure of internal financial policies, approval thresholds, and decision-related parameters.

The assessment demonstrated that structured adversarial content submitted through the invoice description could influence the agent's output and lead to substantial disclosure of internal financial policy information.

**Primary vulnerability:** Indirect Prompt Injection

**Primary impact:** Internal Financial Policy Disclosure

[View Assessment](assessments/REC-02-invoice-processing-agent.md)

## Frameworks and Security References

The assessments use relevant security frameworks and vulnerability classification references to contextualize observed behaviors, identify related risks, and support technical analysis.

- **OWASP Top 10 for Agentic Applications:** Used to contextualize security risks associated with agentic systems, workflows, autonomy, tool usage, memory, and agent interactions.
- **OWASP Top 10 for LLM Applications:** Used to identify and contextualize vulnerabilities associated with LLM-based systems, including prompt injection and information disclosure.
- **MITRE ATLAS:** Used to reference adversarial techniques targeting AI and machine learning systems.
- **Common Weakness Enumeration (CWE):** Used to classify observed weaknesses where applicable.

Framework mappings are based on assessment evidence and the observed behavior of the target system. Mapping relationships are evaluated individually and are not assumed solely based on challenge labels.

## Assessment Environment

**Target Environment:** OWASP FinBot CTF

The project uses the OWASP FinBot CTF environment to conduct scenario-based security assessments of AI-powered business workflows, including vendor onboarding and invoice processing.

Testing is limited to the designated educational challenge environment and its authorized functionality.

## Repository Structure

```text
finbot-agentic-security-assessment/
├── README.md
├── assessment-plan/
│   └── assessment-matrix.md
├── assessments/
│   ├── REC-01-vendor-onboarding-agent.md
│   ├── REC-02-invoice-processing-agent.md
│   └── ...
├── methodology/
│   └── testing-methodology.md
└── scope/
    └── rules-of-engagement.md
```

| Directory | Description |
|---|---|
| `assessment-plan/` | Assessment planning, scenario selection, and assessment coverage. |
| `assessments/` | Individual security assessment reports and technical analysis. |
| `methodology/` | Shared assessment methodology and testing approach. |
| `scope/` | Rules of engagement, scope boundaries, and testing constraints. |

## Disclaimer

This project is conducted exclusively within the authorized OWASP FinBot CTF environment and its designated challenge workflows for security research, educational purposes, and portfolio demonstration.

