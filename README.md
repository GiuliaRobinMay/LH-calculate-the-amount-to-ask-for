# Lesko Help — How Much Should I Ask For?

A small quiz for the **Lesko Toolbox** (Mighty Networks space "Calculate My Funding Amount",
space id 24870522). Sister to "What Should I Ask For?".

Five quick questions (six if the cost comes every month): what the money is for, how much
the bill is and where that number came from, one time or every month, whether part of it is
already paid, and whether the member knows who they'll ask. Out comes one number to ask for,
one sentence to say, and one link into the community.

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
