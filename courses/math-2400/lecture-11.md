---
title: Lecture 11 - Legendre Symbols and Gauss' Lemma
layout: page
permalink: /courses/math-2400/Math-2400-videos/lecture-11
---
**Definition** - Let $$p$$ be a prime.
If $$\gcd(a,p) = 1$$ and $$a\equiv b^2\bmod{p}$$ for some $$b$$, then we say that $$a$$ is a quadratic residue modulo $$p$$.
We sometimes say $$a$$ is a QR.
If $$\gcd(a,p) = 1$$ and $$a$$ is not a QR, then we say that $$a$$ is an NR (for not a quadratic residue).
If $$p\mid a$$ then we do not consider $$a$$ to be either QR or NR.

**Definition** - Let $$p$$ be a prime and let $$a\in \mathbb{Z}$$.
Then we define the Legendre symbol $$\left(\frac{a}{p}\right)$$ as follows

$$ \left(\frac{a}{p}\right) = \left\{ \begin{array}{ll}
1 &\text{if }a \text{ is a QR modulo }p\\
0 &\text{if }p\mid a\\
-1&\text{if }a\text{ is a NR modulo }p
\end{array}\right. $$

**Proposition.** Let $$p$$ be an odd prime and let $$\gcd(a,p) = 1$$. Then

$$ \left(\frac{a}{p}\right) \equiv a^{(p-1)/2}\bmod{p}.$$

**Corollary.** Let $$p$$ be an odd prime. Then

$$\left(\frac{-1}{p}\right) = (-1)^{(p-1)/2}.$$

The goal of the following two videos is to look at Gauss' Lemma and applying it to calculate $$\left(\frac{2}{p}\right)$$.

<iframe width="560" height="315" src="https://www.youtube.com/embed/lLi58WnlQOU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

In the above video, we have

$$S = \{1,2,\ldots,(p-1)/2\}$$

$$S' = \{b,2b,\ldots, \frac{p-1}{2} b\}.$$

**Proposition.** Let $$p$$ be an odd prime and $$\gcd(b,p) = 1$$.
Then for each $$a$$ with $$\gcd(a,p) = 1$$, there exists unique $$s\in S$$ and $$\epsilon\in \{1,-1\}$$ such that

$$ a\equiv \epsilon s\bmod{p}.$$

Similarly, there exists unique $$\epsilon'\in\{1,-1\}$$ and $$s'\in S'$$ with

$$a\equiv \epsilon' s'\bmod{p}.$$

Then in the following video, we apply this to prove Gauss' Lemma and calculate the Legendre symbol $$(2/p)$$.

For each $$r = 1,2,\ldots, (p-1)/2$$ we write $$br \equiv \epsilon_r s_r\bmod{p}$$ with $$\epsilon_r = \pm 1$$ and $$s_r\in S$$.

<iframe width="560" height="315" src="https://www.youtube.com/embed/iTjez_zoj7o" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


**Gauss' Lemma.** We have

$$ \left(\frac{b}{p}\right) = \epsilon_1\epsilon_2\cdots \epsilon_{(p-1)/2}.$$

**Corollary.** We have

$$\left(\frac{2}{p}\right) = (-1)^{(p^2-1)/8}.$$
