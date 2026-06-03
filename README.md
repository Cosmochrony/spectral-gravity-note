This repository contains the source of the **Spectral Gravity Presentation Note** Cosmochrony paper
[*The Spectral Gravity Sub-Programme — Presentation Note 4*](out/SpectralGravityNote.pdf).

This work is a **structured entry point** to the spectral gravity sub-programme of the
Cosmochrony corpus, not a summary of results. It maps the constituent papers, identifies
the internal phases, records the status of every result as proved, structural, numerical,
or open, and states the remaining open deliverables.

## Central Question

The emergent geometry sub-programme (Presentation Note 2) reconstructs the effective
Lorentzian metric $g^{\mu\nu} = 2\eta^{\mu\nu}$ as a forced output of the admissibility
structure of the non-injective projection $\Pi$.

> Why does the projective spectral entropy functional
> $\mathcal{S}_\Pi[g] = \tfrac{1}{2}\log\det' A_g$ produce the Einstein equations as its
> metric variation, and how is this dynamics completed causally and ultraviolet-wise?

The sub-programme establishes that the Einstein equations $G_{\mu\nu} = 8\pi G_N
T_{\mu\nu}^{(\Pi)}$ emerge as the infrared-dominant $a_2$ response of the renormalized
spectral entropy functional, not as a postulated dynamics. This note concerns the
**derivation** of gravitational dynamics in the matter-free IR; the gauge--gravity
stratification belongs to Presentation Note 8.

## Logical Chain

$\mathcal{S}_\Pi[g] = \tfrac{1}{2}\log\det' A_g
\;\Longrightarrow\;
\delta_g\mathcal{S}_\Pi \ni c_{\mathrm{EH}}\, G_{\mu\nu}
\;\Longrightarrow\;
G_{\mu\nu} = 8\pi G_N T_{\mu\nu}^{(\Pi)}
\;\Longrightarrow\;
\omega^2 = c^2 k^2 - \gamma \ell_{\mathrm{sp}}^2 k^4
\;\Longrightarrow\;
\sqrt{-\det(g + \ell_{\mathrm{sp}}^2 R)}.$

Four conceptually distinct stages:

1. **IR Einstein response** — the $a_2$ pole of the renormalized metric variation is
   infrared-dominant in $R\ell_{\mathrm{sp}}^2 \ll 1$ (Gravity 3.0).
2. **Spectral equilibrium** — the Einstein field equations as Euler--Lagrange of
   $\mathcal{S}_\Pi$ at fixed projected matter content, with no horizon or Rindler
   structure invoked (Thermodynamics).
3. **Causal completion** — Lorentzian Schwinger--Keldysh prescription, two
   transverse-traceless helicity-$\pm 2$ graviton modes, dispersion
   $\omega^2 = c^2 k^2 - \gamma \ell_{\mathrm{sp}}^2 k^4$ with $\gamma = 1/30$
   (Lorentz/CausalPropagation).
4. **UV completion** — the Eddington-inspired Born--Infeld action as the unique tensorial
   completion of the Einstein--Hilbert sector under conditions (C1)--(C5) and Hypothesis
   [H-ext] (BornInfeld + Gravity Theorem 1).

## Constituent Papers

| # | Paper | Stage | Local path |
|---|-------|-------|------------|
| 1 | **Gravity 3.0** (Beau2026h) — *Infrared Einstein Response from a Renormalized Spectral Entropy Functional* | IR Einstein response, induced $G_N \sim 16\pi^2 \ell_{\mathrm{sp}}^2$, BI tensorial uniqueness | [`../gravity/`](../gravity/) |
| 2 | **Thermodynamics** (Beau2026Thermodynamics) — local spectral first law, Einstein equation as spectral equilibrium | Spectral equilibrium | [`../thermodynamics/`](../thermodynamics/) |
| 3 | **Lorentz / CausalPropagation** (Beau2026i) — Lorentzian completion, gravitons, $k^4$ dispersion | Causal completion | [`../lorentz-paper/`](../lorentz-paper/) |
| 4 | **BornInfeld** (Beau2026c) — scalar BI uniqueness, parity involution $\chi \mapsto -\chi$ | UV completion | [`../born-infeld-paper/`](../born-infeld-paper/) |

## Status of Results

**Proved (unconditional):**
- Scalar BI uniqueness and parity involution (BornInfeld).
- Spectral carrier identification: $X = \ell_{\mathrm{sp}}^2 g^{-1}R$ (Gravity Lemma 3).
- Scalar BI reduction $h(\lambda) = \tfrac{1}{2}\log(1 + \lambda)$ (Gravity Lemma 2).

**Structural:**
- IR hierarchy and IR dominance of $G_{\mu\nu}$ (Gravity §4.5).
- Induced Newton constant $G_N \sim 16\pi^2 \ell_{\mathrm{sp}}^2$ (Gravity §5).
- Spectral multiplier field and first law (Thermodynamics §2--3).
- Einstein equation as spectral equilibrium (Thermodynamics Theorem 4.3).
- Lorentzian Schwinger--Keldysh kernel, two helicity-$\pm 2$ modes, $\gamma = 1/30$
  dispersion (Lorentz/CausalPropagation §2--3).

**Conditional on [H-ext]:**
- Tensorial BI uniqueness (Gravity Theorem 1, Lemma 1 only).

## Open Deliverables

1. **Analytical proof of [H-ext]** (admissible coherence extensivity) — promotes Gravity
   Theorem 1 to unconditional.
2. **Full Lorentzian Einstein equilibrium** — extend Thermodynamics Theorem 4.3 beyond
   Riemannian signature, integrating the Schwinger--Keldysh prescription.
3. **Coupled $G_{\mu\nu} = 8\pi G_N T_{\mu\nu}$ with matter** — pending the Fermionic
   Matter Sub-Programme (Note 6).

## Compilation

```bash
bash compile.sh
```

Produces `out/SpectralGravityNote.pdf`.

## Citation

To be assigned upon first Zenodo publication.
