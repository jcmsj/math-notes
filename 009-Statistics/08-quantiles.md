# Quantiles
## Types
1. __Quantile | Q__ - 4 equal parts.
2. __Decile | D__ - 10 equal parts.
3. __Percentile | P__ - 100 equal parts.
## Ungrouped formula
$$
\begin{aligned}
&\cfrac{k}{N}(n+1) \\
&\text{where:} \\
k &= \text{target quantile} \\
N &= \text{type} \\
n &= \text{data size}
\end{aligned}
$$

### Example
$$
\begin{aligned}
Q_1 = \dfrac{1}{4}(n+1)
\end{aligned}
$$

## Grouped
1. Quantile class $P_k$: <br>
   $raw = \cfrac{k}{P}n\\$
   $P_k =$class interval with __cf__ >= __raw__<br>
   where: <br>
    P = is a [type](#types)
    
2. $lb_{P_k} + \left[ i \cfrac{ raw - <cf}{\displaystyle f_{\displaystyle p_k}} \right]$ <br>
    where
    * $lb_{P_k}$ =lower class boundary of quantile class
    * &lt;cf = cumulative frequency that is less than the quantile class
    * f = frequency of quantile class
    * i = class interval
