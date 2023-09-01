## Prerequisites
* [Antiderivatives](./calculus.md#anti-derivative) via Reverse Power Rule
* [Definite Integral](./calculus.md#definite-integral)

## Numeric Differentiation 
### Forward
$$
\frac {fx_{i+1} - fx_i} {h}
$$
### Backward
$$
\frac {fx_i - fx_{i+1}} {h}
$$
### Centered
$$
\frac {fx_{i+1} - fx_{i-1}} {2h}
$$  

## Numeric Integration 
### Trapezoidal Rule
$$
\begin{aligned}
let\;n &= \#\;of\;values\;used\\
let\;h &= \frac{b-a}{n}\\
\int^b_ay\:dx&\approx \frac{1}{2}h\left[y_o+2(y_1+\:...\:+y_{n-1})+y_n\right]\\
\end{aligned}
$$
### Simpson's Rule | Prismoidal Theorem
1. Simple
$$
\begin{aligned}
h &= \frac{b-a}{2}\\
x_0 &= a\\
x_1 &= \frac{a+b}{2}\\
x_2 &= b\\
For\;&each\;x, f(x)\;to\;get\;y_i:\\
\int^b_ay\:dx&\approx \frac{1}{3}h(y_o+4y_1+y_2)\\
\end{aligned}
$$
2. Composite 
$$
\begin{aligned}
\int_a^by\:dx\approx\frac{h}{3}\left(y_0+4y_1+2y_2+4y_3+2y_4+...\:+4y_{n-1}+y_n\right)
\end{aligned}
$$