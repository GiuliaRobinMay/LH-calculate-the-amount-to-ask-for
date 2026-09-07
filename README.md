# Lesko Help — How Much Should I Ask For?

A member tool for the **Lesko Toolbox** (Mighty Networks space "Calculate My Funding Amount",
space id 24870522). Sister to "What Should I Ask For?". It answers one question: *how much
should I ask for?* — by turning the member's own bills and quotes into one number, with the
math, a sentence to say, the flags a reviewer would raise, what one door typically gives, and
where in the community to take it.

Same pattern as the other Lesko App Lab tools: **one static HTML file** (`index.html`),
vanilla JS, everything stays on the member's device (localStorage), no sign-up, never asks
for an SSN or bank details, light cream only, embedded in the community via iframe.

## The quiz

Page 1 sorts the kind of money, then only the pages that apply are shown.

**Path one — a cost I already have** (rent, utilities, repair, medical, funeral, deposit,
disaster, school): what it costs and where each number comes from → how many months (only if
a cost repeats) → what is already covering part of it (disaster: insurance → FEMA → loan, in
that order) → the costs people forget → have you asked here before, and their limit if known →
state (optional).

**Path two — a business, nonprofit or project**: line items with a reason each → the costs
people forget → your own share (cash, hours, things you own, donated help) → the funder's
biggest and usual award, and whether it's your first time.

**The result**: the gap (real cost − covered) as the number to ask for, clamped to the door's
limit when known; a one-sentence ask to copy; a printable budget table with "paper / guess"
tags; flags (guesses, no amount, bigger than this door, bigger than one door, monthly costs,
100% asks, big first asks, "miscellaneous" lines, once-a-year doors); "what one door typically
gives" with source and last-checked date; community links only (guides, Questions Channel,
Call Sheet Classes, Grant Basics Step 5) — never the AI Grant Researcher.

Every dollar figure in `DOORS` is a public figure from the program or a primary source with
its URL. `CHECKED` at the top of the script is the last-checked date — refresh the table and
that date once a year.

## Research

`research/sizing-the-ask.html` is the brief that defines the tool (competitors, the eight
expert rules, program caps, first-timer mistakes, the question set). `research/RESEARCH.md`
holds the raw notes and sources.

## Embed in Mighty Networks

Host `index.html` (Netlify, same as the other tools) and paste this in the space's Page:

```html
<iframe src="https://YOUR-SITE.netlify.app/" title="How Much Should I Ask For?"
  style="width:100%;min-height:1400px;border:0;background:#faf6ec"
  allow="clipboard-write" loading="lazy"></iframe>
```
