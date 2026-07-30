---
id: 1f7f4f64835a
type: definition
references:
  - "R. Palais & S. Smale, A generalized Morse theory (1964); standard in Struwe, Variational Methods"
---

# Definition — Palais–Smale condition

The compactness a functional needs for critical points to exist:
sequences that almost minimize and almost stop changing must actually
subconverge — no escaping to infinity or to a bubble.

## Statement

> [!definition] Palais–Smale condition
> A $C^1$ functional $\mathcal{F} : X \to \mathbb{R}$ on a Banach manifold satisfies the *Palais–Smale condition* (PS) if every sequence $\{u_k\} \subset X$ with $\mathcal{F}(u_k)$ bounded and $d\mathcal{F}(u_k) \to 0$ (a *Palais–Smale sequence*) has a convergent subsequence in $X$.

## Notes

> [!note]- Notes (click to expand)
> - (PS) is exactly what turns "there is an almost-critical sequence" into "there is a [[def-critical-point|critical point]]": the limit of a PS sequence is critical. It is the hypothesis of the [[def-mountain-pass|mountain-pass]] and minimization theorems.
> - The [[def-dirichlet-energy|Dirichlet energy]] on maps of a surface *fails* (PS) — a minimizing sequence can concentrate energy into a bubble and lose compactness (this is the critical-exponent failure). The [[def-alpha-energy|α-energy]] with $\alpha > 1$ *satisfies* (PS), by the compact Sobolev embedding $W^{1,2\alpha} \hookrightarrow C^0$ — the whole reason for the perturbation.
