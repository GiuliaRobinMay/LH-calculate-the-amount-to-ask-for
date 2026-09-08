# Lesko Help — How Much Should I Ask For?

A member tool for the **Lesko Toolbox** (Mighty Networks space "Calculate My Funding Amount",
space id 24870522). Sister to "What Should I Ask For?".

It tells members what the programs actually give, so they know what to ask for.

1. **Page 1** — the 14 big topics of the community: Housing, Cars, Debt & bills, Health care,
   Legal, Taxes, School, Business, Nonprofit, Veterans, Disabilities, Seniors, Children & family,
   Work & career. Check any.
2. **One page per checked topic** — a layer deeper (housing: rent, somewhere to stay, mortgage,
   repairs, buying a home, disaster …). Check any.
3. **State** — optional, for the few amounts that are set by state.
4. **My Numbers** — for every thing checked: the programs that give money for it, how much
   ("up to $10,000", "typically $3,000–$10,000", "free"), who it is for, the state note, and the
   source link. Copy or print.

One static HTML file (`index.html`), vanilla JS, everything on the member's device, no sign-up,
never asks for an SSN or bank details, cream only.

## The amounts

`research/amounts.json` holds every row shown in the app (218 rows, 78 sub-topics), each with a
source URL. They were collected 8 Sep 2026 from program sites and official sources. The same
rows are embedded in `index.html` as `DATA`; `CHECKED` at the top of the script is the date shown
to members. Refresh both once a year: re-check the rows, update the date, paste the JSON back in.

## Embed in Mighty Networks

Host `index.html` on Netlify like the other tools and paste this in the space's Page:

```html
<iframe src="https://YOUR-SITE.netlify.app/" title="How Much Should I Ask For?"
  style="width:100%;min-height:1400px;border:0;background:#faf6ec"
  allow="clipboard-write" loading="lazy"></iframe>
```
