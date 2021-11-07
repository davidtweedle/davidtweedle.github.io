---
title: Lecture 10 - Primitive Roots
layout: page
permalink: /courses/math-2400/Math-2400-videos/lecture-10
---

<iframe width="560" height="315" src="https://www.youtube.com/embed/_Ptfiq_jnkY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

**Definition** - Let $$n$$ be a positive integer. Let $$a$$ be an integer such that $$\gcd(a,n) = 1$$.
The order of $$a$$ modulo $$n$$, denoted $$\mathrm{ord}_n(a)$$ is defined to be the least integer $$d$$ such that $$a^d\equiv 1\bmod{n}$$.

*Note* - The order of $$a$$ modulo $$n$$ divides $$\varphi(n)$$.

**Definition** - Let $$n$$ be a positive integer. Let $$a$$ be an integer with $$\gcd(a,n) = 1$$.
Then $$a$$ is called a primitive root modulo $$n$$ if $$\mathrm{ord}_n(a) = \varphi(n)$$.

<iframe width="560" height="315" src="https://www.youtube.com/embed/NwmmeM7vDAk" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

**Proposition** - If $$ d = \mathrm{ord}_n(a) $$ then $$\{\overline{1},\overline{a},\ldots,\overline{a}^{d-1}\}\subseteq U_n$$ has $$d$$ distinct elements.

*Note* - So if $$a$$ is a primitive root modulo $$n$$, and $$\gcd(b,n) = 1$$ then there exists $$j$$ such that $$b\equiv a^j\bmod{n}$$, or $$\overline{a}^j = \overline{b}$$ in $$U_n$$.

<iframe width="560" height="315" src="https://www.youtube.com/embed/_QsoHAkIwcE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

**Proposition** - Let $$p$$ be a prime. Let $$d$$ divide $$\varphi(p) = p-1$$.
Then there are $$\varphi(d)$$ congruence classes $$\overline{a}\in U_p$$ such that $$\mathrm{ord}_p(a) = d$$.
In particular, there are primitive roots modulo $$p$$.

The ingredients for the proof of this proposition are:

1. Möbius inversion: $$\sum_{d\mid m} A(d) = m $$ implies that $$ \varphi(m) = \sum_{d\mid m}\mu(m/d) d = A(m)$$.
2. The polynomial $$x^d-1$$ has exactly $$d$$ roots in $$\mathbb{Z}/p\mathbb{Z}$$ if $$d$$ divides $$p-1$$.

It is also true (but we did not prove it) that there exists a primitive root modulo $$n$$ if and only if $$n = 2,4$$ or $$p^n$$ or $$2p^n$$ where $$p$$ ranges over the odd primes.
