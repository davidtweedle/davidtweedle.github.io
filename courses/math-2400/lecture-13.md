---
title: Lecture 13 - basics of RSA
layout: page
permalink: /courses/math-2400/Math-2400-videos/lecture-13
---
In this series of videos, we will introduce the basics of the RSA cryptosystem.

Alice wants to send a message to Bob securely.

First, Bob generates a public and private key.

He chooses two (very large) primes $$p$$ and $$q$$ and sets $$N = pq$$.

Then he chooses $$1\leq e\leq N$$ with $$\gcd(e,\varphi(N)) = 1$$.

Bob's public key is $$(N,e)$$. He tells everyone his public key.

Next he computes his private key. This is secret.

He computes $$\varphi(N) = (p-1)(q-1)$$.

Then he computes $$1\leq d\leq N$$ such that $$de\equiv 1\bmod{\varphi(N)}$$.

Bob's private key is $$(\varphi(N),d)$$.

<iframe width="560" height="315" src="https://www.youtube.com/embed/M3NDKvuFWR4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Now, $$m$$ is our message we want to send and $$1\leq m\leq N$$.
Before we send $$m$$ we encrypt it by computing $$c = m^e\bmod{N}$$.
Then we send $$c$$ to Bob.

<iframe width="560" height="315" src="https://www.youtube.com/embed/rMW4yoADh3s" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Bob receives the integer $$c$$, called the ciphertext.
He computes $$c^d\bmod{N}$$ (that is why he has kept $$d$$ for himself).

**Proposition.** Assume $$\gcd(m,N) = 1$$. Then $$m\equiv c^d\bmod{N}$$.

<iframe width="560" height="315" src="https://www.youtube.com/embed/sJWMv68iv0A" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

In the following video, we briefly discuss the security of the private key.
It turns out, figuring out the private key given only the private key seems to be very difficult.

<iframe width="560" height="315" src="https://www.youtube.com/embed/ar0GSEnHqa4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
