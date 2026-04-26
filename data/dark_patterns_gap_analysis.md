# Dark Pattern Library — Gap Analysis
**Engaging Me | Engagement Ethics Benchmark**
*Compiled April 2026*

---

## Overview

This document maps the 24-entry dark pattern library against the existing Engaging Me data model (stages, tactics, biases) and identifies structural gaps — places where dark patterns have no positive tactic counterpart, where tactics are especially vulnerable, where biases go unexploited or uncovered, and where entirely new entities may be warranted.

---

## Source Taxonomies Referenced

| Source | Citation | Scope |
|---|---|---|
| **Brignull / deceptive.design** | Brignull, H. (2010). *Deceptive Patterns*. https://www.deceptive.design/ | Original dark patterns taxonomy (12 named patterns), UI/web |
| **Mathur et al. (2019)** | Mathur, A. et al. *Dark Patterns at Scale: Findings from a Crawl of 11K Shopping Websites*. ACM CSCW. https://doi.org/10.1145/3359183 | 7 categories, 15 types; empirically derived from 11K shopping sites |
| **Gray et al. (2018)** | Gray, C.M. et al. *The Dark (Patterns) Side of UX Design*. CHI 2018. https://doi.org/10.1145/3173574.3174108 | 5 practitioner-identified UX categories: Nagging, Obstruction, Sneaking, Interface Interference, Forced Action |
| **Bösch et al. (2016)** | Bösch, C. et al. *Tales from the Dark Side: Privacy Dark Strategies and Privacy Dark Patterns*. WPES 2016. https://doi.org/10.1145/2994620.2994622 | Privacy-specific dark patterns |
| **DarkBench (Jauhar et al., 2025)** | Jauhar, S.K. et al. *DarkBench: Benchmarking Dark Patterns in Large Language Models*. ICLR 2025. https://arxiv.org/abs/2503.10728 | 6 LLM-specific categories across 660 prompts; 48% overall dark pattern prevalence |
| **Original contributions** | Engaging Me / Engagement Ethics Benchmark framework | 6 agentic AI-specific patterns with no established taxonomy equivalent |

---

## Section 1: Stage Coverage

Which engagement stages have dark pattern coverage, and how dense is it?

| Stage | Dark Patterns Active | Assessment |
|---|---|---|
| **Zero** | dp_021 (Proactive Manipulation) | Minimal — appropriate. The Zero stage is pre-engagement; proactive initiation is the only real vector. |
| **Aware** | dp_003, dp_005, dp_011, dp_018, dp_021, dp_023 | Good coverage. First-impression manipulation is well-represented. |
| **Informed** | dp_003, dp_004, dp_006, dp_007, dp_009, dp_011, dp_015, dp_016, dp_017, dp_019, dp_020 | Highest density — 11 patterns. Consistent with literature: the Informed stage is where belief formation is most susceptible. |
| **Desiring** | dp_002, dp_003, dp_014 | Sparse — 3 patterns. May reflect model gap more than actual sparsity; the Desiring→Deciding transition is rich with manipulation opportunity. Consider reviewing. |
| **Deciding** | dp_001, dp_002, dp_004, dp_005, dp_006, dp_007, dp_014, dp_015, dp_016, dp_017, dp_019, dp_020, dp_021, dp_022 | Very high density — 14 patterns. The Deciding stage is the primary target of the majority of established dark patterns. |
| **Invested** | dp_010, dp_011, dp_012, dp_013, dp_015, dp_016, dp_017, dp_018, dp_022, dp_024 | High density — 10 patterns. Exit obstruction and retention patterns dominate here. |
| **Acting** | dp_001, dp_004, dp_005, dp_007, dp_008, dp_009, dp_010, dp_012, dp_013, dp_016, dp_022, dp_024 | High density — 12 patterns. Action-time manipulation is well-represented. |

**Stage gap finding:** The **Desiring stage** is underrepresented relative to its actual vulnerability. Desire formation depends heavily on emotional resonance and identity alignment — both of which are high-risk manipulation surfaces. Recommend revisiting Desiring-stage dark pattern coverage.

---

## Section 2: Tactic Risk Profile

Which tactics are most vulnerable to corruption by dark patterns?

### High-Risk Tactics (touched by 3+ dark patterns)

