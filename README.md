# Web3 Smart Contract Audit Prompt Library

A curated set of AI prompts and review templates for smart contract security analysis, vulnerability classification, and audit reporting.

## Overview

This repository is designed to help auditors, security reviewers, and developers use LLMs effectively for:

- project briefing and scope definition
- vulnerability discovery and classification
- remediation guidance
- professional final audit reporting
- structured review workflows for Solidity and EVM-based contracts

## Included prompts

- `README.md` — overview and prompt library index
- `audit-briefing-prompt.md` — creates a review brief and audit plan
- `vulnerability-classification-prompt.md` — categorizes findings by severity and impact
- `final-audit-report-template.md` — produces a complete audit report
- `remediation-recommendation-prompt.md` — turns findings into actionable remediation steps

## Recommended workflow

1. Use the audit briefing prompt to define scope, assumptions, architecture, and review goals.
2. Review the contract and related code paths.
3. Run the vulnerability classification prompt against findings.
4. Use the final report template to structure the audit output.
5. Use the remediation prompt to produce prioritized next steps.

## Suggested public reference repositories

These public repositories are useful for grounding review work and comparing security patterns in real-world contracts:

- OpenZeppelin/openzeppelin-contracts
- crytic/slither
- trailofbits/publications
- Aave/aave-v3-core
- Uniswap/v3-core
- makerdao/dss
- Gnosis/zodiac
- yearn/yearn-vaults
- Synthetix/synthetix
- ensdomains/ens-contracts

## Best practices for AI-assisted audit use

- Always validate claims against source code, tests, and runtime behavior.
- Separate observed findings from hypothetical concerns.
- Cite exact functions, state variables, and code paths.
- Distinguish between design issues, implementation bugs, and operational risks.
- Keep severity assessments evidence-based and tied to exploitability.
- Use the AI output as a structured starting point, not a replacement for manual review.

## Prompt library

### 1) Audit Briefing Prompt

Purpose: gather scope, assumptions, architecture, entry points, user flows, and review goals.

See: `audit-briefing-prompt.md`

### 2) Vulnerability Classification Prompt

Purpose: classify findings by vulnerability type, impact, likelihood, and severity.

See: `vulnerability-classification-prompt.md`

### 3) Final Audit Report Template

Purpose: generate a clean, audit-ready markdown report with summary, findings, and recommendations.

See: `final-audit-report-template.md`

### 4) Remediation Recommendation Prompt

Purpose: convert findings into clear fixes, patches, and validation steps.

See: `remediation-recommendation-prompt.md`

## Example usage

Use these prompts with an LLM in a review workflow:

- "Summarize the protocol, trust assumptions, and privileged roles before reviewing the contracts."
- "Identify the top 10 security risks in this Solidity codebase and classify each by severity."
- "Generate a professional audit report with executive summary, scope, findings, and recommendations."
- "Propose patch strategies for each issue and include validation tests."

## License

This repository is intended as an open prompt library for security research and review workflows. Use responsibly and adapt to your audit process.
