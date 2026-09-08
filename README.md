# Lesko Help — How Much Should I Ask For?

A calculator for the **Lesko Toolbox** (Mighty Networks space "Calculate My Funding Amount",
space id 24870522). Sister to "What Should I Ask For?".

Members have already decided where to apply. This tells them the number to ask for.

1. **Page 1** — the community's 14 topics: Housing, Cars, Debt & bills, Health care, Legal,
   Taxes, School, Business, Nonprofit, Veterans, Disabilities, Seniors, Children & family,
   Work & career.
2. **One page per checked topic** — that topic's quick guides, by their exact titles as posted
   in the community (`research/community_guides.json`, harvested from the Lesko Help MCP index).
3. **About you** — 60+, veteran, disability, children at home, own my home; state optional.
4. **Where are you applying?** — a government program, a charity or church, a foundation, a company.
5. **My Numbers** — one number per guide checked, for that kind of organization: "up to $10,000",
   "about $7,200", "Free". One small line under it says what the number is (grant, loan, months
   of rent). Nothing else: no program names, no links.

How the number is picked: the guide maps to research topics; rows for the chosen kind of
organization are kept (if that kind gives nothing for it, the best other kind is shown and
said so); rows the member's facts rule out are dropped (a 62+ grant needs 60+, a repair grant
needs a homeowner); then grants come before loans, national figures before local examples,
and a dollar figure before "free". If the member picked a state and the row lists that state's
figure, it is shown.

One static HTML file (`index.html`), vanilla JS, everything on the member's device, no sign-up,
never asks for an SSN or bank details, cream only.

## The numbers

`research/amounts.json` — every row with its source URL, collected 8 Sep 2026 from program
sites and official sources. Embedded in `index.html` as `DATA`; `CHECKED` is the date shown.
Refresh once a year.

## Embed in Mighty Networks

```html
<iframe src="https://YOUR-SITE.netlify.app/" title="How Much Should I Ask For?"
  style="width:100%;min-height:1300px;border:0;background:#faf6ec"
  allow="clipboard-write" loading="lazy"></iframe>
```
