---
title: Lecture 12 - Periodic continued fractions
layout: page
permalink: /courses/math-2400/Math-2400-videos/lecture-12
---
This series of videos is about periodic continued fractions.
Before watching the videos, remember the following facts and definitions.

**Definition** - A nearly simple continued fraction is 

$$[a_0,a_1,a_2,\ldots,a_n,z] = a_0 + \frac{1}{a_1 + \frac{1}{a_2+\frac{1}{\ddots + \frac{1}{z}}}}$$

and if $$\frac{p_n}{q_n} = [a_0,\ldots,a_n] $$ and $$\frac{p_{n-1}}{q_{n-1}} = [a_0,\ldots,a_{n-1}]$$ are the $$n$$-th and $$n-1$$-st convergents, then we have

$$ [a_0,a_1,\ldots,a_n,z] = \frac{p_{n-1} + p_nz}{q_{n-1} + q_n z} $$


In this first video, we will prove the following lemma.

**Lemma** - If $$[a_0,a_1,\ldots,a_n,z] = \frac{A+Bz}{C+Dz}$$ then $$\frac{1}{[a_n,a_{n-1},\ldots,a_0,\frac{1}{w}]} = \frac{A+Cw}{B+Dw}$$.

<iframe width="560" height="315" src="https://www.youtube.com/embed/c1CdfvrDl3g" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Now using the lemma above, we are able to establish that if $$a_0,a_1,\ldots,a_n$$ are positive integers such that

$$ \alpha = [\overline{a_0,a_1,\ldots,a_n}] $$

and

$$ \beta = [\overline{a_n,a_{n-1},\ldots,a_0}] $$

then $$\alpha $$ is the root of a quadratic polynomial and the conjugate root $$\alpha'$$ satisfies $$\alpha' = \frac{-1}{\beta}$$, so that $$-1<\alpha'<0$$.

The following video illustrates the process.
<iframe width="560" height="315" src="https://www.youtube.com/embed/QSzXGu2r4NI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

In fact, there is a converse to the above result.

**Theorem (Converse to above).** Suppose that $$\alpha>1$$ is the root of a quadratic polynomial $$Ax^2 + Bx + C = 0$$ whose conjugate root $$\alpha'$$ is such that $$-1<\alpha'<0$$.
Then the continued fraction of $$\alpha$$ is purely periodic.

One of the ingredients in the proof of the converse is to prove that for fixed $$D>0$$ there are only finitely many $$P,Q$$ such that $$\frac{P+\sqrt{D}}{Q}>1$$ and $$-1 <\frac{P-\sqrt{D}}{Q}<0$$.

This is discussed briefly in the following video.
<iframe width="560" height="315" src="https://www.youtube.com/embed/AutgZI2Bkes" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Finally, we discuss the continued fraction expansion of $$\sqrt{N}$$ in the below video.
<iframe width="560" height="315" src="https://www.youtube.com/embed/-Jfe4b8qeZA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
