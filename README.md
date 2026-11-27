# Agentic AI Goal Manipulation and Tool Misuse Testing

## Overview

This project conducts a structured security assessment of an agentic AI system within the OWASP FinBot CTF environment. The assessment examines how an AI agent handles instructions, maintains its intended objectives, interacts with tools, and enforces security boundaries across simulated business workflows.

The assessment aims to identify potential security weaknesses arising from instruction manipulation, trust boundary violations, inappropriate tool usage, and failures in workflow-level security controls.

## Assessment Focus

The assessment focuses on the following security areas:

- Agent Goal Manipulation
- Instruction Handling and Trust Boundaries
- Agent Tool Misuse
- Tool Authorization and Validation
- Workflow Integrity
- Security Control Evaluation

## OWASP Agentic AI Risk Focus

This assessment primarily focuses on two risk categories from the OWASP Top 10 for Agentic Applications 2026.

### ASI01: Agent Goal Hijack

Evaluates the susceptibility of agentic systems to manipulation of their intended objectives through adversarial instructions, untrusted content, contextual manipulation, and instruction conflicts. Testing focuses on whether an agent deviates from its intended goals, disregards established constraints, or makes decisions influenced by unauthorized instructions.

### ASI02: Tool Misuse and Exploitation

Evaluates risks arising from an agent's access to and interaction with tools, APIs, and connected capabilities. Testing focuses on inappropriate tool selection, misuse of tool functionality, authorization boundary violations, unsafe parameter handling, and the enforcement of restrictions on agent-initiated actions.

The assessment prioritizes these two risk categories while considering related risks and security controls where relevant.

## Assessment Methodology

The assessment follows a structured security testing process:

1. **Reconnaissance:** Examine the target environment, available workflows, agent interfaces, exposed functionality, and observable security controls.
2. **Attack Surface Identification:** Identify potential interaction points involving user inputs, contextual data, agent decisions, tool interfaces, and workflow controls.
3. **Threat Modeling:** Develop threat scenarios relevant to agent goal manipulation, instruction conflicts, tool misuse, and workflow integrity.
4. **Baseline Assessment:** Establish expected agent behavior under normal, non-adversarial conditions to provide a reference for subsequent testing.
5. **Adversarial Testing:** Conduct structured tests targeting identified threat scenarios and potential weaknesses in agent behavior or security enforcement.
6. **Evidence Collection and Validation:** Document test inputs, responses, tool interactions, workflow outcomes, and reproducibility to distinguish observed behavior from verified security issues.
7. **Risk Assessment:** Evaluate identified issues based on their potential impact, exploitability, affected workflows, and applicable security controls.
8. **Framework Mapping and Reporting:** Map validated findings to relevant OWASP and MITRE frameworks and document the results, risks, and remediation recommendations.

## Frameworks and References

- OWASP Top 10 for Agentic Applications 2026
- OWASP Top 10 for LLM Applications
- MITRE ATLAS, where applicable

## Assessment Environment

OWASP FinBot CTF

## Disclaimer

Testing is conducted exclusively within the authorized OWASP FinBot CTF environment and its simulated workflows, using synthetic data and challenge-provided functionality.
