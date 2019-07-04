# 1.
## (a)
From the notes provided on class website, we know that
$\bigtriangledown_x x^TAx=2Ax$ &nbsp; &nbsp; &nbsp; and &nbsp; &nbsp; &nbsp; $\bigtriangledown_x b^Tx=b$

$\therefore\bigtriangledown_xf(x)=\bigtriangledown\frac{1}{2}x^TAx+\bigtriangledown_xb^Tx=Ax+b$

## (b)
$\bigtriangledown_xf(x)=
\bigtriangledown_xg(h(x))=
\begin{bmatrix}
\frac{\partial}{\partial x_1}g(h(x)) \\
\vdots \\
\frac{\partial}{\partial x_n}g(h(x))
\end{bmatrix}$

$=\begin{bmatrix}
g'(h(x))\frac{\partial h(x)}{\partial x_1} \\
\vdots \\
g'(h(x))\frac{\partial h(x)}{\partial x_n}
\end{bmatrix}=g'(h(x))\bigtriangledown_xh(x)$

## (c)
$\bigtriangledown^2_xf(x)=\bigtriangledown^2_x(\frac{1}{2}x^TAx+b^Tx)=\bigtriangledown^2_x\frac{1}{2}x^TAx+\bigtriangledown^2_xb^Tx$

$\because\bigtriangledown^2_x b^Tx=
\begin{bmatrix}
\frac{\partial^2}{\partial x_1\partial x_1}b^Tx\cdots\frac{\partial^2}{\partial x_1\partial x_n}b^Tx \\
\vdots \qquad\qquad \vdots \\
\frac{\partial^2}{\partial x_n\partial x_1}b^Tx\cdots\frac{\partial^2}{\partial x_n\partial x_n}b^Tx 
\end{bmatrix}=0$

$\bigtriangledown^2_x(\frac{1}{2}x^TAx+b^Tx)=\bigtriangledown^2_x(\frac{1}{2}x^TAx)=A$

## (d)
$\bigtriangledown_xg(a^Tx)=
\begin{bmatrix}
\frac{\partial}{\partial x_1}g(a^Tx) \\
\vdots \\
\frac{\partial}{\partial x_n}g(a^Tx)
\end{bmatrix}=
\begin{bmatrix}
g'(a^Tx)\frac{\partial a^Tx}{\partial x_1} \\
\vdots \\
g'(a^Tx)\frac{\partial a^Tx}{\partial x_n} 
\end{bmatrix}
$

$=g'(a^Tx)\bigtriangledown_x a^Tx=g'(a^Tx)a$

$\bigtriangledown_x^2g(a^Tx)=
\begin{bmatrix}
\frac{\partial^2}{\partial x_1 \partial x_1}g(a^Tx)\quad\cdots\quad\frac{\partial^2}{\partial x_1 \partial x_n}g(a^Tx)\\
\vdots \qquad\qquad\qquad\qquad \vdots\\
\frac{\partial^2}{\partial x_n \partial x_1}g(a^Tx)\quad\cdots\quad\frac{\partial^2}{\partial x_n \partial x_n}g(a^Tx)
\end{bmatrix}$

$=g''(a^Tx)\cdot
\begin{bmatrix}
a_1\cdot a_1\quad\cdots\quad a_1\cdot a_n\\
\vdots \qquad\qquad \vdots\\
a_n\cdot a_1\quad\cdots\quad a_n\cdot a_n
\end{bmatrix}$

$=g''(a^Tx)\cdot aa^T$

# 2.
## (a)
$\forall x,\quad x^TAx=\sum^n_{i=1}\sum^n_{j=1}A_{ij}x_ix_j$

$\because A_{ij}=z_iz_j$

$\sum^n_{i=1}\sum^n_{j=1}A_{ij}x_ix_j=\sum^n_{i=1}\sum^n_{j=1}z_iz_jx_ix_j$

$=\sum^n_{i=1}(z_ix_i)^2\geq0$

$\therefore$ A is positive semidefinite

## (b)
$A=\begin{bmatrix}
z_1z_1 \quad\cdots\quad z_1z_n\\
z_2z_1 \quad\cdots\quad z_2z_n\\
\vdots\\
z_nz_1 \quad\cdots\quad z_nz_n
\end{bmatrix}$

row operatins (row i multiply $z_1/z_i$)
$\rightarrow A=\begin{bmatrix}
z_1z_1 \quad\cdots\quad  z_1z_n\\
0 \quad\quad\cdots\quad\quad 0\\
\vdots\\
0 \quad\quad\cdots\quad\quad 0
\end{bmatrix}$

$\therefore$ rank of A equal 1

From the dimension theory, we know that $rank + nullity = n$

$\therefore$ dimenesion of null space is n - 1

Also, null space consists of orthogonal vectors of $z^T$, so $Ax=zz^Tx$ will be 0

## (c)
$\forall x, \quad x^TBAB^Tx = (xB^T)A(B^Tx)$

Let $\quad v = B^Tx$

$v^TAv\geq0$, since A is positive semidefinite.

$\therefore BAB^T$ is positive semidefinite.

# 3.
## (a)
Since Matrix $T$ is invertible, $A=T\Lambda T^{-1} \rightarrow AT=\Lambda T$

$\begin{bmatrix}
    At^{(1)} \quad At^{(2)} \cdots At^{(n)}
\end{bmatrix}=\begin{bmatrix}
\lambda^{(1)}t^{(1)} \quad \lambda^{(2)}t^{(2)} \cdots \lambda^{(n)}t^{(n)}
\end{bmatrix}$

$\therefore \forall i=1 \cdots n$, 
$At^{(i)}=\lambda t^{(i)}$

## (b)
