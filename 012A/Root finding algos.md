## Successive Substitution
1. Make $x = g(x)$
2. Find $a$ & $b$ such that $a<b\:$ and $f\left(a\right)\ast f\left(b\right)<0$.
3. 
$$
x_1 = g(x_0)\\
x_2 = g(x_1)\\
x_3 = g(x_2)\\
...
$$
4. Repeat #2 & #3 until $\left|x_i-x_{i-1}\right|\approx0$
## Newton-Raphson
1. Find $a$ & $b$ such that $a<b\:$ and $f\left(a\right)\ast f\left(b\right)<0$.
2. $x_0 = \frac{a+b}{2}$
3. $x_1=x_0-\frac{f\left(x_0\right)}{f'\left(x_0\right)}$

## Secant method

1. Find $x_0, x_1$ where $x_0<x_1$ and  $f(x_0)*f(x_1)<0$
2. Take the interval $[x_0, x_1]$, then find next $x$.
3. 
$$
x_2=x_1-f\left(x_1\right)\left[\frac{x_1-x_0}{f\left(x_1\right)-f\left(x_0\right)}\right]
$$
4. Repeat 2 & 3 until:
$$
f(x_n) = 0\;or\;|f(x_n)| < DOA
$$