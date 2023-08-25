
# Table of Contents

1.  [Recall Lecture 1](#org81b1858)
2.  [Conditional Complete](#orgfa1313a)
3.  [Algebra](#org5fd8503)
    1.  [Comments](#org7c31400)



<a id="org81b1858"></a>

# Recall Lecture 1

-   $\mathbb{D}$ The east upper bound of A \subseteq S is the least element of the set {all UBs of A}.  
    The lub may not exist; when it does, it is unique.
-   Notation: sup(A) or lub(A)
-   sup(A) needn&rsquo;t lie in A.  
    $\mathbb{E}$ Let S = $\mathbb{P}(X)$, |X| > 1, A = {all **proper** subsets of X} &rArr; A $\subsetneq$ S. In this case, sup(A) = X &notin; A.
-   If sup(A) &isin; A, then sup(A) is the greatest or largest element of A.
-   **THM**: for (S, &le;), IF each nonempty subset of S that is bounded above has a sup, THEN, each nonempty subset of S that is bounded below has an inf.
    
    <div class="proof" id="orgff86943">
    <p>
    Let A be a nonempty subset of S that is bounded below. Let B be the set of LBs for A, and B &sub; S.<br />
    A is bounded below &rArr; B &ne; &empty; <br />
    A &ne; &empty; &rArr; B is bounded above by any a &isin; A.<br />
    Let sup(B) = &gamma;. We claim that &gamma; is a LB for A, i.e. &forall; a &isin; A, &gamma; &le; a.<br />
    This claim implies that &gamma; &isin; B, sup(B) &isin; B.<br />
    By \(\mathbb{D}\) B, let a &isin; A, then &forall; b &isin; B, b &le; a. In other words, a is an UB for B.<br />
    Thus, &gamma; &le; a because &gamma; is the least UB.<br />
    By the previous note, &gamma; is the greatest element of B, i.e. the greatest lower bound of A.
    </p>
    
    </div>


<a id="orgfa1313a"></a>

# Conditional Complete

-   This is equivalent to the least UB property.
-   $\mathbb{D}$ The ordered set S is call **conditional complete** (or has the least UB property) iff it satisfies the hypothesis/conclusion of the previous theorem.
-   $\mathbb{E}$ $\mathbb{P}(X)$ is complete.
    -   Let A \subseteq $\mathbb{P}(x)$, here A is called a family of sets, i.e. whose elements are sets.  
        Then sup(A) = $\bigcup$ A, inf(A) = $\bigcap$ A, where $\bigcup$ A denotes the union of all sets in A.  
        Note that $\bigcap$ &empty; = X, and $\bigcup$ &empty; = \empthset


<a id="org5fd8503"></a>

# Algebra

$\mathbb{D}$ A field of a set F with operations &ldquo;+&rdquo; and &ldquo;&times;&rdquo; satisfying:

-   Additative axioms:
    1.  a + b = b + a;
    2.  a + (b + c) = (a + b) + c;
    3.  $\exists$ 0 &isin; F s.t. 0 + a = a = a + 0;
    4.  &forall; a, &exist; -a s.t. (-a) + a = 0 = a + (-a)
-   Multiplicative axioms:
    1.  ab = ba;
    2.  a(bc) = (ab)c;
    3.  &exist; 1 &isin; F s.t. 1a = a = a1;
    4.  &forall; a &ne; 0, &exist; \frac{1}{a} s.t. \frac{1}{a}a = 1 = a\frac{1}{a}
-   Other axioms:
    1.  a(b+c) = ab + ac;
    2.  0 &ne; 1


<a id="org7c31400"></a>

## Comments

-   if z + z = z, then z = 0  
    pf: -z + (z + z) = -z + z &rArr; (-z + z) + z = -z + z &rArr; 0 + z = 0 &rArr; z = 0.
-   0z = 0
-   The commutativity in addition axioms is redundant.
-   If we replace the distributivity by c(b+a) = ac + bc, then not only the addition axioms&rsquo; commutativity is redundant, but also the multiplicative commutativity is redundant.

