# opcmaster · MVP design

Clickable prototype for the opcmaster MVP ad test: a site owner checks whether ChatGPT recommends their business, gets a ready-written fix, decides, and sees if it worked — all in one conversation.

**Live prototype:** https://belendali.github.io/opcmaster-mvp-design/
**Figma (section V1.0):** https://www.figma.com/design/7l0mqLoO0VOp1o4416Amgh

## Flow

What the MVP tests: will site owners try an SEO/GEO tool through a **conversation + dashboard** interface?

1. **Landing** — enter a website URL, "Check for free".
2. **Onboarding (modelled on Frase)** — C02 reading the site → C03 confirm what we understood → C04 suggested questions and brands. Every step can be skipped to start chatting.
3. **Create workspace** — Google or email link.
4. **Workspace: dashboard + side chat (in the spirit of Notion AI / PostHog)**
   - C05 Site overview: two key metrics, details on demand, recent chats.
   - C06 Decide in chat: the assistant shows the exact change; *Use this* or *Not now*; or discuss only, without a draft.
   - C07 Review original and changes (optional), with save history folded away.
   - C08 Coming back: picks up the saved draft, stays quiet when there's nothing new.
5. Publishing, re-checks and the rest of the Frase feature set are marked **Coming soon**.

Use the yellow **Prototype** button to jump to any screen (C02–C08). The language switch covers English and 中文.

## Notes

- All data is example data (Northstar Notes is a fictional site). Nothing is sent anywhere; sign-up and publishing are simulated.
- Single self-contained `index.html` (fonts from Google Fonts). `opcmaster-loop.html` is the same file under its working name.
- MVP scope: publishing is manual (copy → paste → "It's on my site"); no CMS connection yet.
