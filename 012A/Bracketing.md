## Bisection
$$
\begin{aligned}
let\;c= \frac{x+y}{2}\\
if\;abs\;f(c)\;&<doa:\\
return\;c\\
if\;f(c) < 0:\\
then\;repeat&\;x = c\\
else\;repeat&\;y = c\\
\end{aligned}
$$
## Regula-Falsi
* Like Bisection but c is calculated with:
  $$
  c\;=\;y-\;f(y)*\;\frac{y-x}{f(y)-f(x)}
  $$
## Graeffe's
roots = do descartes
For i in range roots
split EQ nto odds = evens
replace x^2 with y

For i in range roots
 Solve for each var using an EQ where arg = EQ's nth term coef / EQ's n-1th term coef