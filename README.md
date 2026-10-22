This repository contains the source of the **Spectral Gravity Presentation Note** Cosmochrony paper
*The Spectral Gravity Sub-Programme (Presentation Note 4)*.

This work is a **structured entry point** to the spectral gravity sub-programme of the
Cosmochrony corpus, not a summary of results. It maps the constituent papers, records the status
of every result as proved, structural, conditional, or open, and states the remaining open
deliverables.

## Central Question

> Under which conditions does the projective spectral entropy functional
> $\mathcal{S}_\Pi[g] = \tfrac{1}{2}\log\det' A_g$ produce an Einstein sector as its metric
> variation, for a supplied Riemannian metric $g$?

The sub-programme separates the physical proper-time cutoff (power-sensitive terms
$a_0\Lambda^4$, $a_2\Lambda^2$) from zeta regularization (finite and logarithmic terms governed
by $a_4$), decomposes the renormalized metric variation into Einstein, cosmological,
higher-derivative, and non-local sectors, and states the conditions under which the Einstein term
dominates. The renormalized couplings, including the sign and value of Newton's constant, are
matching data, not predictions. Gravity emerging as a spectral response remains a structural
possibility, not an established result.

The metric is **supplied**. The emergent geometry sub-programme (Presentation Note 2) addresses
its reconstruction: under the unestablished spatial-limit hypothesis [H-L] and the open lifting
hypothesis [H-lift], Q5b extracts a rank-three co-metric, and a co-metric proportional to $\eta^{\mu\nu}$
holds only for a supplied rank-four extension satisfying the hypotheses of Q11 Corollary 6.1,
after rescaling $\tau$, with its overall scale free. Relating the supplied Riemannian metric to a
Lorentzian form needs a continuation that is not performed. No metric coefficient value is established.
The gauge dynamics ($a_4$ Yang--Mills response) belongs to Presentation Note 8.

## Logical Chain

$$\mathcal{S}_\Pi[g] = \tfrac{1}{2}\log\det' A_g
\;\Longrightarrow\;
\delta_g\mathcal{S}_\Pi^{\mathrm{ren}} \ni c_{\mathrm{EH}}^{\mathrm{ren}}\, G_{\mu\nu}
\;\Longrightarrow\;
G_{\mu\nu} + \Lambda_{\mathrm{ren}} g_{\mu\nu} = 8\pi G_N T_{\mu\nu}
\;\Longrightarrow\;
\omega^2 = |\mathbf{k}|^2
\;\Longrightarrow\;
\sqrt{-\det(g + \ell_{\mathrm{sp}}^2 R)} \in \{\Phi_a\}$$

Four conceptually distinct stages:

1. **Decomposition and conditional infrared dominance** (Gravity): the Einstein term dominates
   locally, by power counting, when the matched Einstein coefficient is non-zero and $R L_4^2 \ll 1$, with $L_4^2 = |\beta^{\mathrm{ren}}/c_{\mathrm{EH}}^{\mathrm{ren}}|$.
   One minimal scalar contributes $\Delta c_{\mathrm{EH}} = -\Lambda^2/[12(4\pi)^2]$; the finite
   renormalized value, its sign, and $G_N > 0$ require a matching condition and the complete operator
   content.
2. **Conditional Einstein--matter coupling** (Thermodynamics): given supplied renormalized
   coefficients and a projected matter functional $W_\Pi[g, \psi]$, stationarity of
   $\Gamma_\Pi = \mathcal{S}_\Pi^{\mathrm{ren}} - W_\Pi$ yields
   $G_{\mu\nu} + \Lambda_{\mathrm{ren}} g_{\mu\nu} = 8\pi G_N T_{\mu\nu}$ on the Euclidean section, at
   leading local infrared order.
   The heat-kernel scale $u = -\partial_t \log K$ is an eigenvalue scale, not a temperature, so no
   local first law follows from the heat kernel alone.
3. **Lorentzian truncation** (Lorentz/CausalPropagation): on the posited local four-derivative
   transverse-traceless kernel $\Box(c_{\mathrm{EH}} + \beta\Box)$, the massless branch is exactly
   luminal, $\omega^2 = |\mathbf{k}|^2$, beside a massive spin-two pole of opposite residue. No
   quartic dispersion and no observational bound on $\ell_{\mathrm{sp}}$ follow; a Lorentzian
   spectral action requires an in-in construction, which is open.
