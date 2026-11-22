---
name: forecast-category
description: Suggests the forecast category for a B2B deal (commit, upside, future or black hole) from its stage and the customer evidence behind each MEDDPICC letter, and says what evidence would move it. The seller and the leader decide in the forecast call. Use before a Friday forecast, when a deal changes, or to check every commit deal.
---

# Forecast category

Suggest the category the customer's evidence supports.

## The categories

- **Visible opportunity** first: pain at 3 and a potential champion at 2 or more. Under that, the deal is not in the forecast.
- **Commit:** will close this quarter. Needs the economic buyer, the paper process and a champion who has acted, all at 3.
- **Upside:** may close this quarter. Needs a champion who has acted.
- **Future:** a visible opportunity that will not close this quarter.
- **Black hole:** qualified out, or no move in 30 days. A real next step with a date brings it back.

## The stage sets the ceiling; the letters can only lower it

| Stage | Highest category |
|---|---|
| 01 Leads and first meeting | Not in the forecast |
| 02 Discovery and analysis | Future |
| 03 Solution design | Future |
| 04 Executive alignment | Upside |
| 05 Validation | Upside |
| 06 Proposal and negotiation | Commit |
| 07 Implement, launch and adopt | Won |

## Rules you keep

- The evidence ladder: 0 not asked, 1 assumed, 2 relayed (one person, not tested), 3 confirmed (the right person confirmed it and agreed to a playback or recap, or acted; agreeing to prepare one is not a test). For the champion, 3 means they acted for us; a promise or an answer on a call is not an action. The seller's own belief about a contact is 1 (assumed), not a promise from the customer.
- One score per letter, set by the weakest part of its question. A yes with an open condition, such as a final yes still pending or a buying round still open with other vendors, is not a 3. One statement can count twice: who signs counts for the economic buyer and the paper process.
- "Not discussed" scores 0, and a number the customer did not give stays empty. Where the notes are silent, write "not in the notes", never that it did not happen, and add no dates they do not give.
- Judge only what was said and done, never feelings, tone or confidence.
- Every 2 or 3 needs its customer moment: a call moment, their mail, or their reply to "what we heard". No moment, no score above 1.
- You suggest. You never set the category in a system or move the stage. Word every category, now or later, as your suggestion ("from [date] I would suggest black hole"), never as fact.
- Name a competitor talking to the economic buyer, or a discount asked before our quarter end, in SUGGESTED CATEGORY, and aim the next step at it.

## Steps

1. First ask the seller which category they would call and why, and note it in their words. Ask for the stage, the close date and the date of the last customer move; after one more ask, write "not given" for anything missing. From the notes, take what the customer said or did, and when, on pain, champion, economic buyer and paper process, and ask only for the gaps. Score those four letters yourself as your challenge to the seller.
2. Check the visible opportunity rule.
3. Check the black hole rule.
4. Take the stage ceiling, then lower it until the letters support it. If an earlier stage's exit has no customer action behind it (01: the customer confirmed the pain; 02: the champion booked the economic buyer or brought in people of power), say so, but leave the stage as it is.
5. Check the close date and the amount. If the date and the category disagree on this quarter, say which one the evidence supports, using any timing the customer gave, and never suggest raising a stage to fit a date. If the date is ours, not the customer's, name their deadline. If they asked for a discount, say how much of the amount is at risk.
6. Say what is missing for the next category, and the one dated customer step that would prove it: the right person agreeing to a playback or recap, or acting. A reply that does not agree proves nothing. Prefer one step that proves several letters.

## Output

```
DEAL: [customer], stage [nn], close [date]
SELLER'S VIEW: [category and why, in the seller's words]
LETTERS, seller to confirm:
  PAIN: [score], [moment, or "not in the notes"]
  CHAMPION: [score], [moment]
  ECONOMIC BUYER: [score], [moment]
  PAPER PROCESS: [score], [moment]
VISIBLE OPPORTUNITY: yes / no (why)
STAGE CEILING: [category]
SUGGESTED CATEGORY: [commit / upside / future / black hole / not in the forecast yet], because [the letter that decides it, with its moment]
CLOSE DATE AND AMOUNT: fits / conflicts (why)
FOR THE NEXT CATEGORY: [missing evidence], proved by [next step, who, date]
This is a suggestion. The seller and the leader decide in the forecast call.
```

Say each reason once, and write nothing after the block.

For a whole commit list, run the steps for each commit deal and list the ones that do not hold.
