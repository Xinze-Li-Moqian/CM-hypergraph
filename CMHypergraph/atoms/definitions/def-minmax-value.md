---
id: 3c497caf10ac
type: definition
references:
  - "[[ref-jost|Jost, §4.2 — the setup of the general existence theorem]]"
  - "the one-parameter classic: Ambrosetti & Rabinowitz (1973); Struwe, Variational Methods, ch. II"
---

# Definition — min-max value of a family

The general scheme behind every width: sweep a compact family through a space, record the highest value the functional attains on the family, and minimize that height over all competing families. The parameter space is the shape of the sweep; its dimension is the number of directions in which the resulting critical point can be unstable.

## Statement

> [!definition] Min-max value of a family
> Let $X$ be a topological space, $\mathcal{F} : X \to \mathbb{R}$ continuous, $A$ a compact space — the *parameter space* — and $B \subset A$ closed, possibly empty. Fix a continuous $h_0 : A \to X$ and let $H$ be the class of all continuous $h : A \to X$ homotopic to $h_0$ through maps agreeing with $h_0$ on $B$. The *min-max value* of the family class $H$ is
> $$
> k \;=\; \inf_{h \in H} \, \max_{t \in A} \, \mathcal{F}\big(h(t)\big).
> $$
> The family class is *pinned* if $k > \max_{t \in B} \mathcal{F}(h_0(t))$: the top of every near-optimal family lies away from the fixed part.

## Notes

> [!note]- Notes (click to expand)
> - Compactness of $A$ is what the scheme runs on: the maximum over $t \in A$ is attained, near-maximal parameters have convergent subsequences, and $k$ is finite whenever one family has bounded $\mathcal{F}$.
> - **The one-parameter case is the [[def-mountain-pass|mountain pass]]**: $A = [0,1]$, $B = \{0, 1\}$, families = paths between two fixed points; pinning says the pass is higher than both valleys. Producing an actual [[def-critical-point|critical point]] at level $k$ is a theorem, not part of the definition — it needs compactness of the functional ([[def-palais-smale|Palais–Smale]]) or, where that fails, bespoke machinery.
> - The heuristic the pool uses repeatedly: a critical point produced by an $A$-parameter min-max has [[def-minimal-surface-index|Morse index]] at most $\dim A$ — the family provides at most $\dim A$ unstable directions. For sweepouts ($\dim A = 1$) this is the index bound of [[thm-minmax-harmonic-maps]] via [[thm-micallef-moore-index]].
> - Instances in this graph: the [[def-sweepout-width|width]] is the min-max value of $E$ over the sweepout class ($X$ the mapping space, $A = [0,1]$, $B$ its endpoints pinned at constant maps); [[thm-minmax-harmonic-maps]] is the general existence theorem over an arbitrary compact $A$.
