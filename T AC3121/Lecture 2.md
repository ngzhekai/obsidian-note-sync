# Finite Fields And Computational Number Theory

## Section 1: Group, Ring & Field

### Group

A set of elements or "numbers"
With some operation whose result is also in the set (closure)

* Obey: 
	* Associative law:  ***(a.b).c = a.(b.c)***
	* Has identity *e*: ***e.a = a.e = a***
	* Has inverses *a<sup>-1</sup>* : ***a.a<sup>-1</sup> = e***
* If commutative    ***a.b = b.a***
	* then forms an **Abelian group**

### Cyclic Group

Define **exponentiation** as repeated application of operator

* Example : ***a<sup>3</sup> = a.a.a***
* A group is cyclic if every element is a power of some fixed element, i.e. ***b = a<sup>k</sup>*** for some *a* and every *b* in the group.
* *a* is said to be a generator of the group.

### Ring

A set of "numbers". Having two operations (addition and multiplication) which form: 
* An abelian group with addition operation
* and multiplication
	* has closure 
	* is associative
	* distributive over addition: ***a(b+c) = ab + ac***
* If multiplication operation is commutative, it forms a **commutative ring**
* If multiplication operation has an identity and no zero divisors, it forms an **integral domain**

### Field

A set of numbers. Having two operations which form:
* abelian group for addition
* abelia group for multiplication (ignoring 0)
* ring

Have hierarchy with more axioms/laws
* group -> ring -> field