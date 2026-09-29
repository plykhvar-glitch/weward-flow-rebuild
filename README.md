# WeWard — onboarding & paywall rebuild

**Live prototype: https://plykhvar-glitch.github.io/weward-flow-rebuild/**

A clickable prototype of WeWard's onboarding and Premium paywall, re-sequenced for conversion.
The art direction is WeWard's own: Wardy, the mint speech bubbles, the orange pill buttons, the
purple Premium screens. Only the order of the screens and a few lines of copy changed.

Every screen has a side panel explaining the change. Chips under the phone jump to any screen with
answers pre-filled. The second tab holds the ranked list of changes.

## What was kept

- Every question the app asks: name, gender, age, motivations.
- Wardy's conversation layout, the working age wheel, the colour-coded motivation chips.
- The 4,500-step daily goal, the hold-to-commit star, the gauge and the first-Wards card.
- Both Premium screens' visuals, the Free vs Premium table, and both plan cards with their prices.

## Ranked changes

| # | Priority | Change | What changed | Expected impact |
| :-- | :-- | :-- | :-- | :-- |
| 1 | Fix first | Answers used, not just collected | You ask for age, gender and up to seven motivations, and none of them comes back. A short loader and the goal screen now show them, before any price. | CR +10–20% |
| 2 | High | Premium screen names the goal | The Premium screens say the same thing to everyone. The headline now uses the first name and the 4,500-step goal the flow just set. | CR +15–20% |
| 3 | High | Second screen when the paywall closes | Closing the paywall ends the flow. It now opens one more screen: your free week laid out day by day, plus the 4,49 € monthly plan. | ARPU +10–15% |
| 4 | High | Reminders asked after the paywall | The notification request came just before the tutorial and the paywall. It now comes after the paywall. | CR +10–15% |
| 5 | High | Your rating next to the plans | There is no rating or user count on the Premium screens. Your 4.8 from 223K App Store ratings and "30M walkers" now sit above the plans. | CR +10–15% |
| 6 | High | Referral code moved to the end | A code field was the second screen, before anyone saw what WeWard does. It now closes the flow. | CR +5–10% |
| 7 | Medium | Two perk screens become one | Two screens in a row listed the same Premium perks. They are now one screen with your Free vs Premium table. | CR +5–10% |
| 8 | Medium | Yearly saving made obvious | The 12-month card shows 53,88 € crossed out, with no saving stated. It now says Save 39%. | CR +5–15% · ARPU +10–15% |
| 9 | Medium | Apple Health asked when it's needed | Health access was asked before the goal existed. It now comes right before the gauge that uses it. | CR +5–10% |
| 10 | Medium | "No charge today" under the button | The free week appeared only in the button label. The line under it now says no charge today, then 32,99 € a year. | CR +3–8% |
| 11 | Low | First name used | You ask for the name and then say "Nice to meet you!" without it. It now appears on the next screens. | CR +3–8% |

*Impact ranges are Adapty's expected effect from teardowns and A/B tests across subscription apps —
not measured lift for WeWard.*

## Grounding

Prices, ratings, quotes and feature rows come only from WeWard's own published material: the
French App Store listing (4.8 from 223K ratings; Premium Monthly 4,49 €, Premium Annual 32,99 €),
wewardapp.com (30 million walkers across 29 countries, +24% walking, the three testimonials) and
WeWard's in-app screens (the free week, the Free vs Premium rows, "200% more Wards"). The full
list, including the figures left out and why, is in the **Sources & grounding** panel of the
prototype.

## Run locally

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000/. Add `?s=offer` (or any screen id) to open a specific screen.