4. **Ultraviolet completion: admissibility without uniqueness** (Gravity, BornInfeld): under
   conditions (C1)--(C5) and Hypothesis [H-ext], the determinantal Born--Infeld density is an
   admissible member of the family $\Phi(X) = \exp\sum_i h(\lambda_i)$ on the mixed Ricci carrier $X$, which
   the saturation condition applied to $X$ selects, and the explicit family
   $\Phi_a(X) = \sqrt{\det(I+X)}\,e^{a\,\mathrm{tr}X^2}$ shows that it is not uniquely selected.

## Constituent Papers

| # | Paper | Stage | Local path |
|---|-------|-------|------------|
| 1 | **Gravity** (Beau2026h) — *Conditions for an Infrared Einstein Sector from Spectral Geometry* | Scheme separation, infrared decomposition, matching status, classification of the tensorial completions | [`../gravity/`](../gravity/README.md) |
| 2 | **Thermodynamics** (Beau2026Thermodynamics) — *Einstein–Matter Coupling from Spectral Stationarity: A Conditional Variational Result and the Open Thermodynamic Bridge* | Conditional Einstein–matter coupling | [`../thermodynamics/`](../thermodynamics/README.md) |
| 3 | **Lorentz / CausalPropagation** (Beau2026i) — *No Quartic Graviton Dispersion from the Local Covariant Four-Derivative Truncation* | Lorentzian truncation | [`../lorentz-paper/`](../lorentz-paper/README.md) |
| 4 | **BornInfeld** (Beau2026c) — *Bounded Relational Capacity and Its Conditional Continuum Dynamics* | Capacity axiom [A-cap], Born–Infeld saturation candidate | [`../born-infeld-paper/`](../born-infeld-paper/README.md) |

## Status of Results

**Proved (given stated inputs):**
- Scheme separation: the proper-time cutoff carries $a_0\Lambda^4$ and $a_2\Lambda^2$, zeta
  regularization the finite and logarithmic $a_4$ terms (Gravity).
- One-scalar cutoff contribution $\Delta c_{\mathrm{EH}} = -\Lambda^2/[12(4\pi)^2]$ (Gravity).
- Spectral carrier family $Y_\alpha = \tfrac{t}{d}I + X_0/(1-\alpha d)$, $\alpha \neq 1/d$, for carriers linear in
  the curvature, of two-derivative order and with a spectrum that is not a multiple of the identity (with
  $t = \mathrm{tr}\,X$ and $X_0$ the traceless part of $X = \ell_{\mathrm{sp}}^2 g^{-1}R$): all give the same linear
  term, second-order data determine at most $|1-\alpha d|$, leaving the pair $\{\alpha, 2/d-\alpha\}$, and the
  carriers differ in their saturation boundary; within this classification $\alpha$ is free, and the saturation
  condition applied as stated to $X$ selects $\alpha = 0$ (Gravity, Theorem 1). The constraints on the sector
  function, whence non-uniqueness via $\Phi_a$ (Gravity).
- Dimensional status of the heat-kernel scale: an eigenvalue scale, not a temperature
  (Thermodynamics).
- Factorization of the posited transverse-traceless kernel: exactly luminal massless branch,
  opposite-residue massive spin-two pole (Lorentz/CausalPropagation).

**Structural and conditional:**
- Local infrared dominance of $G_{\mu\nu}$ for a non-zero matched Einstein coefficient and $R L_4^2 \ll 1$, by
  power counting, conditional on supplied coefficients, with no general bound on the non-local terms (Gravity).
- Conditional Einstein--matter coupling on the Euclidean section, at leading local infrared order
  (Thermodynamics).
- Admissibility, without unique selection, of the Born--Infeld completion, conditional on [H-ext]
  (Gravity).
- Capacity axiom [A-cap] and Born--Infeld saturation candidate (BornInfeld).

**Interpretive:**
- The stratification $a_2 \to$ gravity, $a_4 \to$ gauge is an organising reading shared with
  Presentation Note 8, not a theorem.

## Open Deliverables

1. **Matching principle for the renormalized couplings**: the sign and value of
   $c_{\mathrm{EH}}^{\mathrm{ren}}$, hence $G_N$.
2. **Analytical proof of [H-ext] and a selection principle for the completion.**
3. **In-in Lorentzian spectral action and Lorentzian stationarity.**
4. **Coupled field equations with matter**, pending the Fermionic Matter Sub-Programme (Note 6).

The emergent reading of the metric needs [H-L], [H-lift], a rank-four extension of the rank-three
co-metric of Q5b that no source constructs, a continuation from Riemannian signature that is not
performed, and data fixing the metric coefficients, which no source supplies.

## Compilation

```bash
bash compile.sh
```

Produces `out/SpectralGravityNote.pdf`.

## Citation

Concept DOI: [10.5281/zenodo.20533351](https://doi.org/10.5281/zenodo.20533351).
