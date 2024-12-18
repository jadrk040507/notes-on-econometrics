# Linear Algebra

## Similar Matrices
Recall that given the basis for an $n$ dimensional vector space $V$, we can represent a linear transformation
$$T: V \to V$$
as an $n \times n$ matrix $A$. Unfortunately, if you choose a different basis for $V$, the matrix representing the linear transformation $T$ will be quite different from the original matrix $A$. This section's goal is to find out a clean criterion for when two matrices actually represent the same linear transformation but under different choice of bases.

<!-- \begin{definition}\label{def:decomposition} -->

Two $n \times n$ matrices $A$ and $B$ are similar if there is and invertible matrix $C$ such that
$$
A = C^{-1}BC
$$
<!-- \end{definition} -->

We want to see that two matrices are similar precisely when they represent the same linear transformation. Choose two bases for the vector space $V$, say ${v_1, \ldots, v_n}$ (the $v$ basis) and ${w_1, \ldots, w_n}$ (the $w$ basis). Let $A$ be the matrix representing the linear transformation $T$ for the basis and let $B$ be the matrix representing the linear transformation for the $w$ basis. We want to construct the matrix $C$ so that $A = C^{-1}BC$.

Recall that given the $v$ basis, we can write each vector $z \in V$ as an $n \times 1$ column vector as follows: we know that there are unique scalars $a_1, \ldots, a_n$ with
$$
z = a_1 v_1 + \dots + a_n v_n
$$
We then write $z$, with respect to the $v$ basis, as the column vector:
$$
\begin{pmatrix}
a_1 \\
\vdots \\
a_n
\end{pmatrix}
$$
Similarily, then are unique scalars $w_1, \dots,  w_n$ so that
$$
z = b_1 w_1 + \dots + b_n w_n,
$$
meaning that with respect to the $w$ basis, the vector $z$ is the column vector:
$$
\begin{pmatrix}
b_1 \\
\vdots \\
b_n
\end{pmatrix}
$$

The desired matrix $C$ will be the matrix such that
$$
C
\begin{pmatrix}
a_1 \\
\vdots \\
a_n
\end{pmatrix}
=
\begin{pmatrix}
b_1 \\
\vdots \\
b_n
\end{pmatrix}.
$$
If $C = (c_{ij})$, then the entries $c_{ij}$ are precisely the numbers which yield:
$$
w_i = c_{i1} v_1 + \dots + c_{in} v_n.
$$
To commute, meaning that $CA = BC$ or 
$$
A = C^{-1}BC,
$$
as desired.
Determining two matrices are similar is a type of result that shows throughout math and physics. Regularly you must choose some coordinate system (some basis) in order to write down anything at all, but the underlying math or physics that you are interested in is independent of the initial choice. The key question becomes: what is preserved when the coordinate system is changed? Similar matrices allow us to understand these questions. \nameref{def:decomposition}



## Eigenvalues and Eigenvectors



