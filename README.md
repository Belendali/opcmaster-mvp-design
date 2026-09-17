# opcmaster · MVP design

Clickable prototype for the opcmaster MVP ad test: a site owner checks whether ChatGPT recommends their business, gets a ready-written fix, decides, and sees if it worked — all in one conversation.

**Live prototype:** https://belendali.github.io/opcmaster-mvp-design/
**Figma (section V1.0):** https://www.figma.com/design/7l0mqLoO0VOp1o4416Amgh

## Flow

1. **Landing** — enter a website URL, "Check for free".
2. **Free check, 3 steps** — Your website (reading pages) → Your business (confirm what we understood) → Questions (suggested questions and brands to compare).
3. **Free report** — how often ChatGPT mentions you and links to your site, plus the biggest gap with a locked fix.
4. **Sign up** — Google or email link, triggered by "See your fix, free".
5. **App (one conversation)** — Use this fix → add the text to your site → we ask ChatGPT again → before/after result and the next gap.

Use the yellow **Prototype** button (bottom right) to jump to any step. The language switch covers English and 中文.

## Notes

- All data is example data (Northstar Notes is a fictional site). Nothing is sent anywhere; sign-up and publishing are simulated.
- Single self-contained `index.html` (fonts from Google Fonts). `opcmaster-loop.html` is the same file under its working name.
- MVP scope: publishing is manual (copy → paste → "It's on my site"); no CMS connection yet.
