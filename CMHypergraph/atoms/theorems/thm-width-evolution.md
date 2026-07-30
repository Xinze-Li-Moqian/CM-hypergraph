---
id: 4664efa21149
type: theorem
references:
  - "[[ref-coldingminicozzi|Colding & Minicozzi, Theorem 1.1]]"
  - "[[ref-john-w-morgan-gang-tian|Morgan & Tian, ch. 18 gives the loop-and-disk analogue]]"
---
# Theorem — Evolution of the width under Ricci flow

The main estimate of the sweepout route to extinction: under Ricci flow, the width decreases at the definite rate $4\pi$, up to a correction that fades like $1/t$.

## Statement

> [!theorem] Evolution of the width under Ricci flow
> Let $(M, g(t))$, $t \in [0, T)$, be a [[def-ricci-flow|Ricci flow]] on a [[def-closed-manifold|closed]] $3$-manifold and let $[\beta]$ be a nontrivial class of [[def-sweepout-width|sweepouts]]. Then the [[def-sweepout-width|width]] $W(g(t), [\beta])$ satisfies, in the sense of the limsup of forward difference quotients,
> $$
> \frac{d}{dt}\, W\big(g(t), [\beta]\big) \;\le\; -4\pi \;+\; \frac{3}{4\,(t + C)}\, W\big(g(t), [\beta]\big),
> $$
> where $C = C(g(0))$ is the constant of [[lem-scalar-curvature-lower-bound]].

## Proof

