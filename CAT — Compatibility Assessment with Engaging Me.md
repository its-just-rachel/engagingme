# Cognitive Attack Taxonomy — Compatibility Assessment with Engaging Me
*April 28, 2026 | Source contributed by Sean*

---

## Overview

The Cognitive Attack Taxonomy (CAT) at cognitiveattacktaxonomy.org is an independently developed framework for classifying cognitive manipulation attacks across digital and human systems. This document assesses its compatibility with the Engaging Me Engagement Ethics Benchmark and identifies where CAT vocabulary, citations, and classification dimensions can enrich the Engaging Me model.

**Bottom line:** CAT and Engaging Me are complementary, not duplicative. They approach the same problem from different angles — CAT as threat intelligence vocabulary; Engaging Me as engagement design ethics. CAT's independent development of a structurally convergent framework serves as external validation for the Engaging Me model's architecture.

---

## Structural Mapping: V-E-T → Engaging Me

CAT organizes entries in a three-layer structure that maps cleanly to the Engaging Me model:

| CAT Layer | CAT Definition | Engaging Me Equivalent |
|-----------|---------------|----------------------|
| **Vulnerabilities** | Cognitive potentialities for exploitation — features of human cognition that can be misused | **Biases** — the psychological levers the system pulls (loss aversion, availability heuristic, automation bias, etc.) |
| **Exploits** | Manipulation mechanisms that activate vulnerabilities | **Tactics** — specific design moves that convert cognitive susceptibility into influence |
| **TTPs** (Tactics, Techniques, Procedures) | Implementation methodologies — concrete deployment of exploits | **Dark Patterns** — named, deployable harmful design implementations |

This convergence is significant because CAT was developed independently by a security/cognition community without reference to the Engaging Me model. That both frameworks arrive at the same three-layer architecture reinforces the validity of both.

---

## CAT's Human Interconnection Model: Layer Mapping

CAT extends the OSI model (Layers 1–7) with three human-facing layers:

| Layer | Name | Relevance to Engaging Me |
|-------|------|--------------------------|
| 8 | Human (biases, heuristics, psychological influence) | **Primary zone of Engaging Me** — all biases and most tactics operate here |
| 9 | Organizational (policy, culture, institutional behavior) | Not currently in scope for Engaging Me; natural future extension (what org structures enable dark pattern deployment?) |
| 10 | Legal (compliance, regulation, jurisdiction) | Not in scope; relevant to regulatory positioning of the paper |

Engaging Me is primarily a Layer 8 framework. CAT's framing of Layers 9 and 10 suggests a natural future extension: documenting what organizational and legal conditions permit or fail to prevent dark pattern deployment (see dp_026 Consent Rerouting — the labyrinthine settings architecture is a Layer 9 organizational choice).

---

## CAT's Maturity Classification Dimension

CAT classifies entries by operational maturity — an orthogonal dimension from severity that captures how established a pattern is in practice:

| Level | Definition | Example Application |
|-------|-----------|-------------------|
| Theoretical | Documented as a vulnerability class; not yet observed in deployment | Agentic applications of some patterns |
| Proof-of-Concept | Demonstrated in controlled conditions | Some agentic amplification modes |
| Observed in Wild | Documented instances in real-world deployment | Most Engaging Me dark patterns |
| In Common Use | Widespread deployment; industry-standard practice | Countdown timers, urgency messaging, roach motels |
| Well-Established | Embedded infrastructure; rarely questioned | Personalization frameworks, engagement metrics optimization |

**Key insight:** Severity and maturity are orthogonal. A pattern can be HIGH severity but only "Observed in Wild" in agentic contexts (dp_027, Incentive Signal Exploitation), or LOW severity but "Well-Established" (minor countdown displays). This distinction is especially useful for flagging emerging agentic applications of established dark patterns.

**Recommended use in Engaging Me:** Adopt maturity as a note-level annotation in `gap_notes` for new entries (see dp_025, dp_026, dp_027 updates). Consider as a formal schema field in a future versioned schema update.

---

## CAT Entries Mapping to Existing Engaging Me Biases

