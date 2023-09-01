**Diagonally dominant** - Target cell is <= the sum of the absolute values of the other cells in a row.
## Gauss-Jacobi
1. Arrange [SLEs](./MATH013/Linear%20Algebra.md) into diagonally dominant.
2. Isolate one unknown for each equations.
3. Initialize a value for the unknowns of zero using __PREVIOUS ITERATION__ state.
4. Iterate until unknowns stop diverging.

## Gauss-Seidel
* Like jacobi but iteration differs.
* Use latest state instead.