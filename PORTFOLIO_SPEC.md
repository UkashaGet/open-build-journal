# Open Build Journal — Portfolio Spec

**Owner:** Muhammad Ukasha (`LOCKED` spelling, use it everywhere)
**Version:** 1.1, 20 Oct 2026. Distilled from the ChatGPT planning chat ("Building Your First Portfolio"), updated with Ukasha's answers.
**Rule:** This file overrides the raw chat. If the two conflict, this file wins. The raw chat is kept only as an archive.

**Status tags**
- `LOCKED`: decided, don't change without asking Ukasha
- `DRAFT`: direction agreed, wording or details can still change
- `OPEN`: not decided yet. Ask before building anything that depends on it.

---

## 0. Instructions for Claude Code

- Build from this file. Don't invent achievements, clients, testimonials, numbers, or experience.
- If something you need is marked `OPEN`, stop and ask. Don't guess.
- Work in small, reviewable stages. Never regenerate the whole site to fix one section.
- Use clearly labelled placeholders for the portrait and project visuals until real assets arrive.
- Ukasha is a beginner with code and GitHub. Explain important actions in plain English.

---

## 1. What this site is — `LOCKED`

- A **personal portfolio**: a website about Ukasha as a person.
- It is **not** a business website and **not** a freelancer sales page.
- PixelFolio (his digital services business) is **one project** shown on the site, not the identity of the site.
- **Audience:** potential clients, small business owners, collaborators, future employers.
- In under two minutes, a visitor should know:
  1. Who is this?
  2. What does he care about?
  3. What can he actually do?
  4. Why should I trust him?
  5. How do I contact him?

---

## 2. Creative direction: Open Build Journal — `LOCKED`

**Core idea:** The site is a living record of someone who explores, learns, plans, builds and keeps improving. It is not a finished résumé.

**Core sentence** (the internal north star, not necessarily shown on the site), `DRAFT`:
> An evolving record of what I'm learning, building and discovering.

**Underlying theme:** exploration and curiosity. He's trying different things to find out what fits him. He also doesn't want his current lack of knowledge to stop him from learning.

**Working loop:** Idea → Plan → Build → Learn → Improve.

**How the metaphor works**
- **Journal = the world and the story.** It uses entries, chapters, numbered builds, notes and reflections.
- **Blueprint = a secondary annotation language inside the journal.** It uses thin rules, a faint grid, small labels and arrows. It stands for planning and structure.
- **"Open"** means the journal is unfinished. The message is "I'm still writing it," not "here's my finished story."

**Visual priority order:** 1. Ukasha → 2. his story → 3. his work → 4. blueprint and journal details.

**What it should not become:**
- a literal notebook
- paper textures everywhere
- a blue engineering sheet
- a website that flips pages like a book all the way through

Design reference: a modern editorial magazine crossed with a designer's sketchbook.

**Visitor's final impression:**
> "A real person with a real mind and a real direction. He's still growing, but he thinks clearly and builds with intention."

---

## 3. Page structure (story in four acts)

The five-section structure is `LOCKED` (decided 20 Oct 2026, replacing the earlier 8-section version). Section content is `DRAFT`.

| # | Section | Act | Purpose |
|---|---|---|---|
| 00 | Hero | I: Who I am | Meet the person |
| 01 | Entry 01: The Person | I | Short personal introduction, with strengths and tools folded in |
| 02 | How I Think | II: How I think | Connected interests, "Things I'm exploring", and the Idea→Plan→Build→Learn→Improve loop, all in one section |
| 03 | Builds | III: What I've built | Projects as build records. **The biggest section on the page.** |
| 04 | What's Next + Contact | IV: Where I'm going | "Still writing.", genuinely open threads, contact, footer |

Rule: the page should spend more space showing work than describing Ukasha.

**Motion scope for v1:** hero entrance, lines drawing in How I Think, hover labels on Builds. The sketch-to-final "transformation" animation is deferred to v2, once real process material exists.

**Visual intensity across the page:**
- The hero is clean and editorial.
- The grid and annotations become more visible through Acts II–III.
- Act IV strips back to open whitespace, because the journal stays open.

Content blocks below (How I Work, Things I'm Exploring, What's Next) are kept as source material and get merged into the five sections above.

---

## 4. Hero — `LOCKED` (final version: "Option C")

**Concept:** One integrated composition. A large editorial portrait and oversized serif typography overlap to form one artwork with one focal point.

