# sefirot-resonant-cavity

Paper: **The Sefirot Graph as Resonant Cavity — Spectral Theory of a 10-Node Governance Architecture**

Spectral analysis of a specific 10-node, 22-edge graph (the sefirot graph) with Z2 pillar symmetry. Proves nine theorems covering Z2 parity decomposition, Perron-Frobenius concentration, bimodal structure, Z2-isospin isomorphism, cross-coupling rank, Goldstone drop-by-2 (discrete GMOR analogue), complement duality, unique maximum equal-density bisection, and optimal Daat coupling.

- 15 pages, `amsart` class, 9 theorems, 12 references
- Written by Hroar Thor Reynisson (ORCID [0009-0003-6518-121X](https://orcid.org/0009-0003-6518-121X))

## Contents

```
paper/
├── sefirot_resonant_cavity.tex     # LaTeX source (canonical)
├── sefirot_resonant_cavity.pdf     # compiled PDF (380 KB)
├── README.md                        # paper-local README (figure plan)
└── figures/                         # 10 figures (PDF for paper, PNG for web)
```

## Figures

All 10 figures are generated from reproducible Python scripts in the main
research repository at `docs/paper_resonant_cavity/figures/scripts/` and
ship as both PDF (paper-ready, vector) and PNG (web preview).

1. `sefirot_graph` — three-pillar layout with degree-sized nodes
2. `z2_decomposition` — even (7-dim) vs odd (3-dim) sectors
3. `pf_concentration` — top Laplacian eigenvector, 86.7% Tiferet
4. `breathing_mode` — Fiedler + top mode, side-by-side
5. `wave_vs_diffusion` — Yesod response under wave vs diffusion dynamics
6. `complement_hub` — complement graph with Daat now degree 10
7. `eigenvalue_pairing` — lambda(G) + lambda(complement) = 10
8. `bisection_landscape` — all 126 five-way partitions ranked
9. `daat_coupling_sweep` — PF concentration vs coupling weight w
10. `char_poly_factorization` — Z2 factorization into p_plus times p_minus

## Build

```bash
cd paper/
pdflatex sefirot_resonant_cavity.tex
bibtex sefirot_resonant_cavity || true
pdflatex sefirot_resonant_cavity.tex
pdflatex sefirot_resonant_cavity.tex
```

## Venue targets

J. Complex Networks (Oxford), SIAM J. Applied Math, Phys. Rev. E,
AI (Elsevier), AAMAS.

## Citation

See `CITATION.cff`. DOI to be minted via Zenodo once `v1.0.1` is cut with
Zenodo-GitHub integration enabled (v1.0.0 will not mint retroactively).

## License

Dual license:
- Code / scripts: AGPL-3.0 (see `LICENSE`)
- Paper / data / figures: CC BY-SA 4.0 (see `LICENSE-CC-BY-SA-4.0`)

## Links

- Zenodo: pending (blocked on user-side GitHub integration)
- arXiv: pending submission (math.SP or cs.MA)
- ORCID: [0009-0003-6518-121X](https://orcid.org/0009-0003-6518-121X)
