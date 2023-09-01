# Gaussian & Gauss-Jordan Elimination
## About
* Named after Carl Friedrich Gauss
* Improved by Wilhlem Jordan
* Elimination method - Based on removing some variables by adding multiples of one equation to another.  
* Matrix conversion into its Reduced / Row-Echelon Form.

## Elemetary Row Operations
* Swap two rows (i, j).
* c x row; let c != 0
* Add a multiple of one row to another

## REF properties
* All rows whose elements are zero are located at the bottom.
* For each row, the first nonzero entry is 1 (called a leading 1).
* Two successive (nonzero) rows, the leading 1 of the higher row is farther to the left than the leading 1 in the lower row.
* RREF if every column containing a leading 1 contains zeros. 
### Steps:
* Write the augmented matrix of the SLEs.
* Apply [[#Elemetary Row Operations|ERO]] towards [matrix](./matrix.md).
* Write the SLE’s corresponding to the matrix (ref).
* Find solution via back-substitution.