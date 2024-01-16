# Approximation in $\ell_p^N$

Here we will discuss basic properties of the $\ell_p^N$ space related to the Approximation theory.
Let us recall that the norm in $\ell_p^N$ is defined as:
```math
\|x\|_p := \begin{cases}
 (\sum_{k=1}^n |x_k|^p)^{1/p},&\quad 1\le p<\infty,
 \max|x_k|,&\quad p=\infty.
\end{cases}
```

## Basic inequalities

Underneath the L_p theory there are some basic numeric inequalities, let us recall them.
It is also wise to trace when the inequality becomes the equality. 

**Inequality between arithmetic and geometric mean** ([HLP], 2.5). Let $a_1,\ldots,a_n\ge 0$ and let $w_i$ be positive weights: $w_i>0$, $w_1+\ldots+w_n=1$ (we do not allow zero weights; $w_k=0$ means simply that $a_k$ is discarded). Then
```math
a_1^{w_1}a_2^{w_2}\cdots a_n^{w_n} \le w_1a_1 + \ldots + w_na_n.
```
To prove this we use the concavity of the log function: $\sum w_n\log a_n \le \log\sum w_na_n$.

We have the equality only in the case $a_1=a_2=\ldots=a_n$. 

**Holder inequality**. Let $x,y\in\mathbb R^N$, $1\le p\le \infty$ and $1/p+1/p'=1$. Then
```math
|\langle x,y\rangle| \le \|x\|_p \|y\|_{p'}.
```
This is obvious when $p=1$ or $p=\infty$. Let $1<p<\infty$. We can assume that $x_k,y_k\ge 0$ (if we replace coordinates by their modules, the rhs of the inequality will not change and lhs will increase). Put $a_1 := x_1^p$, $w_1 = 1/p$, $a_2 = y_1^{p'}$, $w_2=1/p'$ and apply the AGM inequality: $x_1y_1 \le x_1^p/p + y_1^{p'}/p'$. If we sum over all coordinates, we will obtain:
```math
\langle x,y\rangle \le \|x\|_p^p/p + \|y\|_{p'}^{p'}/p'.
```
Holder inequality is homogenius so we can normalize it by $\|x\|_p=\|y\|_{p'}=1$. Then we obtain $\langle x,y\rangle \le 1/p+1/p'=1$, as required.

**Duality**
```math
\|x\|_p = \max_{\|z\|_{p'}\le 1}\langle x,z\rangle = \max_z \langle x,z\rangle / \|z\|_{p'}
```
Indeed, Holder inequality gives $\ge$. The equality holds for $z_k=|x_k|^{p'}\sign x_k$ (???)

## References

[HLP] Hardy, Lettlewood, Polya. *Inequalities*.
