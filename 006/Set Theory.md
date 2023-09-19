# Set Theory
## Introduction
German mathematician G. Cantor introduced the concept of sets. He had defined a set as a
collection of definite and distinguishable objects selected using certain rules or description.
### SET
* Is a collection of well defined objects. 
* Denoted by capital letters of the alphabet and its members are enclosed with brackets.
When talking about sets, it is fairly standard to use Capital Letters to represent the set, and
lowercase letters to represent an element in that set.
Elements — are the members or objects of the set which is denoted by a symbol (E

### Representation
1. Roster Method | Tabular Form
2. Rule method | Set Builder Notation

### Order | Cardinality
1. __Cardinal Number__ - Set's size.
2. __Symbolized__ - n(A) or |A|; where A is the set's name.

### Types
1. Finite 
2. Infinite
3. Unit set - n(A) = 1
4. Empty set | Null set - {} | Ø
5. Universal set - Totality of the set; Where the set is assumed to be part of a larger set __U__.
6. Subset
   1. Improper subset - maybe A == B; A __<u>&lt;</u>__ B
   2. Proper subset - Unequal subset | A __<__ B
7. Equal set
8. Equivalent set | ~ - Sets of equal size
9. Disjoint set | Non-intersecting set

### Operations
1. __Union__: Combination
2. __Intersection__: Vx in A & B
3. __Difference__: Vx in A not in B
4. __Complement__: U - A
5. __Cartesian Product__:  The Cartesian product of set A and B, written as A x B is the set of all possible ordered pairs with first element from A and second element from B. A x B = {(a, b)/ a ∈  A and b ∈ B }

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

## Functions
### Types
1. Injenctive | One-to-one | Injection - All domains are consumed.
2. Surjective | Onto | Surjection -> all ranges are consumed.
3. Bijective  | Bijections - Injective & Surjective.
4. General - Neither one-to-one nor onto.

<details>

<summary>
Challenge
</summary>
Let A ={1,2,3}

1. R = ((1,2), (2,1), (1,1), (2,2)}
1. R = {(1,2), (2,3), (1,3)}
1. R = ((1,1), (2,2), (3,3), (1,2)}
   | Property      | Value | Reason                                       |
   | ------------- | ----- | -------------------------------------------- |
   | Reflexive     | T     | Va ∈ A((a,a) ∈ R)                            |
   | Symmetric     | F     | (1,2) fails Va,b ∈ A((a,b) ∈ R -> (b,a) ∈ R) |
   | Antisymmetric | T     | Va,b ∈ A [(a,b) ∈ R  ^ (b,a) ∈ R ] -> (a=b)  |
   | Transitive    | T     | Va,b,c ∈ A[(a,b) ∈ R^(b,c) ∈ R] -> (a,c) ∈ R |
2. R = {(2,3), (1,2), (1,1)}
3. R = {(2,3)}
4. R = {(1,2), (2,1)}

5. R = {(1,1), (2,2), (3,3)}
6. R = {(1,1), (2,1), (1,1), (2,2)}
7. R = {(3,1), (1,3), (2,3)}
8. R = {(1,2), (2,3), (1,3)}
9.  R = {(2,3), (3,2), (2,2), (3,3)}
10. R = {(1,1), (2,2), (2,3), (1,3)}

Given:
1. R = null
1. R = {(1,1), (2,2), (3,3)}
1. R = {(1,1), (2,2), (3,3), (2,1)}
1. R = {(1,1), (1,3), (2,1), (3,1)}
1. R = ((1,1), (2,2), (3,3), (1,2), (1,3), (2,1), (3,1)}

1. R = {(1,1), (2,2), (3,3), (1,2), (2,1}
1. R = {(1,1), (2,2), (3,3), (1,3), (2,3)}
1. R = {(1,1), (1,2), (2,3), (1,3)}
1. R  = {(1,1), (1,3), (2,2), (2,3), (3,3)}
1. R = {(1,1), (1,2), (2,1), (2,3), (3,1), (3,2), (3,3)}
1. R = A x A
</details>