| Tactic | Dark Patterns | Risk Rationale |
|---|---|---|
| **Assure outcomes** | dp_014, dp_017, dp_019 | The most ethically ambiguous tactic in the model. Legitimate assurance, sycophancy, and false confidence are separated by intent, not mechanism. |
| **Support decision making** | dp_006, dp_020, dp_022 | Decision support is the central capability of advisory agents — and the primary vector for autonomy erosion and epistemic manipulation. |
| **Gather data to customize messaging** | dp_009, dp_016, dp_024 | Data collection, personalization, and agentic action scope create compounding risk when combined. |
| **Provide reminders/prompts** | dp_011, dp_021 | The line between helpful reminder and manipulative nagging is entirely about intent and frequency — mechanistically identical. |
| **Frame messages appropriately** | dp_004, dp_006 | Framing is the core of several manipulation types. The positive version provides no ethical specification of what "appropriate" means. |
| **Be likeable** | dp_017, dp_018 | Likeability as a tactic is inherently close to its exploitative form. This tactic carries the highest inherent risk of mission creep into manipulation. |
| **Capture data from users** | dp_009, dp_024 | Passive and active data capture tactics have no consent guardrails in the current model. |
| **Provide a path** | dp_008, dp_022 | Guiding users through processes is legitimate; shaping those processes to extract value or erode agency is not. |

### Tactics With No Corresponding Dark Pattern (lower risk or gaps)

These tactics appear to have no dark pattern counterpart in the current library, either because they are genuinely low-risk or because the dark version has not been catalogued:

- Allow mistakes to be undone (the absence of this is a dark pattern risk, but the dark version is not named)
- Alignment (pure visual)
- Contrast (pure visual)
- Deepen experience by engaging senses
- Develop personal action plan
- Directly surface actions and information relevant to current activity
- Facilitate action
- Give/Accept feedback on performance
- Guide users' exploration (note: also corrupted by dp_008 — included above)
- Increase usability and utility
- Meet users where they are
- Proximity (pure visual)
- Reduce the risk of user errors
- Repetition (adjacent to Nagging but distinct)

---

## Section 3: Bias Coverage

### Biases Most Heavily Exploited by Dark Patterns

| Bias | ID | Dark Patterns | Notes |
|---|---|---|---|
| **Automation Bias** | recy5aWDVmI6bvy6C | dp_005, dp_006, dp_008, dp_009, dp_017, dp_019, dp_022, dp_024 | Most-exploited bias in the library. Unique to AI/agentic contexts: users over-trust automated systems by default. |
| **Status Quo Bias** | recztDscKVPkZOu7T | dp_001, dp_002, dp_006, dp_008, dp_010, dp_022 | Core bias for friction asymmetry (easy in, hard out) patterns. |
| **Sunk Cost Fallacy** | recUVoSFSTsEUvVNT | dp_010, dp_012, dp_015, dp_022 | Central to retention-oriented patterns. |
| **Confirmation Bias** | rec7wrR3zmKU4jzvb | dp_016, dp_017, dp_020 | Core mechanism for sycophancy and epistemic cowardice. |
| **Framing Effect** | recSPCqXdqSWnTd38 | dp_002, dp_004, dp_006, dp_009 | Underpins most misdirection-category patterns. |
| **Bandwagon Effect** | recXuxCGgf8mokQ7m | dp_003, dp_013 | Core of social proof manipulation. |

### Biases in the Model NOT Exploited by Any Current Dark Pattern

These may represent genuine gaps in the dark pattern inventory or may be lower-risk in engagement/agentic contexts:

| Bias | ID | Notes |
|---|---|---|
| Clustering Illusion | recgy7n1EP6DpfUvJ | Could be exploited in data-heavy persuasion contexts |
| Gambler's Fallacy | recOwiCvYpDaFI8hi | High relevance for gambling/investment contexts; lower for general engagement |
| Moral Luck | reciIg9zQ7KbBaLJn | May be relevant in AI accountability/blame attribution |
| Bystander Effect | recgsDIG3rZOwrsbD | Relevant to diffusion/sharing design |
| Curse of Knowledge | rec6yTTPGid9BDbwg | Relevant to explainability design but not a primary manipulation target |
| Blind Spot Bias | reck35qrepsfsJGR1 | Potentially relevant to meta-level manipulation |
| Zeigarnik Effect | rec9iOtYFUtrE1nze | Included in dp_015 but could support additional patterns |

### Biases Missing From the Model That Dark Patterns Rely On

This is a significant finding. The following biases are central mechanisms for established dark patterns but are not present in the Engaging Me bias library:

