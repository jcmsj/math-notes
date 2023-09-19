## Relations
### Properties
| Property             | Explanation                       |
| -------------------- | --------------------------------- |
| Reflexive            | Each x in X refs itself           |
| Symmetric            | (a,b) ∈ R -> (b,a) ∈ R            |
| Antisymmetric        | x refs y but y doesn't unless x=y |
| Transitive           | Va,b,c ∈ A, aRb ^ bRc -> aRc      |
| Partial Order        | R & A & T                         |
| Equivalence Relation | R & S & T                         |

1. __Reflexive__: 
   1. A relation R of set A is reflexive if V a ∈ A, (a,a) ∈ R 
   2. Va∈A((a,a) ∈ R).
   3. xRx, Vx ∈ A
2. __Symmetric__: 
   1. A relation R of set A is symmetric if (b, a) ∈ R whenever (a, b) ∈ R for all (a, b) ∈ A. 
   2. A pair (a,b) and its mirror (b,a) are both in R.
   3. VaVb((a,b) ∈ R -> (b,a) ∈ R)
   4. Vx,y ∈, xRy -> yRx
   5. when false: Ea,b ∈ A, (a,b) ∈ R -> (b,a) /∈ R
   6. (a,b) ∈ R -> (b,a) ∈ R
4. __Antisymmetric__: 
   1. When a mirror (b,a) of the pair (a,b) is in R, then it is antisymmetric.
   2. [(a,b) ∈ R  ^ (b,a) ∈ R ] -> (a=b)
   3. Negation: E(a,b),(b,a) ∈ R, a !=b
5. __Transitive__: 
   1. A relation R on a set A is transitive if whenever (a, b) ∈ R and (b,c) ∈ R, then (a, c) ∈ R, for all a,b,c ∈ A.
   2. [(a,b)^(b,c)] -> (a,c) ∈ R
   3. Va,b,c ([(a,b) ∈ R ^(b,c) ∈ R] -> (a,c) ∈ R)
   4. Va,b,c ∈ A, aRb ^ bRc -> aRc
6. __Equivalence relation__: Is Reflexive, Symmetric, & Transitive
7. __Partial Order Relation__ | __poset__: Is Reflexive, Antisymmetric, & Transitive
8. __Inverse__: Flip all pairs

9. __Composition__: 
   1. 𝑅<sub>1</sub> ∘ 𝑅<sub>2</sub> = {(𝑥,𝑧) | (𝑥,𝑦) ∈ 𝑅<sub>2</sub> 𝑎𝑛𝑑 (𝑦,𝑧) ∈ 𝑅<sub>1</sub> for some 𝑦 ∈ 𝑌}
   2. Like transitivity; JOIN (a,c) where a,b is from R2 and b,c is from R1.
   3. Notice that we start with the latter relation.
   * Example:
      <br> R1 {(1,3), (2,1), (3,4), (4,6))
      <br> R2 = {(1,5), (2,3), (3,4), (4, 1), (5,3), (6,2))
      <br> 𝑅<sub>1</sub> ∘ 𝑅<sub>2</sub> = {(2,4),(3,6),(4,3), (5,4), (6,1)}
10. __Equivalence Class__:
That of x is denoted by [x] = {y | y ∈ A and (x,y) ∈ R}
### Digraphs
1. Illustrates a relation.
2. Reflexive - an element points to itself.
3. Symmetric - two elements points to each other or reflexive.
4. Antisymmetric - An element points to another but the other does not point back unless reflexive.
5. Transitive - Element a points to b and b points to c.

### Identies
![Identity chart](./identities.PNG)
