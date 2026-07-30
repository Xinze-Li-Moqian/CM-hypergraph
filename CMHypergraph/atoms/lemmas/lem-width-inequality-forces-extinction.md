---
id: 85dff600ea95
type: lemma
references:
  - "[[ref-coldingminicozzi|Colding & Minicozzi, §1]]"
  - "the integration is displayed there between the theorem and its corollary"
---

# Lemma — The width inequality forces extinction

Pure calculus on one quantity: a width that must decrease at rate $4\pi$ minus a fading correction cannot live forever.

## Statement

> [!lemma] The width inequality forces extinction
> Let $(M, g(t))$, $t \in [0, T)$, be a [[def-ricci-flow|Ricci flow]] on a [[def-closed-manifold|closed]] $3$-manifold, $[\beta]$ a nontrivial class of [[def-sweepout-width|sweepouts]], and let $W(t) = W(g(t), [\beta])$ be the [[def-sweepout-width|width]]. Suppose that $W$ is continuous and, for some $C > 0$, satisfies the [[thm-width-evolution|width inequality]] in the sense of the limsup of forward difference quotients:
> $$
> \frac{d}{dt} W(t) \;\le\; -4\pi \;+\; \frac{3}{4\,(t + C)}\, W(t) .
> $$
> Then $T < T^*$ for some $T^* = T^*(C, W(0)) < \infty$.

## Proof

> [!note]- Proof (click to expand)
> Write $(\dagger)$ for the hypothesis $\frac{d}{dt} W \le -4\pi + \frac{3}{4(t+C)} W$, in the sense of the limsup of forward difference quotients.
>
> 1. **Change of variable.** Set
> $$
> \varphi(t) \;=\; (t + C)^{-3/4}\, W(t) .
> $$
> Since $(t+C)^{-3/4}$ is smooth and positive, a smooth factor passes through limsups of difference quotients, and the product rule gives, in the same limsup sense,
> $$
> \frac{d}{dt} \varphi(t) \;=\; (t+C)^{-3/4}\, \frac{d}{dt} W(t) \;-\; \tfrac{3}{4}\, (t+C)^{-7/4}\, W(t) .
> $$
> 2. **Substitute the hypothesis.** Multiplying $(\dagger)$ by $(t+C)^{-3/4} > 0$,
> $$
> (t+C)^{-3/4}\, \frac{d}{dt} W \;\le\; -4\pi\, (t+C)^{-3/4} \;+\; \tfrac{3}{4}\, (t+C)^{-7/4}\, W ,
> $$
> and adding the second term of step 1, the two $W$-terms cancel *exactly* — this cancellation is the reason for the exponent $3/4$ —
> $$
> \implies \quad \frac{d}{dt} \varphi(t) \;\le\; -4\pi\, (t+C)^{-3/4} .
> $$
> 3. **Integrate.** $\varphi$ is continuous (as $W$ is) with upper forward Dini derivative bounded by the continuous function $-4\pi(t+C)^{-3/4}$; by the comparison principle for Dini derivatives (a ground fact of calculus: such a function lies below the integral of its bound),
> $$
> \varphi(t) - \varphi(0) \;\le\; -4\pi \int_0^t (s+C)^{-3/4}\, ds \;=\; -16\pi \left[ (t+C)^{1/4} - C^{1/4} \right],
> $$
> $$
> \implies \quad (t+C)^{-3/4}\, W(t) \;\le\; C^{-3/4}\, W(0) \;-\; 16\pi \left[ (t+C)^{1/4} - C^{1/4} \right] \qquad \text{for all } t \in [0, T).
> $$
> 4. **Read off the bound.** The left side is $\ge 0$ for every $t$, because $W \ge 0$ by hypothesis and the factor is positive. The right side is strictly negative as soon as $(t+C)^{1/4} > C^{1/4} + \frac{W(0)}{16\pi}\, C^{-3/4}$, that is, for all
> $$
> t \;>\; T^* \;:=\; \left( C^{1/4} + \frac{W(0)}{16\pi\, C^{3/4}} \right)^{\!4} - \;C .
> $$
> $$
> 0 \;\le\; \text{LHS} \;\le\; \text{RHS} \;<\; 0 \ \text{ for } t > T^* \quad \implies \quad [0, T) \subseteq [0, T^*] \quad \implies \quad T \;\le\; T^* \;<\; \infty . \qquad \square
> $$

## Notes

> [!note]- Notes (click to expand)
> - **Scope.** The inequality enters as a *hypothesis*, not via [[thm-width-evolution]] automatically — that is what lets the lemma serve flows with surgery too, where the supplier is [[lem-surgery-preserves-width-inequality]] and the function fed in is the component-maximum width; the fit of that function to this statement is part of the surgery lemma's bookkeeping, recorded on the consuming edge.
> - All the geometry is in the two constants — the full accounting is [[rem-width-constants]].
> - Integrating a differential inequality that holds only for limsups of forward difference quotients is legitimate by the standard comparison principle for Dini derivatives.
