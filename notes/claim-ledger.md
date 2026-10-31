# Claim ledger

Every non-obvious claim used in the paper, with its source and confidence. Derived from the
deep-research pass (24 sources fetched, 117 claims extracted, 25 adversarially verified,
21 confirmed / 4 killed). Verification votes are shown as "N-M" (refutes-for : against).

## Confidence levels
- **A** — primary source read directly, claim explicit in it (research vote 3-0).
- **B** — corroborated but with a minor paraphrase/attribution nuance (vote 2-1), or
  well-established background not independently re-fetched this pass.
- **C** — inferred/extrapolated; flagged as the author's interpretation.
- **D** — contested; sources disagree, present both sides.

| # | Claim | Source(s) | Conf | Used in § |
|---|-------|-----------|------|-----------|
| 1 | Target paper = "AI Agents Push Humans Out of the Loop", arXiv 2608.23642 (v1 24 Aug 2026, v3 6 Sep 2026; cs.AI/cs.HC), NeurIPS position paper; Mitchell & Ghosh (HF), Passi (Data & Society) | arxiv.org/abs/2608.23642; datasociety.net; evijit.io | A (3-0) | 2.1 |
| 2 | Central thesis: current dev/deployment doesn't just impede oversight — contributes to its degradation; capacities oversight needs are degraded by extended AI use (partly "passively incentivized") | arXiv 2608.23642 abstract | A (3-0) | 2.2 |
| 3 | Grounds argument in Bainbridge 1983; §4 "The irony of automation", §4.5 "oversight degrades the overseer" (verbatim) | arXiv 2608.23642 §4 | A (3-0) | 2.3, 3.1 |
| 4 | Prescriptive core = "cognitive scaffolding", two-stage: dev affordances (strategic friction, decision design, behavioral monitoring) + deployment protocols (trainings, role design, audits); six goals × mechanisms table; overseer needs = equal to capability | arXiv 2608.23642; Table 1/Appendix Table 2 | A (3-0) | 2.4 |
| 5 | Traditional safeguards (approval prompts) work only if user can recognize mistake & intervene before cascade; agents violate via output volume/speed → "approval fatigue" | datasociety.net; arXiv 2608.23642 | A (3-0) | 2.2 |
| 6 | Companion D&S primer "The Oversight Fallacy" (Passi & Ranjit Singh, 29 Jul 2026), comp-bio lab fieldwork, four components: knowledge/observation/control/intervention | datasociety.net; D&S PDF | A (3-0) | 2.1 |
| 7 | Lineage: Parasuraman & Riley 1997 (~8018 GS), Parasuraman/Sheridan/Wickens 2000 (~7286 GS, levels-of-automation), Parasuraman & Manzey 2010 (~3043 GS); 2000 builds on Sheridan & Verplank 1978 10-level scale | scholar.google (Parasuraman); SAGE; ResearchGate | A (3-0); counts are GS, directional | 3.2, 3.3 |
| 8 | Complacency & automation bias = overlapping manifestations of same effect; attentional reallocation central (but NOT sole — also "active discounting" decision bias) | Parasuraman & Manzey 2010 | A (3-0), precision flag | 3.3 |
| 9 | Dhanorkar, Passi & Vorvoreanu 2026 (arXiv 2606.05391, FAccT/CSCW): 17 devs weekly agent use, four oversight forms (a priori control, co-planning, real-time monitoring, post hoc review); proactive not just reactive | arXiv 2606.05391 | A (3-0) | 3.7, 4.1 |
| 10 | Same study: devs settle for "efficient, not perfect" oversight; gap vs frameworks (EU AI Act, EC trustworthy-AI) that assume feasibility | arXiv 2606.05391 | A (3-0) | 3.7 |
| 11 | Recchia et al. (arXiv 2507.19486, AAAI): independent research to check AI made people MORE confident even when wrong, even with financial incentives — confirmation bias defeats scalable oversight | arXiv 2507.19486; ojs.aaai.org | A (3-0) | 3.7, 4.3 |
| 12 | Faas et al. (arXiv 2510.19512): work-design psychology, motivation & meaningfulness matter; four co-design workshops; four requirements; SMART model | arXiv 2510.19512 | A (3-0) | 3.7 |
| 13 | de la Chica Rodriguez et al. (arXiv 2607.15944, PHP-AIO): positions as pre-decision filter before deployment-commitment; distinct from NIST/EU AI Act/HITL | arXiv 2607.15944 | **B (2-1)**; self-positioning contestable | 3.7 |
| 14 | Broader debate incl. "fictional human oversight" (arXiv 2404.04059), NIST cautions, 35-study review (anti-bias interventions ineffective), intervention success 9-26% | arXiv 2404.04059; datasociety.net | **B** (corroborating context, not independently voted) — re-verify figures before citing | 3.6, 4.3 |

## REFUTED — do NOT state as the position paper's content (killed in verification)
- Paper does **not** present a clean four-mechanism named list (approval fatigue / automation bias / loss of SA / skill atrophy). (vote 1-2)
- No "twelve design considerations via SMART" scheme in the position paper (that's Faas et al., and even there the 12-item operationalization failed 0-3).
- PHP-AIO five-gate / four-risk-category / four-outcome internal structure. (0-3)
- PHP-AIO's claimed grounding of risk categories in human-factors/sociotechnical literature. (0-3)

## KEY EVIDENCE ASYMMETRY (the paper's title claim)
Descriptive lineage (automation bias, complacency, ironies of automation) = strongly
empirically grounded. Applied claim that extended AI-agent use specifically causes skill
atrophy in knowledge/software work = largely ASSERTED by analogy, NOT shown by direct
longitudinal measurement. Companion works (2606.05391, 2507.19486) show oversight is hard
and verification can backfire, but do NOT establish AI-induced deskilling as a measured
effect. → This is the central open research problem (paper §4.2, §5 Direction 1).

## Attribution guard
Only 2608.23642 (+ the two Data & Society companions) are Mitchell/Ghosh/Passi. The four
2025-26 arXiv papers (2606.05391, 2510.19512, 2507.19486, 2607.15944) are DISTINCT related
works — cite to their own sources, never attribute to the position paper.
