# Final Audit Report Template

Use this template to generate a professional smart contract audit report.

## Template

```
# Smart Contract Audit Report

## 1. Executive Summary

### Project
- Project name: [PROJECT_NAME]
- Repository / codebase: [REPO_OR_PATH]
- Chain: [CHAIN]
- Review date: [DATE]
- Auditor(s): [NAMES]

### Scope
- Contracts reviewed: [LIST]
- Commit or version reviewed: [HASH / VERSION]
- Review objective: [Describe the review purpose]

### Summary
Provide a concise summary of the project, its purpose, and the overall audit outcome.

### Rating
- Overall risk level: [None / Low / Moderate / High / Critical]
- Summary of key issues: [brief overview]

## 2. Scope and Methodology

### In-Scope Contracts
- [Contract A]
- [Contract B]
- [Contract C]

### Review Method
- Manual code review
- Static analysis
- Testing and scenario review
- Business logic analysis
- Access control analysis

### Limitations
- [Known limitations, assumptions, or unverified areas]

## 3. Project Overview

Describe the protocol, its intended purpose, key actors, and interactions.

## 4. Architecture and Trust Model

- Core roles: admin, owner, guardian, pauser, governance, operator
- Upgradeability: [Yes / No]
- External dependencies: oracles, routers, tokens, governance modules
- Key assumptions: [list]

## 5. Findings Summary

| Severity | Count | Summary |
| --- | ---: | --- |
| Critical | [N] | [summary] |
| High | [N] | [summary] |
| Medium | [N] | [summary] |
| Low | [N] | [summary] |
| Informational | [N] | [summary] |

## 6. Detailed Findings

### Finding 1: [Title]
- Severity: [Critical / High / Medium / Low]
- Category: [Access control / Reentrancy / Logic flaw / Oracle risk / etc.]
- Status: [Open / Fixed / Partially addressed]
- Location: [Contract + function]

#### Description
Explain the issue in technical detail.

#### Impact
Describe the economic or security impact.

#### Root Cause
Explain the root cause and affected logic path.

#### Recommended Fix
Detail the remediation plan.

#### Verification
Describe how to validate the fix.

---

### Finding 2: [Title]
...[repeat format]...

## 7. Additional Observations

Document lower-risk issues, best-practice improvements, and non-blocking recommendations.

## 8. Risk Assessment

Summarize the overall security posture of the protocol, including notable strengths and weaknesses.

## 9. Remediation Priorities

1. Immediate fixes
2. High-priority fixes
3. Medium-priority improvements
4. Long-term hardening steps

## 10. Conclusion

Provide a final conclusion on security posture and recommended next actions.
```

## Notes

- Insert exact code references where possible.
- Keep the report evidence-based and linked to concrete code paths.
- Distinguish between confirmed issues and theoretical concerns.