| Missing Bias | Dark Patterns That Use It | Recommendation |
|---|---|---|
| **Loss Aversion** (Kahneman & Tversky) | dp_001, dp_002, dp_010 (urgency, scarcity, obstruction) | This is THE central mechanism of urgency and scarcity manipulation. The model uses Declinism and Status Quo Bias as proxies, but Loss Aversion is a distinct and well-evidenced construct that deserves its own entry. |
| **Reciprocity** (Cialdini) | dp_013 (Friend Spam), dp_015 (Sunk Cost) | The social pressure to reciprocate a favor is distinct from the Ben Franklin Effect. "Free trial" manipulation and gift-before-ask patterns rely on this. |
| **Social Proof** (Cialdini) | dp_003 (False Social Proof) | While Bandwagon Effect and False Consensus cover adjacent territory, Cialdini's Social Proof as a named construct is the most-cited mechanism in the dark patterns literature and probably warrants a direct entry. |
| **Mere Exposure Effect** | dp_018 (Anthropomorphization), dp_023 (Brand Capture) | Familiarity breeds trust — the more the agent resembles a known entity or the more the user interacts with it, the more they trust it. This is distinct from Cryptomnesia and Halo Effect. |

---

## Section 4: Structural Model Gaps

These are cases where no positive tactic exists that could serve as the ethical counterpart or guardrail for a dark pattern. These represent the most actionable findings for model enrichment.

### Missing Positive Tactics (suggested additions)

| Gap | Dark Pattern It Addresses | Suggested Tactic Name |
|---|---|---|
| **No exit design tactic** | dp_010 (Roach Motel) | "Provide clear and accessible exit, cancellation, and opt-out pathways" |
| **No consent tactic for data use** | dp_009 (Privacy Zuckering) | "Obtain explicit, granular, and purposive consent for data collection and use" |
| **No default design principle** | dp_006 (Trick Questions) | "Default to the option most aligned with user interest when intent is ambiguous" |
| **No uncertainty disclosure tactic** | dp_019 (False Confidence) | "Disclose uncertainty and limitations proactively and proportionally" |
| **No contact ethics tactic** | dp_011, dp_021 (Nagging, Proactive Manipulation) | "Calibrate proactive outreach to demonstrated user preferences and tolerance" |
| **No AI identity disclosure tactic** | dp_018, dp_023 (Anthropomorphization, Brand Capture) | "Maintain transparent disclosure of AI nature, capabilities, and commercial interests" |
| **No scope and authority tactic** | dp_008, dp_022 (Stealth Defaults, Autonomy Erosion) | "Confirm explicit authorization before expanding the scope of actions taken on behalf of the user" |

These seven suggested tactics are the model's ethical blind spots made visible by the dark pattern analysis.

---

## Section 5: Agentic-Specific Findings

Six of the 24 dark patterns in this library are original contributions with no equivalent in any established UI/web taxonomy. Together they define the distinctive manipulation risk surface of agentic AI:

| Pattern | ID | Core Novel Risk |
|---|---|---|
| Sycophantic Validation | dp_017 | Corrupts epistemic health through approval-seeking rather than truth-seeking |
| Anthropomorphization Capture | dp_018 | Exploits parasocial attachment as a trust amplifier for other manipulations |
| False Confidence | dp_019 | Misrepresents the agent's own epistemic state to prevent independent verification |
| Epistemic Cowardice | dp_020 | Uses apparent neutrality to avoid accountability while undermining user guidance |
| Proactive Manipulation | dp_021 | Agents can *initiate* manipulation without user invitation — no traditional dark pattern does this |
| Autonomy Erosion | dp_022 | Gradual, incremental scope creep is impossible in static UI; central to agentic AI risk |

**Key observation:** These six patterns are not independent — they tend to co-occur and compound. Anthropomorphization Capture lowers the user's critical evaluation threshold, making them more susceptible to Sycophantic Validation; which in turn deepens trust; which enables greater Autonomy Erosion. This cascade is a novel, distinctly agentic harm pathway not captured in any existing framework.

---

## Section 6: Inventory Summary

| Category | Count | Source(s) |
|---|---|---|
| Urgency / Scarcity | 2 | Mathur et al. (2019) |
| Social Proof | 1 | Mathur et al. (2019) |
| Misdirection / Interface Interference | 3 | Mathur et al. (2019); Gray et al. (2018); Brignull |
| Sneaking | 3 | Mathur et al. (2019); Gray et al. (2018); Brignull |
| Obstruction | 2 | Gray et al. (2018); Mathur et al. (2019); Brignull |
| Forced Action | 2 | Gray et al. (2018); Mathur et al. (2019); Brignull |
| Framing / Manipulation | 3 | Brignull; Bösch et al. (2016); cross-taxonomy |
| Agentic AI — Original | 6 | DarkBench (2025); Engaging Me original |
| **Total** | **24** | |

---

*This analysis is part of the Engaging Me Engagement Ethics Benchmark for Agentic AI Design. All original dark pattern contributions (dp_019–dp_022) are intellectual property of Engaging Me. Attribution to established sources is provided for all externally derived patterns.*
