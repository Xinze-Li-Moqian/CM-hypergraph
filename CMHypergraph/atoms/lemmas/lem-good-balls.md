---
id: 9e5c6bfd690b
type: lemma
references:
  - "[[ref-cm-width-extinction|Colding & Minicozzi, Width and finite extinction, §3, Lemma `l:goodballs`]]"
---

# Lemma — Good balls for the tightening

A construction lemma of the tightening (§3): every slice with
substantial energy carries a small-energy ball collection on which one
harmonic replacement sheds a definite fraction of the slice's energy
improvement — and these can be chosen continuously in time.

## Statement

> [!lemma] Good balls
> Let $W > 0$ and $\tilde\gamma \in \Omega$ have no non-constant [[def-minimal-surface|harmonic]] slice. Then there are an integer $m$, collections of balls $\mathcal{B}_1, \dots, \mathcal{B}_m$ in $S^2$, and continuous $r_1, \dots, r_m : [0,1] \to [0,1]$ such that for each $t$:
>
> 1. at most two $r_j(t)$ are positive, and $\sum_{B \in \mathcal{B}_j} \tfrac12 \int_{r_j(t) B} |\nabla\tilde\gamma(\cdot,t)|^2 < \epsilon_1/3$ for each $j$;
> 2. if $E(\tilde\gamma(\cdot,t)) \ge W/2$, then for some $j(t)$, [[def-harmonic-replacement|harmonic replacement]] on $\tfrac{r_{j(t)}}{2}\mathcal{B}_{j(t)}$ decreases [[def-dirichlet-energy|energy]] by at least $\tfrac18\, e_{\tilde\gamma, \epsilon_1/8}(t)$, an eighth of the [[def-energy-improvement|energy improvement]].

## Proof

> [!note]- Proof (click to expand)
> The set $I = \{t : E(\tilde\gamma(\cdot,t)) \ge W/2\}$ is compact (energy is continuous in $t$). For each $t \in I$, choose a finite collection $\mathcal{B}^t$ of disjoint balls with $\tfrac12\int_{\cup\mathcal{B}^t}|\nabla\tilde\gamma(\cdot,t)|^2 \le \epsilon_1/4$ nearly achieving the [[def-energy-improvement|energy improvement]] $e_{\tilde\gamma,\epsilon_1/8}(t)$: replacement on $\tfrac12\mathcal{B}^t$ drops energy by $\ge \tfrac18 e_{\tilde\gamma,\epsilon_1/8}(t)$ (definition of the sup, up to a factor). By continuity of the energy of $\tilde\gamma(\cdot,s)$ and of harmonic replacement ([[lem-harmonic-replacement-continuity]]), the same collection works on a neighborhood of $t$; a finite subcover of the compact $I$ gives finitely many collections $\mathcal{B}_1,\dots,\mathcal{B}_m$. Partition-of-unity radius functions $r_j$ interpolate between them so at most two are active at once — the "at most two" of (1) — while preserving the small-energy bound (radii shrink where energy would exceed $\epsilon_1/3$). $\square$

## Notes

> [!note]- Notes (click to expand)
> - CM Lemma `l:goodballs` (§3): the input to the energy-decreasing map [[thm-energy-decreasing-map]] — it supplies, continuously in $t$, the balls over which replacement is performed.
