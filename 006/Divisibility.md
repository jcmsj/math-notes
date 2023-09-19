# Divisibility

# Congruence Modulo
## Theorems
Let m be a positive integer, if a b(mod m) and c = d(mod m), then
1. a ± c ≡ b ± d(mod m)
2. ac ≡ bd (mod m)
3. a<sup>k</sup> ≡ b<sup>k</sup> (mod m), Vk E N
4. a b(mod m) ≡ a(mod m) b(mod m)

Let m > 1 be fixed and a, b, c, d be arbitrary integers. Then Congruence Modulo m is an
equivalence relation.
* __Reflexive__: a ≡ a (mod m) V a
* __Symmetric__: a ≡ b (mod m) -> b≡a (mod m)
* __Reflexive__: a ≡ b (mod m) ^ b≡c (mod m) -> a c (mod m)
* __Equivalence__: a ≡ b (mod 0) -> a = b
<details>
<summary>
Challenge
</summary>
<pre>
C≡24-25 (mod 9)
C≡6*4-5*5 (mod 9)
C (mod 9) = -1 (mod 9)
C (mod 9) = 8 (mod 9)
C=8

158=17 * 9 + 5

a=bq+r
1780=135*13+25
135=25*q+r
</pre>
</details>

## Algorithms
### Division
  a = bq + r
### GCD via Euclidian
1. Given a,b use div algo
2. after every iteration a = b, b = r
3. Repeat division algo until r = 0
4. the GCD is r from the 2nd to the last iter.
#### Properties
1. gcd(a,b) = gcd(b,a)
2. x > 0 -> (gcd(ax,bx) = x * gcd(a,b))
3. (d = gcd(a,b)) -> (gcd(a|d,b|d)=1)
4. VxE Z, gcd(a,b) = gcd(a,b+ax)

### LCM
ab / gcd(a,b)

### Check if a & b are coprime
* coprime - a & b's gcd's are prime

### Remainder of large numbers
2<sup>524</sup>	&#247; 3
2**254 ≡ -1 (mod 3)

### Last n-digits of large numbers
<details>
<summary>Worked example</summary>
2**524?
2^n ≡ 1 (mod 10)
2^0 ≡ 1 (mod 10)
2^

2^-1
2^n+1^n≡ 1 + 1^n (mod 10)
(2^0)^524≡1^524 (mod 10)
2^0 * 2^524≡1 * 1^524(mod 10)
2^524≡1*1(mod 10)
2^524≡1(mod 10)
Therefore: unit digit is 1

Solving 2^n:
Pattern: unit digit of 2^n where n > 0 cycles between 2,4,8,6
2^1≡ 2 (mod 10)
2^2≡ 4 (mod 10)
2^3≡ 8 (mod 10)
2^4≡ 6 (mod 10)
2^5≡ 2 (mod 10)
2^6≡ 4 (mod 10)
2^7≡ 8 (mod 10)
2^8≡ 6 (mod 10)
2^9≡ 2 (mod 10)
2^10≡ 4 (mod 10) 
....
2^n ≡ 2^u (mod 10); let u be the unit digit of n but if n = 0, then consider it as 10.

So the unit digit of 2^524 is solved by:
let: 
    n = 524
    u = 524 % 10 = 4

Hypothesis:  if n > 0, then unit digit of 2^n follows the pattern 2,4,8,6,...,2,4,8,6.

Basis step(s):
2^1≡ 2 (mod 10)
2^2≡ 4 (mod 10)
2^3≡ 8 (mod 10)
2^4≡ 6 (mod 10)
2^5≡ 2 (mod 10)
2^6≡ 4 (mod 10)
2^7≡ 8 (mod 10)
2^8≡ 6 (mod 10)
2^9≡ 2 (mod 10)
2^10≡ 4 (mod 10) cd 
2^n ≡ 2^u (mod 10)
2^524 ≡ 2^4 (mod 10)
(2^4)^131 ≡ 6 (mod 10)
2^524 ≡ 6 (mod 10)
Therefore: unit digit of 2^254 is 6.

Formal proof: 
to get the unit digit of 2^n take unit digit of n.
Say: 2^524 becomes 2^4, from the expressions earlier we know that the unit digits of 2^4 and 2^8 is 6. From that it can be observed that multiples of 4 have unit digits of 6. Therefore, since the exponent 524 is a multiple of 4 its unit digit is 6.

Inductive Step:
(2^1 % 10), (2^2% 10),
(2^3 % 10), (2^4% 10)
...,(2^n % 10) = 2,4,8,6...,(2^u)
let u be unit digit of n but if u is 0 treat it as 10).

Proof: 2^
</details>

### Number system conversion
1. DEC->Base-n - 
   1. apply euc, let a = dec, b=base-n for 1st iter.
   2. Repeat until q is 0, then bin digits would be r of each iter where nth place value is nth iter's r | place r R->L read from Bot->Top.