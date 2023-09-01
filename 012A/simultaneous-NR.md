# Solutions of simultaneous Nonlinear Equations w/ Newton Raphson 

## Prerequisites 
1. Partial derivative
2. Determinants 
3. NR method 
## Using NRM 

## Steps 
1. Given:
$$
\begin{aligned}
ax_2&+bx_2...kx_n
\end{aligned}
$$
1. Equate EQs to 0.
2. For each EQ, get partial derivatives for each variable
	E.g. $f_x, f_ y$ 
3. For each EQ: $x_0, y_0$
	1. $\\f_0 = f(a,b)\\g_0 = g(a,b)$
4. $
D = \begin{bmatrix} f(x_0) & f(y_0)
           \\g(x_0) & g(y_0)
		   \end{bmatrix}$
1. $
D_x = \begin{bmatrix} f_0 & f_0
           \\g_0 & g_0
		   \end{bmatrix}
$
1. $D_y = \begin{bmatrix} f(x_0) & f_0
           \\g(x_0) & g_0
		   \end{bmatrix}$
2. $h = -(Dx\div D)$
3. $k = -(Dy\div D)$
4. $x_1 = x_0+h$
5. $y1 = y0 + k$
6. $f(x_1, y_1) < DOA$
7. $g(x_1, y_1) < DOA$
8. Repeat if false


$$
x_{n+1} = x-\frac u{y'}
$$