# Mandatory Development Loop — V2

```text
User request
    ↓
Discover → Specify → Impact → Implement → Validate
                                     ↑           │
                                     └─ Repair ←─┤ failures (max 3 distinct attempts)
                                                 ↓ pass
                                            Regression
                                                 │
                                      regression? ├── yes → Impact → Implement → Validate
                                                 ↓ no
                                               Review
                                                 │
                                          defect? ├── yes → Implement → Validate → Regression
                                                 ↓ no
                                               Handoff
```

## Acceptance checklist
- [ ] User-visible behavior and edge cases defined
- [ ] Existing conventions, Git state, and dependencies inspected
- [ ] Impacted callers, API contracts, auth, DB, and shared modules considered
- [ ] Implementation complete within scope
- [ ] Relevant tests added/updated and executed
- [ ] Lint, typecheck, build executed when applicable/available
- [ ] Existing impacted flows regression-tested
- [ ] Diff and security reviewed
- [ ] Docs and migration/rollback notes updated if needed
- [ ] Results and unverified items clearly reported

## Final report template
**Status:** DONE / PARTIAL / BLOCKED

**Delivered:** ...

**Files changed:** ...

**Verification:** `command` — PASS/FAIL/NOT RUN (reason)

**Regression checks:** ...

**Risks and approvals needed:** ...

**Next steps:** ...

## Safety
No unattended destructive DB changes, production deploys, live DNS/firewall changes, access/secret changes, force pushes, or irreversible operations. Follow Claude Code's own permission system.
