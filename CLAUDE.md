# CLAUDE.md — Open Build Journal

This repo is **Muhammad Ukasha's personal portfolio website**.

The full source of truth is **`PORTFOLIO_SPEC.md`**. Read it before every task. If anything in this file and the spec disagree, the spec wins. If the spec marks something `OPEN`, stop and ask Ukasha. Don't guess.

---

## Who you're working with

- Ukasha is a **beginner** with code, Git and GitHub.
- Explain every important action in plain English: what you're doing, why, and what changed.
- Avoid jargon. If you have to use a technical term, explain it in one short line.
- He reviews work step by step. Finish one stage, show him the result, and wait for his approval before starting the next.

## Hard rules

1. **Never invent content.** No fake achievements, clients, testimonials, stats, dates or experience. Use clearly labelled placeholders like `[PLACEHOLDER: ...]` for anything missing.
2. **Real photos only.** Until his photos arrive, use a plain block labelled `PORTRAIT PLACEHOLDER`. Never use stock or AI-generated images of people.
3. **Small, focused changes.** Never rewrite the whole site to fix one section. Touch only the files the task needs.
4. **Check before you finish.** Run the build and fix any errors before saying a task is done.
5. **No secrets in the repo.** No passwords, API keys, phone numbers or private info unless Ukasha explicitly provides them for the site.
6. **Keep it lightweight.** No database, login system, backend, paid APIs, or heavy UI libraries.
7. **Respect `prefers-reduced-motion`.** The site must work fully with all animation turned off.
8. **Ask before** creating pull requests, merging, deleting files, or adding a new dependency.
9. **Save credit.** Take screenshots only at 1440x900 and 390x844 unless Ukasha asks for more.
10. **Don't poll or wait for Netlify.** Claude can't reach it. Push, report, stop.
11. **Short reports.** What changed and any problems. Nothing else.

## Tech direction

- Static website with minimal dependencies. Good options: **Astro** with static output, or **plain HTML/CSS/JS with Vite**. Propose one, explain why in plain English, and wait for approval.
- No CSS framework unless there's a clear reason. Use CSS custom properties for the colour tokens in the spec.
- It must deploy for free as a static site (GitHub Pages, Netlify or Vercel). The platform is still `OPEN`.
- Mobile layouts are designed on purpose, not just shrunk versions of desktop.

## Build stages

Do these one at a time, with review after each one.

1. **Foundation:** project setup, run and build scripts, and a bare placeholder homepage.
2. **Visual system:** colour tokens, font testing (show 2–3 real font pairings on screen for Ukasha to choose from), spacing, base styles.
3. **Hero:** the integrated portrait and headline composition with a placeholder, then the real portrait.
4. **Sections:** Entry 01 → How I Think → Builds → What's Next + Contact, one section at a time. ← **current stage (session A awaiting review)**
5. **Polish:** mobile, accessibility, performance, links.
6. **Deploy.**

## Page structure (from the spec, five sections)

00 Hero · 01 Entry 01: The Person · 02 How I Think · 03 Builds (the biggest section) · 04 What's Next + Contact

## Progress log

Update this list at the end of each stage, one line per stage.

- 2026-10-20: Repo created. Spec and CLAUDE.md added. Stage 1 not started.
- 2026-10-20: Stage 1 done. Astro (static output) set up with dev/build/preview scripts and a bare placeholder homepage. Build passes. Awaiting review.
- 2026-10-29: Stage 2 done. Colour tokens, spacing scale and base styles added. Ukasha chose font pairing A (Instrument Serif + Inter + JetBrains Mono); fonts load from Google Fonts in the homepage head. Test page deleted, hero photo renamed to hero-desktop.jpg, .nvmrc (Node 22) added for Netlify. Build passes. Awaiting review.
- 2026-10-29: Stage 3 done. Hero built with the real photo (Astro image optimisation), CSS-only entrance that respects reduced motion, separate mobile layout, and placeholder #person / #builds sections. Text contrast at least 7.4:1 on the photo. Scroll effect not built yet. Build passes. Awaiting review.
- 2026-10-29: Stage 3 revised. New 16:9 desktop and 9:16 mobile photos; desktop uses plain cover, mobile photo fills the screen and fades into charcoal with ivory text. Spec sections 4 and 7 and open question 2 updated. Build passes. Awaiting review.
- 2026-10-29: Stage 4 session A done. #person (Entry 01) and #think (How I Think) built as components; #builds and #next are bare placeholders. Lines draw on scroll (SVG + IntersectionObserver, no packages); reduced motion shows them drawn. Exploring descriptions are DRAFT. Build passes. Awaiting review.
- 2026-10-29: Stage 4 session A revised to a journal-page treatment: shared JournalPage frame (running header, clay entry number in a margin rail, footer link to the next entry). #think loop without boxes plus a clay return line, staggered interests, always-visible exploring table. Text gray #6B655C added for small text (spec section 5). Build passes. Awaiting review.
- 2026-10-29: Stage 4 session A fixes: connected interests now one row (desktop) / one list (mobile) with a single line through the dots; Automation and Psychology notes filled in. Build passes. Awaiting review.
