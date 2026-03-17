# The Delivery Mirror
### Phase 1: The Gap Finder

> *What was promised. What was signed. What is happening. All three — in one view.*

An agentic system that reads your sales call transcripts, audits your SOW, and surfaces every gap between what was verbally committed and what was actually signed — before a single sprint starts.

**Part of the PAVE framework:** Promise → Alignment → Velocity → Execution

---

## Phase 1 Capability (This Repo)

Two agents run sequentially:

**Agent 1 — Transcript Analyst**
Reads meeting transcript exports (.md from Loom, Teams, or Zoom) and extracts every promise, commitment, assumption, and stakeholder signal made by the vendor team.

**Agent 2 — Reconciliation Agent**
Cross-references transcript analysis against the signed SOW. Finds every gap. Scores severity (CRITICAL / HIGH / MEDIUM / LOW). Estimates which week each gap becomes a crisis if unaddressed.

**Output:** A structured gap report with pre-kickoff actions, stakeholder risk signals, and what is actually well-aligned.

---

## Synthetic Demo Documents

Test the system with the included Meridian Financial scenario:

- `meridian-transcript.md` — 3 discovery calls, 4.5 hours, exported from Teams
- `meridian-sow.md` — the signed SOW that doesn't quite match what was said

The gaps the system finds in this scenario are modeled on real delivery failures observed across enterprise consulting engagements.

---

## Deploy

Same pattern as all projects in this portfolio — static HTML + Vercel serverless function.

1. Fork/clone repo
2. Import to Vercel
3. Add `ANTHROPIC_API_KEY` environment variable
4. Deploy

No build step. No framework. Deploys in under 60 seconds.

---

## Roadmap

- **Phase 2:** Story Generator — SOW → Jira backlog via MCP
- **Phase 3:** Assignment Orchestrator — stories → dev agents
- **Phase 4:** Async Monitor — weekly delivery health scoring
- **Phase 5:** Full PAVE loop — sales call to deployed code, humans govern

---

## Built By

Tanu Panigrahy — Agentic Architect | Enterprise AI Strategist

*"I spent years watching the gap between what was sold and what was delivered destroy margins and damage client relationships. I built a system that finds those gaps on day zero."*

---

## License

MIT
