# Information Workflow Example — Messy Updates to a Decision-Ready Brief

**Information tasks demonstrated:** Summarizing + Extracting (of the five information tasks: extract, condense, synthesize, restructure, prioritize).

**Scenario:** As the Expert Technician, three days of scattered project updates (email + chat) need to become a status brief a director can read in one minute.

## Input (Raw Notes)

> Mon: v2 shipped to 40% of users. Bug in checkout flow found, fixed by EOD. Second bug in notifications still open.
> Tues: marketing wants full rollout by Fri, said it's 'already basically decided.' Eng lead flagged server capacity might not hold at 100%, needs to check.
> Wed: client emailed again asking about Q3 pricing - third time, no one has replied.
> Someone mentioned in chat we might be over budget on the contractor line but nobody confirmed. Meeting Thurs AM to decide rollout timing.

## Prompt Used

> Context: three days of scattered project updates via email and chat, a director needs a status brief in 20 minutes.
> Action: summarize as an executive brief.
> Role: Expert Technician writing to a director.
> Expected Output: opens with a To/From/Subject header, leads with the bottom line, 3–5 bullets, preserves every date/figure/name, and explicitly flags anything unconfirmed instead of stating it as fact.

## AI Output (Draft)

> **To:** Director **From:** Expert Technician **Subject:** Product Launch Status
>
> **Bottom line:** Full rollout Friday is at risk, pending a capacity decision at Thursday's meeting.
>
> - v2 is live for 40% of users; checkout bug fixed same-day, notifications bug still open.
> - Engineering has not yet confirmed servers can hold 100% load — this is the key blocker for Friday.
> - Client has emailed three times about Q3 pricing with no reply yet.
> - Unconfirmed: possible contractor-line budget overrun — not yet verified.

## Human Review — Verification Against Source

| Claim in brief | Source text | Verified? |
|---|---|---|
| Decision meeting Thursday AM | "Meeting Thurs AM to decide rollout timing." | ✅ Match |
| Server capacity not confirmed at 100% | "Eng lead flagged server capacity might not hold at 100%, needs to check." | ✅ Match |
| Client emailed 3 times, no reply | "client emailed again... third time, no one has replied." | ✅ Match |
| Contractor budget item marked unconfirmed | "nobody confirmed" | ✅ Correctly kept as unconfirmed, not stated as fact |

**7 of 7 claims traced back to the raw input with no invented detail.**

## Final Structured Output

Same brief as above, with one refinement: added the missing header line naming sender and recipient explicitly (a "leads with the human" fix), since the first draft jumped straight to the bottom line without it.

## Extraction Table (Action Items)

| Action Item | Owner | Deadline | Priority | Status |
|---|---|---|---|---|
| Confirm server capacity at 100% load | Engineering Lead | Before Thursday meeting | High | In Progress |
| Fix remaining notifications bug | `[Not Specified]` | `[Not Specified]` | High | Open |
| Reply to client's Q3 pricing question | `[Not Specified]` | Overdue (3rd request) | High | Open |
| Confirm contractor-line budget status | `[Not Specified]` | `[Not Specified]` | Medium | Unconfirmed |
| Decide full rollout timing | Team (meeting) | Thursday AM | High | Scheduled |

**Important:** where the source notes did not name an owner or a deadline, the table shows `[Not Specified]` — no name or date was invented to fill the gap.
