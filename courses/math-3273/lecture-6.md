---
title: Lecture 6 - QR factorizations
layout: page
permalink: /courses/math-3273/videos/lecture-6
---
In this sequence of videos, we will talk about isometries, unitary and orthogonal matrices, Householder transformations, and the QR factorization.

In this series, $$k = \mathbb{R}$$ or $$\mathbb{C}$$, and $$V$$ is an inner product space over $$k$$ with inner product $$\langle\cdot,\cdot\rangle$$.

Recall that the norm on $$V$$ is defined by $$\lVert \mathbf{v}\rVert = \sqrt{\langle \mathbf{v},\mathbf{v}}$$.

Recall: 
1. If $$V$$ is finite-dimensional and $$T:V\to V$$ then there exists $$T^*:V\to V$$ such that $$\langle \mathbf{w}, T(\mathbf{v})\rangle = \langle T^*(\mathbf{w}),\mathbf{v}\rangle$$ for all $$\mathbf{v},\mathbf{w}\in V$$.
2. (This is not something we discussed but it can be verified). If $$k = \mathbb{R}$$ then

$$\langle \mathbf{v},\mathbf{w}\rangle = \frac{1}{4}(\lVert \mathbf{v}+\mathbf{w}\rVert^2 - \lVert \mathbf{v}-\mathbf{w}\rVert^2),$$

and if $$k=\mathbb{C}$$ then

$$ \langle \mathbf{v},\mathbf{w}\rangle = \frac{1}{4}(\lVert \mathbf{v} + \mathbf{w}\rVert^2+
i\lVert i\mathbf{v} + \mathbf{w}\rVert^2 + i^2 \lVert i^2\mathbf{v} + \mathbf{w}\rVert^2
+i^3\lVert i^3\mathbf{v} + \mathbf{w}\rVert^2).$$
Note this is stated incorrectly in the video.

<iframe width="560" height="315" src="https://www.youtube.com/embed/9-VYnD6Vouc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

**Definition.** An isometry is a linear transformation $$T:V\to V$$ such that $$\lVert T(\mathbf{v})\rVert = \lVert \mathbf{v} \rVert$$ for all $$\mathbf{v}\in V$$.

In the video, we see that an isometry can be characterized as satisfying

$$ \langle T(\mathbf{v}),T(\mathbf{w})\rangle = \langle \mathbf{v},\mathbf{w}\rangle $$

for all $$\mathbf{v},\mathbf{w}\in V$$.

Furthermore, if $$V$$ is finite-dimensional, then $$T$$ is an isometry if and only if $$T^*T = I$$.

<iframe width="560" height="315" src="https://www.youtube.com/embed/HQR-mmiVq7c" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

**Definition.** An $$n$$-by-$$n$$ matrix $$U$$ is called unitary if $$U^*U = I$$.
If $$U$$ has real entries and $$U^TU = I$$ then $$U$$ is called orthogonal.

*Note* - The columns of a unitary matrix form an orthonormal basis for $$\mathbb{C}^n$$, and the columns of an orthogonal matrix form an orthonormal basis for $$\mathbb{R}^n$$.

<iframe width="560" height="315" src="https://www.youtube.com/embed/15R7hH9dDpY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Recall that if $$\mathbf{w}\neq\mathbf{0}$$ then we define the projection onto $$\mathbf{w}$$ as the matrix

$$P_{\mathbf{w}} = \frac{\mathbf{w}\mathbf{w}^*}{\mathbf{w}^*\mathbf{w}}.$$

With this convention, the Householder matrix corresponding to $$\mathbf{w}$$ is

$$U_{\mathbf{w}} = I - 2\frac{\mathbf{w}\mathbf{w}^*}{\mathbf{w}^*\mathbf{w}} = I - 2P_{\mathbf{w}}.$$

Householder matrices are unitary (orthogonal if $$\mathbf{w}$$ has real entries, and satisfy $$U_{\mathbf{w}}^2 = I$$.

<iframe width="560" height="315" src="https://www.youtube.com/embed/y4vHBePzRps" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Householder matrices can be used as follows.
If $$\lVert \mathbf{x}\rVert = \lVert \mathbf{y}\rVert \neq 0$$ then let $$\mathbf{w} = \mathbf{x} - \mathbf{y}$$, and let $$U = U_{\mathbf{w}}$$. Then $$U\mathbf{x} = \mathbf{y}$$.

<iframe width="560" height="315" src="https://www.youtube.com/embed/SLmxFcT8TXU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

By using Householder matrices one may calculate the QR factorization.

**Theorem.** Let $$A$$ be an $$m$$-by-$$n$$ matrix with $$m\geq n$$.
Then there exists an $$m$$-by-$$m$$  unitary matrix $$V$$ and an $$n$$-by-$$n$$ upper triangular matrix $$R$$ with non-negative entries on the diagonal such that

$$A = V\left(\begin{array}{c} R\\ 0\end{array}\right).$$

In the following video, we calculate the QR factorization step-by-step using sagemath.

<iframe width="560" height="315" src="https://www.youtube.com/embed/ZNW21C0VB7Y" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Here are some of the functions we used in the above video.

To define a vector $$x = \left(\begin{array}{c}1\\2\\3\\4\end{array}\right) $$, say, we would enter 

    x = vector([1,2,3,4]);

To compute $$I - 2\frac{\mathrm{w}\mathrm{w}^T}{\mathrm{w}^T\mathrm{w}} $$ we used

    identity_matrix(4) - 2*(w.row()*w.column())/(w*w);

To define a 4-by-4 matrix, $$ A = \left(\begin{array}{cccc} 1&2&3&4\\0&1&2&3\\0&0&1&2\\0&0&0&1\end{array}\right) $$ we can use

    A = matrix(4,4,[[1,2,3,4],[0,1,2,3],[0,0,1,2],[0,0,0,1]]);

If we have two matrices $$ A $$ and $$ B $$ we can construct the block matrix $$A\oplus B = \left(\begin{array}{cc} A&0\\0&B\end{array}\right)$$ by doing

    A.block_sum(B)

Finally, if we are given a 4-by-4 matrix $$ A $$ and we want to extract the matrix $$ B $$ consisting of the entries in the 2nd, 3rd and 4th columns and rows, we would put

    A = random_matrix(ZZ,4,4);
    B = A[[1..3],[1..3]];

Note that there was a mistake in the code shown above in the video, sorry!
