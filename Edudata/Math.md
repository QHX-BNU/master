https://github.com/hendrycks/math
# Description
josn 文件
七大类：
1. algebra
2. counting and probility
3. geometry
4. intermediate algebra
5. number_theory
6. prealgebra
7. precalculus

| Field    | Annotation                  | Example                   |
| -------- | --------------------------- | ------------------------- |
| problem  | the content of the problem  | [[Math#tip1]]latex语法，需要转换 |
| level    | the level of the problem    | Level 4                   |
| type     | the type of the problem     | Precalculus               |
| solution | the solution to the problem | [[Math#Tip2]]             |
# tip1
Let
$$
{A} = 
\begin{pmatrix}
0 & 1 & 2 \\
1 & 0 & 1 \\
2 & 1 & 0 \
\end{pmatrix}.
$$
There exist constants $p$, $q$, and $r$ such that
\
$$
{A}^3 + p {A}^2 + q {A} + r {I} = {0}
$$
where $\\bold{I}$ and $\\bold{0}$ are the $3\times3$ identity matrix and zero matrix, respectively.  Enter the ordered triple $(p,q,r).$
# Tip2
We see that
$$
{A}^2 = 
\begin{pmatrix} 
0 & 1 & 2 \\
1 & 0 & 1 \\
2 & 1 & 0 
\end{pmatrix} 
\begin{pmatrix} 
0 & 1 & 2 \\
1 & 0 & 1 \\
2 & 1 & 0 \\
\end{pmatrix} = 
\begin{pmatrix} 
5 & 2 & 1 \\
2 & 2 & 2 \\
1 & 2 & 5 
\end{pmatrix}
$$
and
$$
{A}^3 = 
\begin{pmatrix}
0 & 1 & 2 \\
1 & 0 & 1 \\
2 & 1 & 0 
\end{pmatrix} 
\begin{pmatrix} 
5 & 2 & 1 \\
2 & 2 & 2 \\
1 & 2 & 5 
\end{pmatrix} = 
\begin{pmatrix} 
4 & 6 & 12 \\
6 & 4 & 6 \\
12 & 6 & 4 
\end{pmatrix}.
$$Thus, we want $p$, $q$, and $r$ to satisfy
$$
\begin{pmatrix} 
4 & 6 & 12 \\
6 & 4 & 6 \\
12 & 6 & 4 
\end{pmatrix} +
p \begin{pmatrix} 
5 & 2 & 1 \\
2 & 2 & 2 \\
1 & 2 & 5 \\
\end{pmatrix} +
q \begin{pmatrix}
0 & 1 & 2 \\
1 & 0 & 1 \\
2 & 1 & 0 
\end{pmatrix} + 
r \begin{pmatrix} 
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1 
\end{pmatrix} = 
\begin{pmatrix} 
0 & 0 & 0 \\
0 & 0 & 0 \\
0 & 0 & 0 
\end{pmatrix}.
$$The left-hand side is equal to
$$
\begin{pmatrix} 
5p + r + 4 & 2p + q + 6 & p + 2q + 12 \\
2p + q + 6 & 2p + r + 4 & 2p + q + 6 \\
p + 2q + 12 & 2p + q + 6 & 5p + r + 4 
\end{pmatrix}.
$$This gives us the system of equations
$$
\begin{align*}
5p + r &= -4, \\
2p + q &= -6, \\
p + 2q &= -12, \\
2p + r &= -4.
\end{align*}
$$
Solving this system, we find $(p,q,r) = \\boxed{(0,-6,-4)}.$
Note: The polynomial $x^3+px^2+qx+r$ is the characteristic polynomial of the matrix $\\mathbf A.$
