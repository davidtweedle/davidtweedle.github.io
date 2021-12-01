---
title: Lecture 8 - Singular value decomposition
layout: page
permalink: /courses/math-3273/videos/lecture-8
---
This sequence of videos introduces the singular value decomposition of a matrix.

**Propopsition.** Suppose that $$ A = A^T$$ if $$A $$ has real entries ($$A$$ is called symmetric) or $$A = A^{\ast}$$ if $$A$$ has complex entries ($$A$$ is called Hermitian).
Then if $$A$$ is symmetric, there exists orthogonal $$Q$$ such that $$A = QDQ^T$$ where $$D$$ is a diagonal matrix with real entries.

If $$A$$ is Hermitian, then there exists unitary matrix $$U$$ such that $$A = UDU^{\ast}$$ where $$D$$ is a diagonal matrix.<br>

**Definition.** Let $$A$$ be a symmetric or Hermitian matrix.
Let the eigenvalues of $$A$$ be $$\lambda_1,\ldots,\lambda_n$$.
Then $$A$$ is called positive semi-definite if $$\lambda_1,\ldots,\lambda_n\geq 0$$.<br>

**Proposition.** Let $$A$$ be a symmetric or Hermitian matrix. Then $$A$$ is positive semi-definite if and only if $$\mathbf{x}^TA\mathbf{x}\geq 0$$ for all $$\mathbf{x}\in\mathbb{R}^n$$ (if $$A$$ is symmetric) or $$\mathbf{x}^{\ast}A\mathbf{x}\geq 0$$ for all $$\mathbf{x}\in\mathbb{C}^n$$ (if $$A$$ is Hermitian).<br>

<iframe width="560" height="315" src="https://www.youtube.com/embed/HOLcRW6UmIk" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

**Proposition.** If $$A$$ is positive semi-definite, then there exists a unique positive semi-definite matrix $$B$$ such that $$B^2 = A$$.

<iframe width="560" height="315" src="https://www.youtube.com/embed/auvgZiwEct0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

**Definition.** Let $$A$$ be an $$m$$-by-$$n$$ matrix.
Let the rank of $$A$$ be $$r$$.
Then $$A^{\ast}A$$ is positive semi-definite and has $$r$$ non-zero eigenvalues.
Writing the eigenvalues as $$\sigma_1^2,\ldots,\sigma_r^2$$, we define the singular values of $$A$$ to be $$\sigma_1\geq \sigma_2\geq\cdots \sigma_r>0 = \sigma_{r+1} = \cdots = \sigma_q$$
where $$q = \min(m,n)$$.<br>

<iframe width="560" height="315" src="https://www.youtube.com/embed/e2dSJs0tDW4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

**Theorem.** Let $$A$$ be an $$m$$-by-$$n$$ matrix, with rank $$r$$.
Let

$$\Sigma_r = \left(\begin{array}{cccc} \sigma_1\\&\sigma_2\\&&\ddots\\ &&&\sigma_r\end{array}\right) $$

and let

$$\Sigma = \left(\begin{array}{cc} \Sigma_r & 0\\0&0\end{array}\right) $$

be an $$m$$-by-$$n$$ matrix written in block form.
Then there exists a unitary $$m$$-by-$$n$$ matrix $$V$$ and unitary $$n$$-by-$$n$$ matrix $$W$$ such that

$$A = V\Sigma W^{\ast}.$$

<iframe width="560" height="315" src="https://www.youtube.com/embed/A9oums1jw3U" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
