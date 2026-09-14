# Planning Workflow Example — Legacy Authentication Migration

**Scenario:** As the Technical Expert, I need to plan the migration of a legacy authentication system to a new SSO provider within 6 weeks, with limited testing windows and a dependency on another team.

## Weak Prompt (Before)

> "Create a plan to fix our login system."

**Why it's weak:** too vague. It lacks the goal's real constraint (6 weeks), the dependency on another team, and any expected structure — leading to a generic, unusable plan.

## Structured Prompt (C.A.R.E.)

- **Context:** Goal is to migrate the legacy authentication system to a new SSO provider within 6 weeks; testing windows are limited to weekends; the identity team's cooperation is a hard dependency.
- **Action:** Build a phased plan using Goal → Mechanisms → Phases → Tasks.
- **Role:** Experienced technical program lead.
- **Expected Output:** Phases with tasks, and an owner/deadline/dependency per task.

## Resulting Plan

### Goal
Migrate the legacy authentication system to the new SSO provider within 6 weeks, with zero unplanned login downtime.

### Mechanisms
- Parallel-run the old and new systems before cutover, rather than a hard switch.
- Use weekend windows only for any user-facing testing, to avoid business-hours risk.
- Treat the identity team's sign-off as a gating dependency before each phase, not an assumption.

### Phases

| Phase | Focus | Target Window |
|---|---|---|
| 1. Assessment | Map all current login dependencies and edge cases | Week 1 |
| 2. Parallel Build | Stand up the new SSO integration alongside the legacy system | Weeks 2–3 |
| 3. Controlled Testing | Test with a limited user group on weekend windows only | Weeks 4–5 |
| 4. Cutover | Full migration and legacy system decommission | Week 6 |

### Tasks

| Task | Owner | Deadline | Dependency |
|---|---|---|---|
| Document all current login integration points | Technical Expert | End of Week 1 | None |
| Build SSO integration in parallel environment | Technical Expert + Identity Team | End of Week 3 | Identity team resource availability |
| Run weekend pilot test with limited user group | Technical Expert | Week 4 weekend | Phase 2 complete |
| Review pilot results and fix any issues found | Technical Expert | Week 5 | Pilot test complete |
| Execute full cutover and monitor for 48 hours | Technical Expert + Identity Team | Week 6 | Identity team sign-off on Phase 3 |
| Decommission legacy authentication system | Technical Expert | End of Week 6 | Successful 48-hour monitoring window |

## Why This Is Stronger Than the Weak Version

- The plan is **specific to the real constraint** (6 weeks, weekend-only testing, a cross-team dependency) instead of a generic checklist.
- Every task has an **owner, deadline, and dependency** — nothing is left implicit.
- The plan stays **concise and workplace-focused**: six tasks across four phases, not an open-ended essay.
