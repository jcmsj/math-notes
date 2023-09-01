## Inference Laws ##

<div>
__Modus Ponens (MPP)__
```
p -> q
p
-------
∴ q
```
</div>

__Modus Tollens (MTT)__
```
p -> q      | ~q -> ~p
~q          | ~q
------      | -------
∴ ~p        | ∴ ~p
```

Note: think of this as taking MPP of the contrapositive (see right side)

__Hypothetical Syllogism (HS)__
```
p -> q
q -> r
-------
∴ p -> r
```

Note: Similar to transitivity.

__Disjunctive Syllogism (DS)__
```
p v q
~p
-------
∴ q
```

__Addition (Add) | Or Introduction (vI)__
```
p
----
∴ pvq
```
__Simplification (Simp) | And elimination (^E)__
```
p^q
----
∴ p
∴ q
```

Note: Always bring down leftmost var first

__Conjunction | And Introduction (^I)__
```
p
q
---
∴ p^q
```

__Absorption__
```
p->q
---
∴ p->(p^q)
```

__Constructive Dilemma (CD)__
```
(p->q)^(r->s)     | 1. p->q
pvr               | 2. r->s
-------------     | 3. pvr
∴ qvs             | ∴ qvs
```

Note: Applies MPP to #1 #2 to get a conclusion from #3

__Destructive Dilemma (DD)__
```
(p->q)^(r->s)       | 1. p->q
~qv~s               | 2. r->s
-------------       | 3. ~qv~s || ~(q^s)
∴ ~pv~r             | ∴ ~pv~r
```

Note: Applies MTT to #1 #2 to get a conclusion from #3

