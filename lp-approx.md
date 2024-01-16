# Approximation in $\ell_p^N$

Here we will discuss basic properties of the $\ell_p^N$ space related to the Approximation theory.
Let us recall that the norm in $\ell_p^N$ is defined as:
```math
\|x\|_p := \begin{cases}
 (\sum_{k=1}^n |x_k|^p)^{1/p},&\quad 1\le p<\infty,
 \max|x_k},&\quad p=\infty.
\end{cases}
```

## Basic inequalities

Underneath the L_p theory there are some basic numeric inequalities, let us recall them.

**Inequality between arithmetic and geometric mean**. Let $a_1,\ldots,a_n>0$ and let $w_i$ be positive weights: $w_i>0$, $w_1+\ldots+w_n=0$. Then
```math
a_1^{w_1}a_2^{w_2}\cdots a_n^{w_n} \le w_1a_1 + \ldots + w_na_n.
```
To prove this we use the concavity of the log function: $\sum w_n\log a_n \le \log\sum w_na_n$.
