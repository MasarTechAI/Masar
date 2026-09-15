# Masar

**Team:** Masar

## Project Idea

Masar is an Agentic AI ecosystem that connects people who want to learn and build AI with businesses that need AI solutions.
It creates a pathway from learning and building to connecting, adopting solutions, and unlocking future opportunities in Saudi Arabia and beyond.

---

## Working prototype

`index.html` is a self-contained, working prototype of Masar's core interaction:

**Business problem → AI opportunity → AI solution → Builder**

Open it in any modern browser. No build step, no server, no API keys.

- **Live:** https://masartechai.github.io/Masar/ (GitHub Pages, served from `main`)
- **Local:** double-click `index.html`, or serve the folder with any static server.

### The three-screen flow

| Screen | What happens |
| --- | --- |
| **01 · Discover** | The SME owner picks a business type and department and describes a repetitive workflow in their own words. Inputs are validated and kept in application state. |
| **Analysis** | A four-step analysis state (reading → identifying repetitive tasks → mapping opportunities → finding a solution) ends with *AI opportunity found*. |
| **02 · Opportunity** | A summary of the workflow, an explanation of which part could be assisted or automated by Agentic AI, the recommended solution, and a Before / With Masar comparison. |
| **03 · Solution** | Problem it solves, how it works (Input → AI processing → Human review → Output), capabilities, limitations, Before / After, the Masar Verified label with its disclaimer, and **Connect with builder**. |
| **Connect** | A confirmation modal (*Ready to connect?* → *Request connection* → *Connection request submitted*) with *Back to Masar* and *Start again*. |

The Discover screen also positions the wider ecosystem (Learn → Build → Connect → Adopt → Scale) and Masar's Saudi-first direction (Saudi Arabia → GCC → Global) aligned with Vision 2030 priorities.

### Recommendation engine

The analysis is a local, rule-based engine (`recommend()` in `index.html`). No AI model is called and nothing is sent anywhere.

- Keyword evidence in the workflow text is scored first (English and a few Arabic terms).
- The chosen department breaks ties and decides when the text has no signals.
- **WorkflowPilot AI** is the honest fallback for any other repetitive operational work.

| Signals in the text | Recommendation |
| --- | --- |
| invoice, receipt, spreadsheet, bookkeeping, accounting, expense, financial records… | **InvoiceFlow AI** |
| customers, questions, WhatsApp, support, inquiries, complaints, messages… | **SupportFlow AI** |
| CV, resumes, candidates, recruitment, hiring, interviews, applicants… | **RecruitMatch AI** |
| anything else repetitive | **WorkflowPilot AI** |

You can exercise the engine from the browser console: `Masar.recommend("text", "Department", "Business type")`.

### What is real and what is not

- The four solutions are **fictional prototype examples**, not real customers, companies or deployed products. The interface labels them as such.
- **Masar Verified** is a Masar-created evaluation label. It is not a government, SDAIA or Vision 2030 certification and implies no official endorsement.
- Masar is aligned with Saudi Vision 2030 priorities but is an independent startup, not a government product.
- State lives in the browser (`sessionStorage`) so a refresh keeps the user's input. Nothing is transmitted or stored server-side.

### Design reference

`reference/masarsite-v2.html` is the earlier Masarite v2 prototype. The working prototype carries its visual identity forward: the obsidian ground, mint and violet accents, Archivo display type with mono labels, hairline cards, the network canvas, the Before / With Masar journey component, and the amber prototype-disclosure flags.

### Not built (by design)

Login, payments, dashboards for learners, builders or investors, messaging, real AI deployment, real integrations. The prototype proves one excellent user flow.