**Layers**
1. **Photo:** the main visual mass. Close crop with a strong light/shadow relationship. Takes up roughly 55–70% of the composition.
2. **Headline:** oversized serif that crosses into the portrait's space.
   - Never covers the eyes.
   - Stays readable over both light and dark areas.
   - No opaque text boxes behind it.
3. **Journal interface:** tiny labels, navigation and a scroll cue.

**Content**
- **Top-left:** `MUHAMMAD UKASHA` (small uppercase sans)
- **Top-right:** `OPEN BUILD JOURNAL / 01`
- **Small label:** `ENTRY 001`
- **Headline** (`DRAFT`, working headline): **Learning / *by building.*** on two lines, with the second line in italic or a different weight.
- **Supporting copy** (`DRAFT`): "Exploring ideas, learning new things, and turning what interests me into real projects."
- **Primary call to action:** `Explore my work →` (more visual weight)
- **Secondary call to action:** `A little about me` (quieter)
- **Bottom:** `SCROLL TO EXPLORE ↓` with a thin line
- **Optional:** one small handwritten-style note, e.g. "Still figuring things out." Only include it if the composition benefits.

**Layout (desktop starting values)**
- Height 90–100vh, outer margins 4–5vw
- Supporting copy around 30–42 characters per line
- Navigation is compact and sits at the top edge
- Must **not** read as a left-text / right-photo split

**Motion**
- The background appears first.
- The portrait and headline then reveal together. The headline reveals line by line with a fade or small upward move. No typewriter effect.
- Labels appear last.
- The whole entrance takes about 1–1.5 seconds, then stops.
- **On scroll:** the portrait shifts up slightly and the headline moves away more slowly. It should feel like the hero is becoming Entry 01, not a hard cut to the next section.

**Mobile**
- This is its own composition, not a squeezed version of desktop.
- Order: name → portrait → headline → short copy → one call to action → scroll cue.
- Keep the overlap only if it stays readable.
- No clipped letters, no tiny metadata, no text across facial features.

**Hero must not have:**
- a centered headline with a circular headshot
- rounded cards or pill buttons
- fake stats like "5+ years" or "100+ projects"
- 3D objects, AI brains, code snippets, neon, glow
- a long paragraph
- several competing animations

---

## 5. Visual system

### Palette — `LOCKED`

| Name | Hex | Use |
|---|---|---|
| Warm ivory | `#F3EBDD` | Main background |
| Soft paper | `#FAF8F2` | Secondary surfaces |
| Deep charcoal | `#24221F` | Headlines, primary text |
| Warm gray | `#79736A` | Metadata, supporting text, fine lines |
| Muted clay | `#A66E53` | Optional, very restrained accent |

- The page is mostly ivory and charcoal. Never pure white, never pure black.
- **Banned:** teal-led palette, bright blue, purple-blue gradients, neon, glassmorphism, colourful cards.
- A muted blue for blueprint lines: `OPEN` (see Open Questions).

### Typography

The three roles are `LOCKED`. The actual font families are `OPEN`.

| Role | Style | Used for |
|---|---|---|
| Display | Contemporary, characterful editorial serif. Not ornate, not wedding-invitation style. | Big statements |
| Body | Clean, highly readable sans-serif | Paragraphs, navigation, name (small uppercase, slight letter spacing) |
| Technical | Monospace, used sparingly | Labels like `BUILD 01 / 2026 / PIXELFOLIO`, `ENTRY 001`, `STATUS / ACTIVE` |

Poppins was the original choice and is **dropped**.

### Layout and components — `LOCKED`

- Lots of whitespace and strong vertical rhythm.
- A faint grid in Act II–III sections only.
- Thin rules, light borders and small corner radius. No heavy shadows, no big rounded cards, no pill buttons.
- **Buttons:** text with an arrow. Primary can have a solid charcoal fill. On hover, the arrow nudges a few pixels. No glow, no gradients.
- **Icons:** simple outline icons only. No 3D, no cartoon, no mixed styles.
- **Journal and blueprint marks allowed:** entry numbers, thin rules, small crosshairs, `BUILD 0X` labels, dates, short annotations.
- **Journal and blueprint marks not allowed:** fake coordinates or measurements, multiple handwritten notes, construction diagrams used as decoration.
- If a visitor notices the marks before the content, there are too many.

---

## 6. Motion language — `LOCKED`

**Rule:** every animation must show progression, discovery, construction, or transition. If an animation does none of these, cut it.

