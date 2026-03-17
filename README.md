# The Delivery Mirror
### Phase 1: The Gap Finder

> *What was promised. What was signed. What is happening. All three — in one view.*

An agentic system that reads your sales call transcripts, audits your SOW, and surfaces every gap between what was verbally committed and what was actually signed — before a single sprint starts.

**Part of the PAVE framework:** Promise → Alignment → Velocity → Execution

---

## What It Does (Phase 1)

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

## ⚠️ Prototype Limitations

**This is a Phase 1 prototype.** It demonstrates the core agentic pattern and validates the use case. It is not yet enterprise-grade. Current limitations include:

**Input constraints**
- Accepts plain text (.md) only — transcripts must be manually exported and converted before upload
- No direct integration with Loom, Microsoft Teams, Zoom, or other recording platforms
- SOW input is text paste only — no native .docx, .pdf, or multi-file upload support
- No support for ingesting supporting materials from the broader sales cycle (RFPs, proposals, email threads, slide decks, prior engagement history)
- Context window limits apply — very long transcripts or SOWs may need to be trimmed before input

**Output constraints**
- Gap report is rendered in-browser only — no downloadable PDF, Word, or structured export
- Recommended actions are directional guidance, not assigned tasks — no workflow integration
- No persistent storage — results are not saved between sessions

**Scale and reliability**
- Single-user, single-session architecture — not designed for team use or concurrent analysis
- No audit trail or version history
- API key is client-side — not suitable for sharing broadly without a server-side proxy

**Intelligence constraints**
- Analysis quality depends on transcript completeness — poor transcription quality degrades output
- Agent judgment is probabilistic — human review of all CRITICAL gaps is strongly recommended before acting
- No industry-specific calibration — risk scoring is general, not tuned to FSI, healthcare, or public sector delivery norms

---

## Enterprise Vision — What This Becomes

The prototype proves the concept. The enterprise version of The Delivery Mirror is a full delivery intelligence platform. Here is what that build looks like:

**Multimodal input pipeline**
Direct ingestion of Loom recordings, Microsoft Teams meeting recordings, Zoom transcripts, and Gong call recordings — no manual export required. Upload .docx SOWs, PDFs, RFP responses, proposal decks, and email threads. The system processes all inputs and builds a unified commitment model for the engagement.

**Full sales cycle intelligence**
Rather than a single SOW snapshot, the enterprise version ingests the entire pre-sales trail — discovery calls, demos, proposal iterations, pricing negotiations, and stakeholder communications. The Reconciliation Agent traces commitment drift across the full arc of the sale, not just the final document.

**Structured, downloadable outputs**
Gap reports exportable as branded PDF, Word, or structured JSON. Executive briefing format suitable for delivery to client sponsors or internal MDs. Machine-readable output for downstream pipeline integration.

**Remediation workflow engine**
Each identified gap comes with specific, sequenced remediation steps — not just directional recommendations. Steps are prioritised by effort, urgency, and dependency. The system generates a pre-kickoff action plan that can be executed immediately.

**CRM and platform integration**
Direct integration with Salesforce and HubSpot to pull deal history, contact records, and prior engagement notes into the analysis context. Gap remediation tasks pushed directly to ServiceNow, Jira, or Asana — assigned to named individuals with due dates, linked to the originating gap.

**Continuous delivery monitoring (Phases 3-5)**
The gap finder is Phase 1. Phases 3-5 extend the system to monitor delivery health throughout the engagement — comparing sprint actuals against SOW commitments on a weekly basis, scoring drift, and surfacing emerging risk before it becomes a client conversation.

**Governance and audit layer**
Full audit trail of every analysis run, every gap identified, and every remediation action taken or deferred. Role-based access for delivery leads, MDs, and client stakeholders. Compliance-ready logging for regulated industries.

---

## Deploy (Phase 1)

1. Fork/clone this repo
2. Import to Vercel — no build settings required
3. Add `ANTHROPIC_API_KEY` environment variable *(optional — users can enter their own key in the UI)*
4. Deploy — live in under 60 seconds

---

## Roadmap

| Phase | Capability | Status |
|---|---|---|
| Phase 1 | Gap Finder — transcript + SOW reconciliation | ✓ Live |
| Phase 2 | Story Generator — SOW → Jira backlog via MCP | Planned |
| Phase 3 | Assignment Orchestrator — stories → dev agents | Planned |
| Phase 4 | Async Delivery Monitor — weekly health scoring | Planned |
| Phase 5 | Full PAVE loop — sales call to deployed code | Roadmap |

---

## Built By

Tanu Panigrahy — Agentic Architect | Enterprise AI Strategist

*"I spent years watching the gap between what was sold and what was delivered destroy margins and damage client relationships. I built a system that finds those gaps on day zero."*

---

## License

MIT — use it, fork it, build on it.
