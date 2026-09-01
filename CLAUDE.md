# Scoring Expansion — Planned but Incomplete

## Tier thresholds vs current max score

The Simple Results panel shows **"out of 21"** and the tier bar shows **Tier 4: 18–20 pts** and **Enterprise: 21+ pts**. These labels are intentionally forward-looking.

**Current max achievable score is 19** (containers 1–5, multienv 1–2, auth 1 or 3, istio 1 or 3, data 1 or 3, deploy 1 or 3 → max = 5+2+3+3+3+3 = 19). This means:

- Score of 20 is currently unreachable → Tier 4 upper bound never reached
- Score of 21+ is currently unreachable → Enterprise tier is dead code today

**When adding new questions or expanding existing score ranges**, update these to make the full tier structure reachable:
- Bring max possible score to at least 21
- Or adjust tier thresholds to match whatever the new max is
- Also update the PDF `${total}/19` hardcoded denominator (line ~1060 in `downloadPDF`)
- Update the breakdown table Max column values if question maxes change