Use only these five types, repeated consistently:
1. **Page construction:** elements are placed onto the page in order (text → line → image → annotation).
2. **Drawing:** lines draw themselves to connect related things, e.g. interests in How I Think.
3. **Transformation (the signature):** a rough version becomes the finished version (sketch or wireframe → final project).
4. **Entry transition:** moving between sections feels like moving to the next journal entry. A literal page-turn appears at most once, if ever.
5. **Reveal:** small annotations appear on hover, e.g. `BUILT / 2026`, `TOOLS / …`, `STATUS / ACTIVE`.

**Banned:** bouncing, spinning, heavy parallax, floating elements, slow intros that delay reading.

**Required:** respect `prefers-reduced-motion`. The site must be fully usable with no animation at all.

---

## 7. Photography

The direction is `LOCKED`. The photos themselves are **not shot yet**.

- Real photos of Ukasha only. No AI portraits, no stock photos standing in for him.
- **Style:** editorial or documentary, not a LinkedIn headshot.
  - Directional natural window light
  - Warm skin tones, soft but visible shadows
  - Plain warm-neutral background
- **Clothing:** solid charcoal, black, or neutral. No logos.
- **Expression:** calm and thoughtful. Looking slightly away or toward the light works for the hero. No big posed smile.
- **Editing:** restrained warmth, natural skin texture. Light grain only if it suits the photo. No heavy orange grade, glow, or vignette.

**Shot list (minimum)**
1. Hero portrait: close crop, head and shoulders, with negative space on one side for the headline. Shoot several framings: close crop, head and shoulders, and wider with space on the left and on the right.
2. Working at desk
3. Planning or writing
4. Building something (screen, editing timeline, etc.)

The final hero text placement is decided **after** the real portrait exists. Development starts with a labelled placeholder.

---

## 8. Content

### Voice rules — `LOCKED`

- Simple, human English. Honest and grounded. Confident without bragging. Slightly reflective.
- It should sound like Ukasha on his best day: clear and genuine, not like AI and not like raw chat messages.
- **Banned phrases and patterns:** "passionate professional", "creative visionary", "digital ninja", "helped 100+ businesses", "trusted by leading brands", hype, long fluffy paragraphs.

### Honesty rules — `LOCKED`

- Demo or practice work is labelled as a concept or learning project. It is never presented as client work.
- No testimonials, client logos, statistics, or experience claims that aren't true.
- No skill bars, star ratings, or percentages.

### Deliberately left out — `LOCKED`

- Gaming
- The social-media scrolling struggle
- "I'm a leader"
- "I'm known for discipline" (the site should *show* discipline through finished work, not claim it)
- "I give joy and emotional things to others" (personal, not professional)
- Leading with location (see the Karachi note in Open Questions)

### 01 · Entry 01: The Person (About) — `DRAFT`

> I'm someone who learns best by doing. I like taking a plan, breaking it into steps, and turning it into something real. My interest in technology pushed me toward different areas — YouTube content creation, video editing, photo editing, design, AI tools, and building websites.
>
> I'm still growing, still learning, and still trying different things to understand what I do best. I don't believe in fake confidence or empty words. I believe in building real work, improving steadily, and staying focused on long-term goals.

Metadata labels around the photo: `BUSINESS STUDENT` · `TECHNOLOGY` · `AI` · `DIGITAL CREATION` · `CURRENTLY EXPLORING`

### 02 · How I Think — `DRAFT`

- **Connected interests diagram:** AI → Design → Media → Business → Psychology, linked by lines that draw in on scroll. The point is that the interests are different but connected.
- **The loop:** Idea → Plan → Build → Learn → Improve, shown as stages that connect on scroll.
- Message: he enjoys the execution phase after careful planning, and he breaks complex ideas down into practical work.

### 03 · Things I'm Exploring — `DRAFT`

Shown as numbered entries, each with a short line on hover or click:
`01 AI` · `02 Automation` · `03 Design` · `04 Psychology` · `05 Video` · `06 Web` · `07 Business`

### 04 · Builds — `DRAFT` (real details still needed)

**Template for each entry:**
```
BUILD 0X / YEAR / STATUS
TITLE
Question:      what was I trying to find out?
What I built:  the work itself
What I learned:
What I'd improve next time:
Visual:        real screenshots, logos, mockups, thumbnails
Process strip: Idea → Plan → Build → Result (rough → finished transformation)
```

