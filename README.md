# Lesko Help — How Much Should I Ask For?

A small quiz for the **Lesko Toolbox** (Mighty Networks space "Calculate My Funding Amount",
space id 24870522). Sister to "What Should I Ask For?".

Three short pages: check your problems, put an amount next to each, and say whether you already
have some of it. Out comes the total, the little budget, and one sentence to say.



One static HTML file (`index.html`), vanilla JS, everything stays on the member's device,
no sign-up, never asks for an SSN or bank details, light cream only.

The `research/` folder holds the research behind the questions. It is for the team, not for
members, and nothing from it is shown in the app.

## Embed in Mighty Networks

Host `index.html` on Netlify like the other tools and paste this in the space's Page:

```html
<iframe src="https://YOUR-SITE.netlify.app/" title="How Much Should I Ask For?"
  style="width:100%;min-height:1100px;border:0;background:#faf6ec"
  allow="clipboard-write" loading="lazy"></iframe>
```