> [!note]- Proof — citation chain (click to expand)
> Fix $t_0 \in [0, T)$ and write $W_0 = W(g(t_0), [\beta])$. Below $C'$ is a constant depending only on $t_0$, allowed to change from line to line. The strategy: use the sweepout at time $t_0$ as a *competitor* for the width at later times $t > t_0$.
>
> 1. **The top of the sweepout is minimal spheres.** Apply [[prop-minmax-minimal-spheres]] to $(M, g(t_0))$ and $[\beta]$: for $\epsilon > 0$ there are $J$ and $\delta > 0$ so that for $j > J$, any slice with $E_{g(t_0)}(\gamma^j_s) > W_0 - \delta$ is $\epsilon$-close in the [[def-varifold|varifold distance]] to a union $\bigcup_i \Sigma_{s,i}$ of [[def-minimal-surface|branched minimal]] $2$-spheres.
> 2. **Each near-maximal slice decays.** Fix such an $s$. By [[lem-varifold-quadratic-form]] with $F = \operatorname{Ric}$, the first-variation integrand of [[lem-area-first-variation-under-flow]] for $\gamma^j_s$ agrees with that for $\bigcup_i \Sigma_{s,i}$ up to $C'\epsilon\,\|\operatorname{Ric}\|_{C^1}\operatorname{Area}(\gamma^j_s)$; then [[lem-minimal-sphere-area-decay]] on each $\Sigma_{s,i}$ and the lower bound $\min_M R(t_0) \ge -\tfrac{3}{2}/(t_0+C)$ of [[lem-scalar-curvature-lower-bound]] give
> $$
> \frac{d}{dt}\Big|_{t=t_0}\!\operatorname{Area}_{g(t)}(\gamma^j_s) \;\le\; -4\pi \;-\; \frac{E_{g(t_0)}(\gamma^j_s)}{2}\min_M R(t_0) \;+\; C'\epsilon \;\le\; -4\pi + \frac{3}{4(t_0+C)}\max_s E_{g(t_0)}(\gamma^j_s) + C'\epsilon .
> $$
> 3. **Compare at later times — the estimate $(\ast)$.** For $j > J$ and $0 < h < \bar h$, in the sense of forward difference quotients,
> $$
> \operatorname{Area}_{g(t_0+h)}(\gamma^j_s) - \max_s E_{g(t_0)}(\gamma^j_s) \;\le\; \Big[ -4\pi + C'\epsilon + \tfrac{3}{4(t_0+C)}\max_s E_{g(t_0)}(\gamma^j_s)\Big] h + C' h^2 . \tag{$\ast$}
> $$
> This holds by *two cases on $s$*, for a threshold $\bar h > 0$ independent of $j$:
>    - if $E_{g(t_0)}(\gamma^j_s) > W_0 - \delta$: since the $g(t)$ vary smoothly and the $\gamma^j$ have uniformly bounded energy, $E_{g(t_0+h)}(\gamma^j_s)$ is a smooth function of $h$ with a uniform $C^2$ bound near $h = 0$; Taylor expansion of the bound in step 2 gives $(\ast)$;
>    - if $E_{g(t_0)}(\gamma^j_s) \le W_0 - \delta$: continuity of $g(t)$ keeps $E_{g(t_0+h)}(\gamma^j_s) \le W_0$ for $h$ small, so $(\ast)$ holds automatically after shrinking $\bar h$.
> 4. **Pass to the width.** The width is a minimum over competitors, so using $\gamma^j$ as a competitor for $g(t_0+h)$,
> $$
> W(g(t_0+h), [\beta]) \;\le\; \max_s \operatorname{Area}_{g(t_0+h)}(\gamma^j_s).
> $$
> Taking $\max_s$ in $(\ast)$ and letting $j \to \infty$ (so $\max_s E_{g(t_0)}(\gamma^j_s) \to W_0$),
> $$
> \frac{W(g(t_0+h), [\beta]) - W_0}{h} \;\le\; -4\pi + C'\epsilon + \frac{3}{4(t_0+C)} W_0 + C' h ;
> $$
> letting $h \to 0^+$ and then $\epsilon \to 0$ gives the claim at $t_0$. $\square$

## Notes

> [!note]- Notes (click to expand)
> - **How to read "in the sense of the limsup of forward difference quotients."** The function $t \mapsto W(g(t), [\beta])$ need not be differentiable: an inf–max of smooth quantities is in general only Lipschitz, with corners wherever the near-optimal sweepout changes — the same way the lowest eigenvalue of a smooth family of operators loses differentiability at a crossing. The display is therefore shorthand for the genuine assertion
>   $$
>   \limsup_{h \to 0^+} \frac{W(g(t+h), [\beta]) - W(g(t), [\beta])}{h} \;\le\; -4\pi + \frac{3}{4\,(t+C)}\, W(g(t), [\beta]).
>   $$
>   *Forward* ($h \to 0^+$) because the proof only controls the future: the near-optimal sweepout at time $t$ is evolved as a competitor at times $t + h$ (step 4), which bounds $W(g(t+h))$ from above and says nothing about $h < 0$. $\limsup$ because the difference quotients may not converge as $h \to 0^+$, so the claim is that even their worst subsequential rate obeys the bound. Nothing is lost downstream: for a continuous function, an upper bound on this upper forward Dini derivative still integrates — the ODE comparison lemma holds verbatim in the Dini sense — so the consumers of this card may treat $W$ as if it were differentiable.
> - **Relation to the source statement.** The source theorem assumes $M$ closed, [[def-orientable|orientable]], prime and non-[[def-aspherical|aspherical]], and writes $W(g(t))$ with no class in sight. The hypotheses are refactored here by exact match: the estimate consumes only the *existence* of a nontrivial sweepout class, so this card takes the class $[\beta]$ as its hypothesis and carries it in the notation $W(g(t), [\beta])$. That closed manifolds with no aspherical prime factor carry such a class ($\pi_3 \neq 0$) is the separate topological fact [[lem-nonaspherical-sweepout-class]] — stated there without the primeness assumption, which the extinction argument cannot afford: post-surgery components are connected sums. The source's concluding sentence, "hence, $g(t)$ must become extinct in finite time", is [[cor-no-immortal-flow]].
> - The three inputs play fixed roles: the min-max realization converts the width into concrete minimal spheres, the area-decay lemma provides the $-4\pi$, and the scalar-curvature clock provides the fading correction. Nothing else about the flow is used — no surgery theory, no canonical neighborhoods.
> - The immediate cash-out is [[cor-no-immortal-flow]]: a smooth immortal flow on a manifold carrying a nontrivial sweepout class is impossible — the engine behind finite-time extinction.
> - What this card does *not* cover, toward the extinction theorem proper — both now cards of their own: the topological input is [[lem-nonaspherical-sweepout-class]] (a nontrivial class exists when no prime factor is aspherical), and the compatibility with surgery times is [[lem-surgery-preserves-width-inequality]] (surgeries only remove components or decrease the width). The extinction proof assembles all three.
