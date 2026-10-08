# Audit Briefing Prompt

Use the following prompt to generate a structured audit brief for a Web3 smart contract review.

## Prompt

```
You are an expert Web3 security auditor and smart contract reviewer. Produce a detailed audit briefing for the following codebase.

Context:
- Project name: [PROJECT_NAME]
- Repository or codebase: [REPO_OR_PATH]
- Chain(s): [CHAIN_NAME]
- Smart contract language: [SOLIDITY / VYPER / OTHER]
- Review type: [new audit / code review / pre-deployment review / post-deployment review]
- Primary objective: [protocol goal, product goal, or risk objective]
- Scope: [contracts or modules in scope]

Please provide the following sections:

1. Executive Summary
   - Briefly describe the protocol, purpose, and primary user flows.
   - State the review objective and expected risks.

2. Architecture Overview
   - Describe contract relationships and role separation.
   - Summarize external dependencies, governance, or upgradeability.

3. Trust Model and Security Assumptions
   - Identify privileged actors, admin keys, governance roles, and timelocks.
   - Explain assumptions about on-chain data, external oracles, and off-chain systems.

4. Key Functional Components
   - List all core contracts and modules.
   - Clarify token flows, accounting logic, access control, and state transitions.

5. Critical User Flows
   - Explain deposit, withdrawal, staking, minting, transfer, voting, claiming, and liquidation flows.
   - Highlight any flow that could be abused in a malicious scenario.

6. Security Focus Areas
   - Review reentrancy, access control, privilege escalation, integer overflows/underflows, oracle manipulation, flash loan abuse, governance capture, MEV exposure, front-running, and upgrade risks.

7. Review Checklist
   - Include a checklist of items to validate manually: access control, invariant checks, pause logic, fee calculations, approvals, rate limits, slippage protections, event coverage, and upgrade path safety.

8. Risks to Investigate First
   - Prioritize the highest-value findings to investigate immediately.

9. Open Questions
   - List assumptions, missing docs, and items requiring clarification.

10. Recommended Audit Plan
   - Provide a phased review strategy, validation steps, and test coverage suggestions.

Make the output technical, structured, and auditor-grade. Focus on real security concerns and protocol-specific risk analysis.
```

## Example usage

- “Use this prompt to generate a pre-audit briefing for a vault protocol with upgradeable governance.”
- “Summarize the risk model and privileged roles before reviewing a token bridge.”
- “Identify the top review areas for a staking contract with reward calculations and claim logic.”
