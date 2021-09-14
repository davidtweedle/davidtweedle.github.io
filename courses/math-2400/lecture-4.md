---
title: Lecture 4 - more about gcd's
layout: page
permalink: /courses/math-2400/Math-2400-videos/lecture-4
---
<iframe width="560" height="315" src="https://www.youtube.com/embed/l_nr7jY1jyM" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

In this video we cover the following concepts:

*gcd* - We prove that $$ \gcd(ab,c) = \gcd(a,c)\gcd(b,c) $$ if $$ \gcd(a,b,c) = 1 $$.

*more gcds* - We use the above formula to prove that if $$ \gcd(m,n) = 1 $$ and if $$ D \mid mn $$ then $$ D = \gcd(m,D) \gcd(n,D) $$ so that $$ D $$ factors as a divisor of $$ m $$ times a divisor of $$ n $$.

Let's make a table with $$ m = 20 $$ and $$ n = 21 $$, so $$ mn = 420 $$

| $$ d $$ |  $$ \gcd(d,20) $$ |  $$ \gcd(d,21) $$ |
|--------|------------------|-------------------------|
| 1 | 1 | 1|
|2 | 2 | 1 |
|3 | 1 | 3 |
|4 | 4 | 1 |
|5 |5 | 1 |
|6 |2 | 3|
|7 | 1 | 7|
|10 | 10 | 1 | 
| 12 | 4 | 3 |
| 14 | 2 | 7 |
| 15 | 5 | 3 | 
| 20 | 20 | 1 | 
| 21 | 1 | 21 |
| 28 | 4 | 7 |
|30 | 10 | 3 |
| 35 | 5 | 7 |
| 42 | 2 | 21 |
| 60 | 20 | 3 |
| 70 | 10 | 7 |
| 105 | 5 | 21 |
| 140 | 20 | 7 |
| 210 | 10 | 21 |
| 420 | 20 | 21 |

Now ask yourself, what is the relationship between the number of divisors of $$ 20 $$ (which is $$ 6 $$) and the number of divisors of $$ 21 $$ (which is $$ 4 $$) and the number of rows of the above table.