**Planned entries**
1. **PixelFolio.** `STATUS / CLOSED`. Question: Can I turn digital skills into a small side income for local businesses? Shows branding, poster, services list.
   - **What happened (real):** a side project for extra income. Marketing was only posters in public places. It got zero clients and has stopped.
   - **What I learned (Ukasha's words, to be sharpened):** "You have to market your services properly. Sticking posters up wasn't enough."
   - The entry is presented as an honest closed experiment, never as a running business.
2. **YouTube.** Channel: **Muhammad Ukasha**, https://www.youtube.com/@mohd_ukasha. A thoughts-based channel. Question: Can I learn storytelling by actually making videos? Shows the process: topic research → script → edit → sound design → thumbnail → final video. *Videos to feature still to be chosen.*
3. **This portfolio.** The site itself as a build, from the planning process to the finished site.
4. **Learning projects.** Small experiments with AI, design and web. *Only include items that actually exist.*

### 05 · How I Work — `DRAFT`

> I don't like shallow work. I prefer understanding things properly, making a clear plan, and then executing it step by step. Real progress comes from consistency and staying committed to long-term goals. I'm still building my path, but I take it seriously.

- **Strengths:** learns quickly · plans before executing · long-term thinking · systems thinking · breaks complex ideas down · uses AI efficiently in work · manages multiple tasks
- **Tools and skills:** YouTube content creation · video editing (DaVinci Resolve Studio) · photo editing · Photoshop · sound design · AI-assisted workflows · content planning · website building
- Only list what he can demonstrate. Illustrator was mentioned in the chat; confirm before listing.

### 06 · What's Next — `DRAFT`

- "Currently exploring…" followed by a few genuinely open threads. No fake plans.
- Ending headline: **Still writing.** (alternative: "Still exploring. Still building.")
- Line: "There is always something new to learn, build, and explore."
- The visual language opens up here: less grid, more whitespace.

### 07 · Contact + Footer — `DRAFT`

- WhatsApp, email, social links. *Actual handles and links needed.*
- Kept extremely simple.
- **Footer:** name, short line ("Learning by building." or "Still writing."), copyright, one or two links.

---

## 9. Tech and build plan — `DRAFT`

- **Builder:** Claude Code (cloud) with a GitHub repo. Lovable and Canva are **no longer** the build tools.
- **Repo:** `open-build-journal`, public. *Not created yet.* Never commit passwords, keys, or private info.
- **Stack:** lightweight static site with minimal dependencies. No database, auth, backend, or paid APIs. Claude Code proposes the exact stack and explains it.
- **Deployment target:** `OPEN` (e.g. GitHub Pages, Vercel, or Netlify free tier). Start on a free subdomain. Buy a custom domain only after the site is something worth sending.
- **Budget:** $100 Claude Code cloud credit. Expiry reportedly around 5 Nov 2026. **Verify in account.**

**Build order:**
1. Foundation: repo, project setup, working preview and build
2. Visual system: fonts, colours, spacing, base styles
3. Hero with placeholder portrait, then the real portrait
4. Sections 01–07
5. Polish: mobile, accessibility, performance, links
6. Deploy

**Timeline:** about 15–18 days. If time runs short, cut features before cutting visual quality or basic function.

---

## 10. Open questions (resolve before or during build)

1. ~~Name spelling~~ **Resolved: Muhammad Ukasha.**
2. **Final hero headline:** "Learning by building." is a working headline. The deeper theme turned out to be exploration, and "Still exploring. Still building." was proposed. Decide one.
3. **Font families** for the display serif, body sans, and mono.
4. **Muted blue accent** for blueprint lines: yes or no. The final palette doesn't include it.
5. **Karachi in the hero copy and metadata:** the early advice was not to lead with location, but the later copy includes it. Decide.
6. ~~PixelFolio's real status~~ **Resolved: closed, zero clients.** Still needed: the real visuals (logo, poster, any branding files).
7. **YouTube details:** channel resolved. Still needed: which videos to feature, real thumbnails and timeline screenshots.
8. **Which learning projects actually exist** and have visuals.
9. **"What I'm Building Toward" (financial independence):** was in the v1 copy but isn't in the final structure. Keep it, reframe it, or drop it.
10. **Contact details:** WhatsApp number, email, which social links.
11. **Deployment platform** and domain plan.
12. **Portrait shoot date.**

---

## 11. Rejected — do not reintroduce

- Business or freelancer framing ("I help individuals and small businesses improve their digital presence")
- v1 Lovable design: teal palette, Poppins, left-text / right-portrait hero, plain skill pills, text-only project cards
- Building from a Canva template
- The Explorer (map) and Experiment Lab concepts
- Treating the blueprint as an equal theme. It stays secondary.
- A literal book or page-flip throughout the site
- Fake stats, testimonials, client claims, skill percentages
- AI-generated or stock portraits
- Neon, gradients, glassmorphism, 3D icons, flashy animation
