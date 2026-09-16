# Masar

**Team:** Masar

## Project Idea

Masar is an Agentic AI ecosystem that connects people who want to learn and build AI with businesses that need AI solutions.
It creates a pathway from learning and building to connecting, adopting solutions, and unlocking future opportunities in Saudi Arabia and beyond.

---

## The AI Agent Ecosystem — Start Smart prototype

`index.html` is a self-contained, working prototype. Open it in any modern browser. No build step, no server, no API keys.

- **Live:** https://masartechai.github.io/Masar/ (GitHub Pages, served from `main`)
- **Local:** double-click `index.html`, or serve the folder with any static server.

### Positioning

**The AI Agent Ecosystem — the bridge between AI agent creation and the market demand that drives adoption.** Creators build agents, businesses bring demand, Masar checks quality (accuracy, precision, data privacy) and connects the two. Learn → Build → Verify → List → Adopt → Earn → Invest. No "first" or "only" claims.

### What the homepage does

| # | Section | Question it answers |
| --- | --- | --- |
| 1 | Hero: headline, three direct doors (Explore agents / Build / Learn), bridge diagram over a moving network | What is Masar? |
| 2 | Seven static frames: learn → build → check → list → subscribe → grow → invest | How does the whole loop work? |
| 3 | Creators build, businesses need, Masar connects + "Why not ChatGPT?" | What does Masar actually do? |
| 4 | Four doors (Learn, Build, Business, Invest) | Where do I start? |
| 5 | Tabs: how each step works (Learn, Build, Discover, Adopt & earn, Invest) | How does each part work? |
| 6 | **Business AI discovery engine** (the live demo) + Before / With Masar | How does a business use it? Where is the AI? |
| 7 | Explore AI agents (marketplace, fictional examples) | What do agents look like? |
| 8 | Creators: Masar brings demand | Why would creators join? |
| 9 | Why Saudi / Vision 2030 | Why here, why now? |
| 10 | Start small: four phases + business model | Is it feasible? Who pays? |
| 11 | Trust | Why is this responsible? |
| 12 | Five questions every judge asks | Does it hold up? |
| 13 | Final CTA | Try it. |

### The live demo (2–3 minutes)

Homepage → **Find your path** → **I want AI for my business** → describe a workflow (or tap an example) → **Analyze my workflow** → five-step analysis → **Opportunity** screen with the step-by-step reasoning (workflow → repetitive task → bottleneck → AI opportunity → recommended solution → why) → **Explore solution** → problem, how it works, capabilities, limitations, human involvement, Masar Verified → **Connect with builder** → request → confirmation → **Back to the ecosystem** (flywheel).

Routes: `#/opportunity`, `#/solution`, `#/solution/<id>` (marketplace browse mode), and `#<section>` anchors on the homepage. State survives refresh via `sessionStorage`.

### Recommendation engine and the agent catalogue

Local, rule-based, deterministic (`recommend()` in `index.html`). Keyword evidence outweighs department; department breaks ties; the **Operations Workflow Agent** is the honest fallback. Exercise it from the console: `Masar.recommend("text", "Department", "Business type")`. The UI labels it as rule-based.

Ten fictional prototype agents, six curated on the marketplace (View all reveals the rest). The marketplace is problem-first: "What do you need to solve?" leads to the agent.

| Department | Business problem | Agent |
| --- | --- | --- |
| Finance | Manual invoice / receipt processing | Invoice Processing Agent |
| HR | CV screening and shortlisting | Recruitment Screening Agent |
| Operations | Repetitive task coordination and follow-ups | Operations Workflow Agent |
| Sales | Leads lost or followed up inconsistently | Lead Qualification Agent |
| Marketing | Creating and distributing content | Marketing Content Agent |
| Customer Service | Repetitive customer questions | Customer Support Agent |
| Procurement | Comparing supplier quotations manually | Procurement Comparison Agent |
| Legal & Compliance | Checking documents for required information | Document Compliance Agent |
| IT | Repetitive internal support requests | IT Support Agent |
| Management | Information scattered across reports | Business Insights Agent |

Agents work together (each listing shows "Works with"), and a creator chooses whether to keep an agent private or publish it.

### What is real and what is not

- The ten agents are **fictional prototype examples**, labelled as such throughout. No customers, partners, revenue, funding, users, market sizes or testimonials are claimed.
- **Masar Verified** is an internal Masar evaluation label, not government, SDAIA or Vision 2030 certification.
- Masar is aligned with Vision 2030 priorities but is an independent startup prototype, not a government product.
- Only the Business path is functional. Learn, Build and Invest are positioning for later phases and say so.

### Design reference

`reference/masarsite-v2.html` is the earlier Masarite v2 prototype whose visual identity this build carries forward.

### Animated diagram

`diagrams/agent-economy.html` — a standalone six-step animated story (learn → build → Masar quality check → marketplace → a business subscribes, Sara keeps ownership and earns monthly revenue → more businesses subscribe and she builds the next agent). Not linked from the prototype.
