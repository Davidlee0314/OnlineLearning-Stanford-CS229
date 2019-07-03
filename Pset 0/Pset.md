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
