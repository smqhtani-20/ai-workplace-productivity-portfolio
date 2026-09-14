# Personal AI Integration Plan

The following plan describes realistic ways I can use generative AI as an Expert Technician while keeping accuracy, confidentiality, and final decisions under human control.

| Recurring Task | Expected Benefit | Preferred Prompt or Workflow | Main Risk / Verification Requirement | Frequency | What Success Looks Like |
|---|---|---|---|---|---|
| Turn scattered engineering/status updates into a decision-ready brief | Saves time before director/stakeholder meetings and makes risks and open decisions easier to track | Use the **Executive Brief From Scattered Updates** prompt, then follow Input → Prompt → AI Output → Human Review → Final Output | AI may state an unconfirmed item (e.g., budget, capacity) as settled fact. Compare every figure and decision against the source before sending | After multi-day gaps in status updates, before leadership check-ins | A brief is ready within 20 minutes, every claim traces to the source, and unconfirmed items stay labeled as unconfirmed |
| Draft technical status and incident communications for different audiences | Produces a solid first draft and adapts tone correctly for peers, managers, and clients without changing the underlying facts | Use the **Deployment Delay Notice** or **Root-Cause Summary (R.C.T.O.)** prompt, followed by Draft → Verify → Refine → Human Sign-off | Wrong dates, an overstated root cause, or an inappropriate tone for the audience. Verify every fact and confirm exactly one clear next action is stated | One to three times per week, or immediately after an incident | The final message is accurate, audience-appropriate, contains one clear action, and is approved before sending |
| Extract and track action items from meeting notes or incident logs | Turns messy notes into a trackable table instead of losing action items in chat history | Use the **Decisions & Actions Extraction** prompt, then apply the Verification Checklist from `05-verification/` | AI may invent an owner or deadline that wasn't stated. Trace every row to the source and mark gaps `[Not Specified]` | After every technical meeting or incident review | Every action item has a traceable source, all real gaps are marked `[Not Specified]` instead of guessed, and the table is reviewed before sharing |

## Habits I Will Build

1. Start every AI request with a structured C.A.R.E. or R.C.T.O. prompt instead of a vague one.
2. Use only fictional or properly anonymized technical details unless an approved tool and policy allow otherwise.
3. Keep the raw source next to the AI output during verification, as done in `05-verification/`.
4. Mark missing information as `[Not Specified]` or "Unconfirmed" and ask a human for clarification rather than guessing.
5. Save prompts that work well into my Prompt Library and refine the ones that don't.
6. Record human review and approval for any technical communication before it goes out under my name.