| CAT Entry | CAT ID | Engaging Me Equivalent | Notes |
|-----------|--------|----------------------|-------|
| Loss Aversion | — | `bias_loss_aversion` | Direct match; CAT provides independent citation |
| Decision Fatigue | CAT-2022-050 | *Check bias catalog — may be gap* | High relevance to Deciding and Invested stages |
| FOMO (Fear of Missing Out) | — | Check bias catalog | Likely present; confirm ID |
| Scarcity | — | Check bias catalog | Likely present under urgency/scarcity framing |
| Reciprocity Norm | — | Partial overlap with `bias_social_proof` | CAT frames as obligation; Engaging Me frames as social evidence — distinct enough to note |
| Availability Heuristic | — | `rec1mQOkbN30aQmv1` | Direct match |
| Automation Bias | — | `recy5aWDVmI6bvy6C` | Direct match |

**DITF / FITD (Door-in-the-Face / Foot-in-the-Door):** These are influence *techniques* in CAT, mapping more cleanly to Engaging Me Tactics than Biases. Check tactics.json for equivalent entries.

---

## CAT Framing of the Three New Dark Patterns

### dp_025 — Emotional Vulnerability Exploitation
- **CAT layers:** Layer 8 exploit of emotional availability biases
- **CAT maturity:** In Common Use (holiday ad backlash documented both the practice and acknowledged industry awareness of harm)
- **CAT vocabulary value:** "Exploit" framing reinforces that this is a deliberate activation of a known vulnerability, not an incidental effect

### dp_026 — Consent Rerouting
- **CAT layers:** Layer 7–8 interaction — the algorithmic routing decision (Layer 7) exploits the compliance gap between item-level and category-level refusal (Layer 8); the settings labyrinth is a Layer 9 organizational choice
- **CAT maturity:** In Common Use
- **CAT vocabulary value:** "TTP" framing helps explain that item-level remediation while preserving category routing is not a fix — it's a different TTP serving the same exploit

### dp_027 — Incentive Signal Exploitation
- **CAT layers:** Layer 7 engineering choice (who controls the optimization signal) exploiting Layer 8 automation bias
- **CAT maturity:** Split — Well-Established for social media algorithmic systems; Observed in Wild for agentic AI (Moltbook data, arXiv:2602.13458)
- **CAT vocabulary value:** The split maturity across social media and agentic AI is significant and worth calling out in the paper — the mechanism is old, but the agentic application is new and less documented

---

## What Engaging Me Has That CAT Doesn't

- **Engagement journey mapping:** The 7 stages (Zero → Acting) give practitioners a "when does this happen" answer CAT doesn't provide
- **Design-forward framing:** CAT names attacks; Engaging Me names attacks AND their ethical counterparts (corrupts/inverts/amplifies relationship types; tactic-as-positive-counterpart)
- **Agentic AI specificity:** CAT treats AI as a Layer 7 target, not as a perpetuating actor; Engaging Me's agentic amplification notes are ahead of CAT here
- **Practitioner audience design guidance:** CAT is threat intelligence; Engaging Me is design ethics with actionable tactic guidance

---

## Philosophical Framing Distinction

CAT defines "threat actor" as *anyone not being completely transparent in their intentions.* This is broader than Engaging Me's operator/designer framing, and intentionally so — CAT treats opacity as the base condition for threat. Engaging Me takes a design ethics stance: it's not about actors, it's about patterns. Both framings are valid and serve different audiences. Worth noting in the paper to prevent conflation.

---

## Recommended Paper Citations

**Conceptual grounding section:** Cite CAT as an independently-developed framework whose V-E-T structure converges with the Engaging Me biases/tactics/dark-patterns architecture. Frame this convergence as external validation. Credit Sean [last name if available] as source contributor.

**Maturity framing:** When discussing why emerging agentic applications of established patterns warrant documentation, CAT's maturity taxonomy provides a useful vocabulary.

**Specific bias citations:** Where Engaging Me biases overlap with CAT-named entries (Loss Aversion, Decision Fatigue, etc.), CAT can serve as a secondary citation alongside primary cognitive science sources.

---

## Future Collaboration Note

The Engaging Me model's design-forward orientation and the CAT team's threat intelligence framing are complementary enough to warrant sharing findings. CAT may not have seen the engagement journey or agentic amplification framing; Engaging Me may benefit from CAT's cross-community visibility in security/cognition circles. Consider reaching out after the paper is published.

---

*Source: cognitiveattacktaxonomy.org | Contributed by Sean | Assessed April 28, 2026*
