# Verification Checklist

## My Personal Checklist

Before using or sharing AI-generated workplace content, I will:

1. Identify the type of content, intended audience, and level of risk.
2. Compare names, dates, numbers, decisions, and figures with the original source.
3. Check that uncertainty, assumptions, and missing information are clearly labeled, not stated as fact.
4. Confirm the AI did not invent an owner, deadline, status, or cause that wasn't in the source.
5. Check that the output opens by identifying who it's for and who it's from, not just the content.
6. Remove or avoid any confidential, private, or sensitive information.
7. Record any correction made and confirm human approval before final use.

## Worked Example

### Output Selected
The executive brief in [Section 3 — Information Workflow](../03-information-workflow/information-processing-example.md), built from three days of scattered TaskFlow launch updates.

### Application of the Checklist

| Check | What I Tested | Finding | Action Taken |
|---|---|---|---|
| Content and audience | Executive brief for a director, 20-minute deadline | Correct level of detail, but the draft jumped straight into content | Added a To/From/Subject header before the bottom line |
| Names, dates, and numbers | 40% rollout, checkout bug, Thursday AM meeting | All matched the raw notes exactly | Kept unchanged |
| Decisions vs. open questions | Full rollout by Friday | Marketing called it "basically decided," but engineering had not confirmed server capacity | Kept framed as at-risk, not confirmed |
| Missing owners and deadlines | Notifications bug owner, client pricing reply owner | Not stated anywhere in the source | Replaced with `[Not Specified]` instead of guessing a name |
| Unconfirmed items | Contractor-line budget overrun | Source explicitly said "nobody confirmed" | Labeled "Unconfirmed," not stated as a fact |
| Sensitive information | Product name, client mentions | Scenario (TaskFlow) is fictional; no real client or company data | Confirmed safe for this portfolio |
| Human approval | Final brief + extraction table | Corrections reviewed against source line by line | Marked as trainee-reviewed and approved |

## Verification Result

The first AI draft was accurate on every fact traced (7 of 7 claims matched the source), but it was **not yet ready to send** because it skipped the recipient header. After applying the checklist, the header was added and every gap (bug owner, pricing-reply owner, contractor budget) was confirmed correctly marked rather than invented.

**Final decision:** Approved for inclusion as a fictional, trainee-reviewed course example.
