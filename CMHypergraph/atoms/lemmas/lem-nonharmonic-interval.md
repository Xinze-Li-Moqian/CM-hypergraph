---
id: 044bee5b3430
type: lemma
references:
  - "[[ref-cm-width-extinction|Colding & Minicozzi, Width and finite extinction, §3, Lemma `l:sf`]]"
---

# Lemma — Non-harmonic slices fill an interval

The energy improvement of a slice cannot jump: near any time, the
improvement available at a slightly finer scale is at most twice that
at the current one — so the tightening acts on a whole interval, not an
instant, and can be done continuously.

## Statement

> [!lemma] Interval structure of non-harmonic slices
> If a slice $\sigma(\cdot, t)$ is not [[def-minimal-surface|harmonic]] and $\epsilon \in (0, \epsilon_1]$, then there is an open interval $I^t \ni t$ such that the [[def-energy-improvement|energy improvement]] satisfies
> $$
> e_{\sigma, \epsilon/2}(s) \;\le\; 2\, e_{\sigma, \epsilon}(t) \qquad \text{for all } s \in 2I^t
> $$
> (the doubled interval).

## Proof

> [!note]- Proof (click to expand)
> Continuity of [[def-harmonic-replacement|harmonic replacement]] in $C^0 \cap W^{1,2}$ ([[lem-harmonic-replacement-continuity]]) gives $\delta_1 > 0$ (depending on $t$) such that if $\|\sigma(\cdot,t) - \sigma(\cdot,s)\|_{C^0\cap W^{1,2}} < \delta_1$ and $\mathcal{B}$ is a collection where both slices have energy $\le \epsilon_1$, then the energy drops from replacement on $\tfrac12\mathcal{B}$ agree for $\sigma(\cdot,s)$ and $\sigma(\cdot,t)$ up to a factor near $1$. Since the family $\sigma(\cdot,\cdot)$ is continuous into $C^0\cap W^{1,2}$, the condition $\|\sigma(\cdot,t)-\sigma(\cdot,s)\| < \delta_1$ holds on an open interval $I^t$ around $t$; on its double $2I^t$ (shrinking $I^t$ if needed) the balls realizing $e_{\sigma,\epsilon/2}(s)$ are admissible for $\sigma(\cdot,t)$ at scale $\epsilon$, giving $e_{\sigma,\epsilon/2}(s) \le 2\, e_{\sigma,\epsilon}(t)$. $\square$

## Notes

> [!note]- Notes (click to expand)
> - CM Lemma `l:sf` (§3): the local-in-time structure that lets [[lem-good-balls]] be patched into a continuous choice, hence [[thm-energy-decreasing-map]] be a continuous map of families.
