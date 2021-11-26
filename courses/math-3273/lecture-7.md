---
title: Lecture 7 - Jordan canonical form
layout: page
permalink: /courses/math-3273/videos/lecture-7
---
In this sequence of videos, we will discuss the Jordan canonical form of a matrix/linear transformation.

**Definition** - Let $$ U $$ be a subspace of $$ V$$ and suppose $$ T:V\to V$$. Then $$U $$ is called $$T$$-invariant if $$T(U)\subseteq U$$.

**Example** - $$0$$, $$ V$$, $$\mathrm{ker}(T)$$, $$T(V)$$, $$\mathrm{ker}(g(T))$$, $$g(T)(V)$$ where $$ g$$ is a polynomial, are all examples of invariant subspaces.

**Key Lemma** - $$V = \mathrm{ker}(g(T)) \oplus \mathrm{ker}(h(T))$$ if $$f(T) = 0$$ and $$f = gh$$ with $$\gcd(g,h) = 1$$.

**Example** - Suppose that $$ (T-2)(T-3) = 0$$, then prove that $$ T$$ is diagonalizable.

<iframe width="560" height="315" src="https://www.youtube.com/embed/Quju5CDEtJE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Using the above lemma and induction, we can establish that

**Theorem** 

$$V = \mathrm{ker}((T-\lambda_1)^{m_1})\oplus \mathrm{ker}((T-\lambda_2)^{m_2})\oplus\cdots \oplus \mathrm{ker}((T-\lambda_k)^{m_k}).$$

The key is that each of the above subspaces is $$T$$ invariant.

So the matrix of $$T$$ will be a block diagonal matrix

$$\left(\begin{array}{cccc} A_1\\&A_2\\&&\ddots\\ &&&A_k\end{array}\right) $$

where each $$A_i$$ is the matrix of $$ T $$ restricted to $$\mathrm{ker}((T-\lambda_i)^{m_i})$$

Restricting to $$\mathrm{ker}((T-\lambda_i)^{m_i})$$ and substituting $$T' = T-\lambda_i$$, we have reduced to the case when $$ T^m = 0 $$.

In order to understand the case when $$ T:V\to V$$ and $$ T^m = 0$$ we have cyclic subspaces.

**Definition** - Suppose that $$ T^m\mathrm{v} = \mathrm{0}$$ but $$ T^{m-1}\mathrm{v} \neq \mathrm{0}$$.
Then $$ U = \mathrm{span}(\mathrm{v},T\mathrm{v},\ldots,T^{m-1}\mathrm{v})$$ is called a cyclic subspace of $$ V $$.
The vector $$\mathrm{v}$$ is called a cyclic vector.
Notice that every element of $$ U $$ can be written as $$\mathrm{u} = p(T) \mathrm{v} $$ for some polynomial $$p$$.
If $$ U $$ is a cyclic subspace with cyclic vector $$\mathrm{v}$$ we write $$U = C(\mathrm{v})$$.

First, we define cyclic subspaces and prove that $$ \mathrm{v},T\mathrm{v},\ldots, T^{m-1}\mathrm{v}$$ is a basis for $$C(\mathrm{v})$$.

<iframe width="560" height="315" src="https://www.youtube.com/embed/BLOxA4gwgbM" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Then we prove that if $$ T:V\to V $$ and $$ T^m = 0$$, and $$ V $$ is finite-dimensional, then $$ V $$ is the direct sum of cyclic subspaces.


<iframe width="560" height="315" src="https://www.youtube.com/embed/9wWYAo-7LYc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

The proof is by induction.

Finally, we (briefly) mention the payout from all this work.
<iframe width="560" height="315" src="https://www.youtube.com/embed/zsqIB_IRlqE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

