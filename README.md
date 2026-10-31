# On Keeping Humans Meaningfully in the Loop of AI Agents

A critical review and research agenda responding to **Mitchell, Ghosh & Passi,
_"AI Agents Push Humans Out of the Loop"_**.

**Author:** Ahmet Selim Fedakar

## What this is

A scholarly response paper. It (1) reconstructs the argument of the target
position paper, (2) situates it in the human–automation interaction literature
(from Bainbridge's *ironies of automation* through meaningful human control),
(3) critically evaluates how well its central claims are supported, and (4)
proposes a concrete, testable research agenda on oversight degradation in
agentic AI systems.

It is written as a LaTeX preprint intended for public release.

## Repository layout

```
paper/
  main.tex         # the paper
  references.bib   # bibliography (entries get verified by the research pass)
  figures/         # figures
notes/             # raw research synthesis, claim ledger, source list
```

## Building the PDF

```bash
cd paper
pdflatex main && bibtex main && pdflatex main && pdflatex main
```

Requires a TeX distribution (e.g. MacTeX / TeX Live).

## Status

- [ ] Deep-research synthesis landed
- [ ] Target paper verified (arXiv id, venue, exact claims)
- [ ] Bibliography fields verified
- [ ] Sections drafted from synthesis
- [ ] First full draft
- [ ] Review pass

> `\todo{...}` markers in `main.tex` flag everything still to be sourced. The
> `notes/` directory holds the research synthesis each section is drawn from.

## Provenance & integrity

Every non-obvious claim is tied to a source in `notes/claim-ledger.md`, with a
confidence level. Claims that could not be independently verified are flagged
rather than dropped. Bibliography entries marked `UNVERIFIED` must have their
fields confirmed before the final PDF.

## License

Suggested (pick before publishing): **CC BY 4.0** for the paper text and
**MIT** for any code. No license file is committed yet.
