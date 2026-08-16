# Orchestrator Engine V6

This is the **paper repository** for *"Orchestrator Engine V6: A Deterministic, Self-Healing
State Machine Architecture for Enterprise LLM Intent Routing"*.

- **arXiv preprint**: [arXiv:XXXX.XXXXX](https://arxiv.org/abs/XXXX.XXXXX) *(added on submission)*
- **Zenodo archive / DOI**: [10.5281/zenodo.XXXXXXX](https://doi.org/10.5281/zenodo.XXXXXXX) *(minted on first GitHub Release)*
- **Code representation**: the [OSMv6 Orchestrator Engine](https://github.com/agentic-framework-skills/OSMv6)
  in the [agentic-framework-skills](https://github.com/agentic-framework-skills) org.

---

## Abstract

> Large Language Model (LLM) agents deployed in enterprise environments face critical failures
> regarding stochastic non-determinism, state drift during asynchronous operations, and
> susceptibility to graph poisoning via untrusted external tool outputs. In this paper, we
> present **Orchestrator Engine V6**, a unified state-machine control plane combining
> deterministic graph routing, additive sentiment scaling, stateless horizon persistence, and
> zero-trust asynchronous healing. V6 guarantees $0.0\%$ hallucination on known execution paths
> while bounding compute latency to $\mathcal{O}(1)$ for exact matches and $\mathcal{O}(K)$ for
> indexed edge lookups. We formalize the mathematical convergence of bounded reinforcement weight
> updates under asymmetric decay and establish security guarantees for asynchronous external graph
> mutations.

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
@article{Machuca2026osm,
  author    = {Machuca, Jean},
  title     = {Orchestrator Engine {V6}: A Deterministic, Self-Healing State Machine Architecture for Enterprise {LLM} Intent Routing},
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

The paper's title block additionally credits the *Autonomous AI Systems Research Group*
(`research@orchestrator.ai`).
