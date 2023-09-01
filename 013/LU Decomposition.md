
## About
* Most efficient algorithm for solving [SLEs](Linear%20Algebra.md#sle)
* Also applied for cryptography.

## Algorithm
* Ax = b; A = LU.
1. Solve Ax = b
2.	Calc [[matrix#Types|Upper triangle]] of A using [[eliminations#Elemetary Row Operations|EROs]].
3.	For each ERO done get the [[matrix#Types|Elementary matrix]].
4.	Combine all elementary matrices generated to create the [[matrix#Type|Lower triangular matrix]].
5.	Solve Ly = b with forward substitution.
6.	Solve Ax = y with backward substitution.
7.	The column vector x will be the solution set.
