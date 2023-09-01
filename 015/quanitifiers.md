
* let x = dogs
* let Px = are brown

De morgan's law of Quantifiers:
~VxPx == Ex~Px
~ExPx == Vx~Px
    
VxPx <-> ~Ex~Px
* L: All dogs are brown.
* R: There is no dog that is not brown.

ExPx <-> ~Vx~Px
* L: There exists a dog that is brown.
* L: Some dogs are brown.
* R: Not all dogs are not brown.
 
~VxPx <-> Ex~Px
* L: Not all dogs are brown.
* R: There is a dog that is not brown.
* R: Some dogs are not brown.

~ExPx <-> Vx~Px
* L: There is no dog that is brown
* R: All dogs are not brown.

<pre>
VxEy[P(x,y)^Q(y)]
-V-E  
ExVy [~P(x,y)v~Q(y)]
</pre>