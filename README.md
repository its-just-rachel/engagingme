# Engaging Me — Engagement Ethics Benchmark for Agentic AI Design

**Author:** Rachel Weatherly  
**Venture:** Engaging Me  
**Status:** Working paper (pre-publication)

---

## Overview

This repository contains the data model and working paper for the *Engagement Ethics Benchmark for Agentic AI Design* — a practitioner framework for identifying and countering manipulative engagement patterns in AI systems.

The framework maps cognitive biases, ethical counter-tactics, and dark patterns into a relational data model designed to support product designers, UX researchers, and AI ethics practitioners.

---

## Repository Structure

```
/data/
  biases.json          — 54 cognitive biases with academic citations
  tactics.json         — 82 ethical counter-tactics
  dark_patterns.json   — 24 dark patterns with attribution categories
  stages.json          — 7 engagement stages
  groups.json          — 10 tactic groups
  action_types.json    — 4 action type classifications
  action_needed.json   — Flags for model items needing review

Engagement Ethics Benchmark — Full Draft.md     — Full white paper (working draft)
Engagement Ethics Benchmark — Full Draft.docx   — Word version for collaborative review
Literature Grounding & Attribution Audit.md     — Source verification and attribution notes
Acknowledgments.md                              — Contributor acknowledgments and AI disclosure
```

---

## Data Model

The model is relational: tactics link to biases, stages, and groups via ID references. All cross-references are validated to be bidirectional and consistent.

**Model counts (as of April 2026):**
- 82 tactics
- 54 cognitive biases
- 24 dark patterns
- 7 engagement stages
- 10 tactic groups

---

## Access

This is a public repository for transparency and academic access. The working paper is shared here as a pre-publication draft.

To request collaboration access or provide feedback, contact: **rachel@engaging.me**

For citation of the framework or data model prior to formal publication, please contact the author directly.

---

## Attribution

Dark patterns in this framework are attributed across three categories:
- **(A) Established** — Drawn from existing academic taxonomies (Brignull, Mathur et al., Gray et al., Bösch et al., DarkBench)
- **(B) Synthesized** — Engaging Me application of established concepts to agentic AI contexts
- **(C) Original** — Novel patterns identified through the Engaging Me research process

See `Literature Grounding & Attribution Audit.md` for full sourcing detail.

---

## License

© 2026 Rachel Weatherly / Engaging Me. All rights reserved.

This work is shared publicly for academic transparency and peer review. Reproduction or derivative use requires written permission from the author.
