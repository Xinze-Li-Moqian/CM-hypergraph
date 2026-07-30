---
id: cd13da19fa02
type: definition
references:
  - "[[ref-coldingminicozzi|Standard spectral geometry; Colding & Minicozzi, Appendix A]]"
  - "Chavel, Eigenvalues in Riemannian Geometry"
---

# Definition — eigenvalue and eigenfunction

The resonant frequencies of an operator: the values at which it acts by
mere scaling, and the functions it scales — for the Laplacian, the pure
tones of a drum.

## Statement

> [!definition] Eigenvalue; eigenfunction; first eigenvalue
> Let $L$ be a self-adjoint elliptic second-order operator on a closed Riemannian manifold $(\Sigma, g)$ — for instance the [[def-laplacian|Laplacian]] $\triangle$ or a *Schrödinger operator* $\triangle + V$. A number $\lambda$ is an *eigenvalue* with *eigenfunction* $\eta \not\equiv 0$ if
> $$
> L\eta + \lambda\, \eta \;=\; 0 .
> $$
> The spectrum is a discrete sequence $\lambda_1 \le \lambda_2 \le \cdots \to \infty$; $\lambda_1$ is the *first eigenvalue*, characterized variationally by the *Rayleigh quotient*
> $$
> \lambda_1 \;=\; \inf_{\phi \not\equiv 0} \frac{\int_\Sigma \big(|\nabla\phi|^2 - V\phi^2\big)}{\int_\Sigma \phi^2} .
> $$

## Notes

> [!note]- Notes (click to expand)
> - On a closed manifold the spectrum is discrete and bounded below (elliptic self-adjointness), so counts like the [[def-minimal-surface-index|index]] — the number of negative eigenvalues of the [[def-jacobi-operator|Jacobi operator]] — are finite.
> - The first eigenfunction of a Schrödinger operator does not change sign, so it may be taken positive; the higher Rayleigh quotients are minimized over functions orthogonal to the lower eigenfunctions — the fact the index-one argument of [[lem-second-eigenvalue-test]] uses.
