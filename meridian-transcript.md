# Meridian Financial Group — AI Onboarding Portal Project
## Meeting Transcripts: Discovery Call Series
### Exported from Microsoft Teams | Converted via Whisper AI

---

## Discovery Call 1 — Initial Scoping
**Date:** February 3, 2026
**Attendees:** Sarah Chen (AE), Marcus Webb (Solutions Architect), James Okafor (Client CTO), Priya Nair (Client Head of Digital)

---

**Sarah Chen:** James, thanks for making time. Based on our initial conversations I want to make sure we're aligned on what success looks like here. Can you walk us through the core pain point again?

**James Okafor:** Sure. Our customer onboarding is taking 14 days on average. Competitors are doing it in 2. The drop-off rate at the KYC verification step is killing us — about 40% of applicants abandon there. We need that fixed.

**Marcus Webb:** We've solved this before. Real-time KYC verification integrated directly into the onboarding flow — we can have that running by sprint 3, maybe sprint 2 if the API documentation is clean. This is not a new problem for us.

**Sarah Chen:** Exactly. And Priya, you mentioned your team has been wanting a self-service portal for document uploads. That's very much in scope.

**Priya Nair:** Yes, that's critical for us. And I need to be clear — I want to be very involved in this. I'll be the product owner. I can dedicate most of my time to this project.

**Marcus Webb:** That's great to hear. Having an engaged PO is half the battle. With someone like Priya fully committed we can move fast.

**Sarah Chen:** We're thinking a 12-week delivery. Aggressive but very achievable with the right team. We'll bring 6 dedicated resources — two senior engineers, a solution architect, a UX designer, a BA, and a delivery lead.

**James Okafor:** What about the Finacle integration? That's our core banking system. Everything has to talk to Finacle.

**Marcus Webb:** Our team has done Finacle integrations before. It's not trivial but it's well within our capability. We'll scope that in properly.

**Sarah Chen:** Absolutely. Full Finacle integration is part of what we're proposing.

---

## Discovery Call 2 — Technical Deep Dive
**Date:** February 10, 2026
**Attendees:** Sarah Chen (AE), Marcus Webb (Solutions Architect), Priya Nair (Client Head of Digital), David Lim (Client IT Architecture)

---

**Marcus Webb:** David, good to have you in this one. I wanted to walk through the integration architecture with someone who knows your systems.

**David Lim:** Appreciate that. The Finacle environment is complex. We're on version 11.8, it's heavily customized, and our IT team is stretched. Any integration work needs to go through a formal change request process — minimum 4 weeks lead time.

**Marcus Webb:** That's fine. We'll plan for that. We'll kick off the change request in week 1 so we're not blocked later.

**Priya Nair:** I should mention — I'm also the product owner for our mobile banking refresh that's running in parallel. But this project is the priority. I'll make it work.

**Sarah Chen:** We've seen this before — Priya, we'll make sure we're efficient with your time. We don't need you 100%. Maybe 60-70% is enough with the right communication structure.

**Marcus Webb:** The backlog is actually something I want to talk about. We can have a solid draft ready by end of week 1. We've built onboarding portals before so we have a strong base of stories we can adapt. Priya just needs to validate, not create from scratch.

**Priya Nair:** That would be a huge help. I can't be writing stories from zero.

**Marcus Webb:** Exactly. We come in with the backlog. You validate. We're sprinting by week 2.

**David Lim:** On the KYC piece — which provider are you integrating with? We have a contract with Jumio but the API is version 1 and it's not great.

**Marcus Webb:** Jumio v1 — yeah, we've worked with that. It's manageable. We can build a wrapper that makes it behave like a real-time service even if the underlying response time isn't perfect. Users won't notice.

**Sarah Chen:** This is why you want a team that's done this before. Marcus knows every corner of these systems.

---

## Pre-Kickoff Alignment Call
**Date:** February 24, 2026
**Attendees:** Sarah Chen (AE), Marcus Webb (Delivery Lead), Priya Nair (Client PO), James Okafor (Client CTO), Lisa Park (Client PMO)

---

**Lisa Park:** I want to make sure we have the governance model clear before we sign. Who owns the backlog? Who signs off on stories?

**Sarah Chen:** Priya owns the backlog. Marcus and his team will keep it healthy. Stories get written by the delivery team, Priya validates and approves.

**Marcus Webb:** We'll have sprint planning every two weeks. Priya, I need you there for the full two hours. Outside of that we'll be mostly self-sufficient.

**Priya Nair:** Two hours every two weeks I can definitely commit to. And I'll try to do a mid-sprint check-in.

**James Okafor:** What's the go-live plan? We have a board presentation in week 15 where I need to show this live.

**Sarah Chen:** 12 weeks of delivery, plus 2 weeks of UAT, puts you at week 14. You'll have a live system with real data by week 13 for internal testing. Comfortable for a week 15 presentation.

**Marcus Webb:** We can make that work. As long as the Finacle change request goes in week 1 and we get the KYC API credentials early.

**Lisa Park:** Runbook and operational handover documentation — when does that happen?

**Marcus Webb:** We build the runbook as we go. By week 10 you'll have a solid draft. Final version delivered with go-live package.

**James Okafor:** And the team — 6 people, dedicated, for the full 12 weeks?

**Sarah Chen:** Dedicated to this engagement. Our best people.

---
*End of transcript series. Total duration: 3 meetings, approximately 4.5 hours of recorded conversation.*
*Transcription confidence: 94%. Low-confidence segments marked with [?] — none identified in this export.*
