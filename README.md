# Masar

**Team:** Masar

## Project Idea

Masar is an Agentic AI ecosystem that connects people who want to learn and build AI with businesses that need AI solutions.
It creates a pathway from learning and building to connecting, adopting solutions, and unlocking future opportunities in Saudi Arabia and beyond.

---

## The Agentic AI Ecosystem — Start Smart prototype

`index.html` is a self-contained, working prototype. Open it in any modern browser. No build step, no server, no API keys.

- **Live:** https://masartechai.github.io/Masar/ (GitHub Pages, served from `main`)
- **Local:** double-click `index.html`, or serve the folder with any static server.

### Positioning

**Learn → Use → Build → Connect → Adopt → Scale.** One ecosystem with four entry points: learners/users, builders/creators, businesses, investors. Masar's differentiation is the **connection layer** between stages that already have good tools — it makes no "first" or "only" claims.

### What the homepage does

| # | Section | Question it answers |
| --- | --- | --- |
| 1 | Hero + the 40-second animated story (learn → build → check → list → subscribe → grow → invest) | What is Masar? |
| 2 | Why Masar exists (six stages light up on scroll) | Why does it exist? |
| 3 | The connection layer + "Why not ChatGPT?" | Why is it different? |
| 4 | From AI capability to economic value + one verified data point | Why does it matter in Saudi Arabia? |
| 5 | Four entry points (hover shows which paths feed which) | Where do I enter? |
| 6 | Learn: from user to creator | How does a learner become a creator? |
| 7 | **Business AI discovery engine** (the live demo) + Before / With Masar | How does a business use it? Where is the AI? |
| 8 | AI solutions marketplace (filterable, fictional examples) | What do solutions look like? |
| 9 | Builders: turn AI skills into opportunities | Why would builders join? |
| 10 | Invest: capital follows opportunity | Where does investment fit? |
| 11 | The Masar flywheel | How does it compound? |
| 12 | Why Saudi / Vision 2030 | Why here, why now? |
| 13 | Start small: four phases + initial monetization hypothesis | Is it feasible? Who pays? |
| 14 | Trust | Why is this responsible? |
| 14b | Five questions every judge asks, with links to the evidence | Does it hold up? |
| 15 | Final CTA | Try it. |

### The live demo (2–3 minutes)

Homepage → **Find your path** → **I want AI for my business** → describe a workflow (or tap an example) → **Analyze my workflow** → five-step analysis → **Opportunity** screen with the step-by-step reasoning (workflow → repetitive task → bottleneck → AI opportunity → recommended solution → why) → **Explore solution** → problem, how it works, capabilities, limitations, human involvement, Masar Verified → **Connect with builder** → request → confirmation → **Back to the ecosystem** (flywheel).

Routes: `#/opportunity`, `#/solution`, `#/solution/<id>` (marketplace browse mode), and `#<section>` anchors on the homepage. State survives refresh via `sessionStorage`.

### Recommendation engine

Local, rule-based, deterministic (`recommend()` in `index.html`). Keyword evidence outweighs department; department breaks ties; **WorkflowPilot AI** is the honest fallback. Exercise it from the console: `Masar.recommend("text", "Department", "Business type")`. The UI labels it as rule-based and explains that a production version would place a language model behind the same reasoning steps.

| Signals in the text | Recommendation |
| --- | --- |
| invoice, receipt, spreadsheet, bookkeeping, accounting, expense… | InvoiceFlow AI |
| customers, questions, WhatsApp, support, inquiries, complaints, messages… | SupportFlow AI |
| CV, resumes, candidates, recruitment, hiring, interviews, applicants… | RecruitMatch AI |
| anything else repetitive | WorkflowPilot AI |

### What is real and what is not

- The four solutions are **fictional prototype examples**, labelled as such throughout. No customers, partners, revenue, funding, users, market sizes or testimonials are claimed.
- The only statistic shown is verified: **45.2% of Saudi internet users use AI tools** (Saudi Internet Report 2025, CST) — labelled as AI-tool use, not agent adoption.
- **Masar Verified** is an internal Masar evaluation label, not government, SDAIA or Vision 2030 certification.
- Masar is aligned with Vision 2030 priorities but is an independent startup prototype, not a government product.
- Only the Business path is functional. Learn, Build and Invest are positioning for later phases and say so.

### Design reference

`reference/masarsite-v2.html` is the earlier Masarite v2 prototype whose visual identity this build carries forward.

### Animated diagram

`diagrams/agent-economy.html` — a standalone six-step animated story (learn → build → Masar quality check → marketplace → a business subscribes, Sara keeps ownership and earns monthly revenue → more businesses subscribe and she builds the next agent). Not linked from the prototype.
