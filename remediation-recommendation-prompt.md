# Remediation Recommendation Prompt

Use the following prompt to convert findings into clear remediation tasks and validation steps.

## Prompt

```
You are a senior smart contract engineer and security reviewer. Review the findings below and produce actionable remediation guidance.

Project: [PROJECT_NAME]
Contracts in scope: [LIST]
Audit findings: [FINDINGS]
Risk priorities: [SEVERITY / PRIORITY]

For each finding, provide:

1. Issue summary
2. Recommended code-level fix
3. Design or architecture changes if needed
4. Validation strategy
   - unit tests
   - integration tests
   - fuzzing or invariant checks
   - static analysis checks
5. Example patch direction
   - describe logic changes, guard conditions, and state checks
6. Risk after remediation
   - confirm whether residual risk remains
7. Implementation order
   - specify whether the fix should be handled before deployment or in a later hardening phase

Also provide:

- a prioritized remediation checklist ordered by severity and exploitability
- a short list of regression tests to add before production deployment
- an explanation of any trade-offs in the proposed fix
- a final recommendation on deployment readiness

Use a practical, engineering-first tone. Be specific about function-level changes and state validation needed for secure fix implementation.
```

## Example usage

- “Turn these audit findings into a patch plan and validation checklist.”
- “Recommend secure remediation steps for the critical issues found in the vault logic.”
- “Generate a deployment readiness checklist after the remediation work.”
