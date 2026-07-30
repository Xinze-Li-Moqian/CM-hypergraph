---
id: b5d2ecee64e3
type: lemma
references:
  - "[[ref-perelman3|Perelman, Finite extinction time…, §4.4]]"
  - "[[ref-coldingminicozzi|Colding & Minicozzi, §1]]"
  - "[[ref-john-w-morgan-gang-tian|Morgan & Tian, §18.12]]"
---
# Lemma — Surgery does not save the width

The width argument survives the surgeries: cutting necks and capping with balls can only remove components or decrease the width, so the differential inequality that dooms a smooth flow dooms the flow with surgery too.

## Statement

> [!lemma] Surgery does not save the width
> Let $({\mathcal M}, G)$ be a [[def-ricci-flow-with-surgery|Ricci flow with surgery]] defined for $t \in [0, \infty)$, and suppose every component of every time-slice carries a nontrivial class of [[def-sweepout-width|sweepouts]]. Define
> $$
> W(t) \;=\; \max_{N \,\subset\, M_t} \; \min_{[\beta] \neq 0} \; W\big(G(t)|_N, [\beta]\big),
> $$
> the maximum over components $N$ of $M_t$ of the smallest nontrivial width. Then $W$ satisfies, at every surgery time $T$,
> $$
> W(T) \;\le\; \limsup_{t \to T^-} W(t),
> $$
> and between surgery times it satisfies the differential inequality of [[thm-width-evolution]] with a constant $C$ depending only on the initial metric.


## Proof

> [!note]- Proof (click to expand)
> **Between surgery times** the flow is smooth on each component, so $W(t)$ is the max over components of a smooth-flow width, each satisfying the differential inequality of [[thm-width-evolution]] with the constant $C$ of [[lem-scalar-curvature-lower-bound]] — which is not reset because surgery regions carry large positive scalar curvature, so $\min_M R$ is unaffected downward. A maximum of finitely many functions each obeying $\frac{d}{dt}W_N \le -4\pi + \tfrac{3}{4(t+C)}W_N$ obeys the same inequality (the max's forward difference quotient is that of the achieving component).
> **Across a surgery time $T$** the post-surgery slice $M_T$ is obtained from $M_{T^-}$ by cutting necks and capping, plus discarding components. Each surviving component $N \subset M_T$ is a connected-sum factor of a pre-surgery component $N^-$; the quotient map $N^- \to N$ (collapse the other summands to points) pushes any [[def-sweepout-width|sweepout]] of $N$ back to one of $N^-$ *without increasing energy*, so every nontrivial class on $N$ has width $\le$ some nontrivial class on $N^-$: $W(T) \le \limsup_{t\to T^-} W(t)$. Discarded components only remove terms from the maximum. $\square$
## Notes

> [!note]- Notes (click to expand)
> - The mechanism (the proof debt): a post-surgery component $N$ is a connected-sum factor of a pre-surgery component $N^-$; the quotient map $N^- \to N$ collapsing the other summands pushes sweepouts forward without increasing energy, so nontrivial classes survive with no larger width. Components that disappear only remove terms from the maximum.
> - The constant $C$ survives surgery because the scalar-curvature lower bound does: the standard caps are glued with scalar curvature far above the running minimum, so the clock of [[lem-scalar-curvature-lower-bound]] is never reset.
> - This is the only card of the sweepout network that must know surgery exists; everything else lives on a smooth flow.
