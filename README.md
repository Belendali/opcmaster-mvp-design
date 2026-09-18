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
5. **One chat per page.** Each check's suggestions go into the chat for that page. A later check adds new messages to an existing page chat (e.g. a second suggestion for the pricing page), opens a new chat only for a page that shows up for the first time (e.g. the homepage), and doesn't repeat suggestions you skipped. Site-wide questions get their own chat (`+ New chat`).
6. CMS publishing and the rest of the Frase feature set are marked **Coming soon**.

Prototype menu → C09 shows check #2 (overview, pricing page follow-up, new homepage chat, flashcards result). Try the suggested questions in a page chat to see what stays in the chat and what moves to a new one.

Use the yellow **Prototype** button to jump to any screen (C02–C08). The language switch covers English and 中文.

## Notes

- The demo uses answerai.pro as the example site. Its page copy is taken from the public site, but every check result, ChatGPT answer and suggestion is **made-up example data, not a real measurement**. Nothing is sent anywhere; sign-up is simulated.
- Single self-contained `index.html` (fonts from Google Fonts). `opcmaster-loop.html` is the same file under its working name.
- MVP scope: publishing is manual (copy → paste → "It's on my site"); no CMS connection yet.
