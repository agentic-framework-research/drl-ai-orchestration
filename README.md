# Deterministic Reinforcement Learning and AI Orchestration

This is the **paper repository** for *"Deterministic Reinforcement Learning and AI
Orchestration"* by Jean Machuca (CognitiveOS-Labs).

- **arXiv preprint**: [arXiv:XXXX.XXXXX](https://arxiv.org/abs/XXXX.XXXXX) *(added on submission)*
- **Zenodo archive / DOI**: [10.5281/zenodo.XXXXXXX](https://doi.org/10.5281/zenodo.XXXXXXX) *(minted on first GitHub Release)*
- **Code representation**: the [OSMv6 Orchestrator Engine](https://github.com/agentic-framework-skills/OSMv6)
  in the [agentic-framework-skills](https://github.com/agentic-framework-skills) org.

---

## Abstract

> _Placeholder._ Replace this section with the paper's abstract.

---

## Repository structure

```text
drl-ai-orchestration/
├── paper/                 # arXiv-ready LaTeX source
│   ├── main.tex           # main document
│   ├── references.bib     # BibTeX bibliography source
│   └── figures/           # figures
├── paper.pdf              # compiled PDF (built by CI)
├── CITATION.cff           # citation metadata (ORCID, DOI, related code)
├── LICENSE                # MIT (source code, LaTeX, figures, CI)
├── LICENSE_PAPER          # CC-BY-4.0 (paper text/content)
├── README.md              # this file
└── .github/workflows/
    ├── tex.yml            # build PDF + arxiv tarball on PRs / pushes
    └── release.yml        # SemVer tag -> GitHub Release (for Zenodo DOI)
```

## Citing

Prefer the **Zenodo DOI** of an archived release; a preprint is also on **arXiv**.
Citation metadata lives in [`CITATION.cff`](CITATION.cff).

```bibtex
@article{Machuca2026drl,
  author    = {Machuca, Jean},
  title     = {Deterministic Reinforcement Learning and {AI} Orchestration},
  year      = {2026},
  doi       = {10.5281/zenodo.XXXXXXX}
}
```

## Build

The PDF is built automatically by GitHub Actions (`xelatex` + `bibtex`) and attached to pull
requests and tagged releases. To build locally:

```bash
cd paper
xelatex main.tex
bibtex main
xelatex main.tex
xelatex main.tex
```

## License

- **Code, LaTeX source, figures, CI** — [MIT](LICENSE) © 2026 Jean Machuca.
- **Paper text/content** — [CC-BY-4.0](LICENSE_PAPER) © 2026 Jean Machuca, CognitiveOS-Labs.

## Author

**Jean Machuca** — [GitHub @jeanmachuca](https://github.com/jeanmachuca) ·
[ORCID 0009-0004-9924-2911](https://orcid.org/0009-0004-9924-2911) ·
[Sponsor on GitHub Sponsors](https://github.com/sponsors/jeanmachuca)
