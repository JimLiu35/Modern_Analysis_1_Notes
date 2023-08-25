
# Table of Contents

1.  [Nomenclature](#orga56eae2)
2.  [Partial Order](#orgc469b97)
3.  [Strict Order](#org2e012d8)
4.  [Bounds](#orgd04dab6)



<a id="orga56eae2"></a>

# Nomenclature

-   $\mathbb{D}$ = Definition
-   $\mathbb{E}$ = Exercise or Example
-   $\bigvee$ = logic &ldquo;OR&rdquo;
-   $\bigwedge$ = logic &ldquo;AND&rdquo;
-   $\mathbb{M}$ = Personal Understanding


<a id="orgc469b97"></a>

# Partial Order

$\mathbb{D}$: A (partial) order on the set S is a relation &ldquo;&le;&rdquo; on S that is

1.  reflexive:
    -   What is Reflexive Relation?
        In set theory, a binary relation on A is said to be a **reflexive relation** if every element of the set is related to itself. For example, define a relation on the set of integers \mathbb{Z} as &rsquo;is equal to&rsquo;. Now, we know that each integer is equal to itself such as 0=0, 1=1, and so on. This implies every integer is related to itself. Hence, the relation &rsquo;is equal to&rsquo; on the set $\mathbb{Z}$ is a reflexive relation.
    -   $\mathbb{D}$: A binary relation R defined on a set A is said to be reflexive if, for every element a&isin; A, we have aRa, that is, (a,a) &isin; R.
    -   $\mathbb{M}$ if R is a relation and is defined for a set A, this relation is reflexive if aRa is true. $\mathbb{E}$ for integer set $\mathbb{Z}$, if R is defined as /leq, then since 1 &isin; $\mathbb{Z}$ and 1 &le; 1 is ture. Hence, R = &le; is a reflexive relation. Counter $\mathbb{E}$ if R is defined as <, then since 1 &isin; $\mathbb{Z}$ and 1 < 1 is false. Hence, < is not a reflexive relationship.
2.  antisymmetric: a &le; b $\bigwedge$ b leq a &rArr; a = b
3.  transitive: a &le; b $\bigwedge$ b &le; c &rArr; a &le; c

$\mathbb{D}$ &le; is **total** iff &forall; a,b &isin; S, a &le; b $\bigvee$ b &le; a


<a id="org2e012d8"></a>

# Strict Order

$\mathbb{D}$ A **strict order** on S is a relation < that is

1.  irreflexive;
2.  transitive: a < b $\bigwedge$ b < c &rArr; a < c.

Note: from PO (partial order) &harr; SO (strict order):

1.  &rarr;: Given &le;, $\mathbb{D}$ a < b := (a &le; b) $\bigwedge$ (a &ne; b)
    
    <div class="proof" id="org5f5a855">
    <p>
    (Proof via Definition)<br />
    </p>
    
    <ol class="org-ol">
    <li>Show &lt; is transitive, i.e. a &le; c \(\bigwedge\) a &ne; c: <br />
    Spse a &lt; b and b &lt; c, i.e. spse (a &le; b) \(\bigwedge\) (a &ne; b) \(\bigwedge\) (b &le; c) \(\bigwedge\) (b &ne; c),<br />
    &because; According to \(\mathbb{D}\) of partial order, &le; is transitive,<br />
    &there4; a &le; c <br />
    Spse a = c<br />
    Then 1. a &le; b and 2. b &le; a<br />
    &rArr; a = b (as &le; is antisymmetric)<br />
    but a &ne; b, \(\Rightarrow\!\Leftarrow\) <br />
    Thus, &lt; is transitive.</li>
    <li>Show &lt; is irreflexive<br />
    a &lt; a &rArr; (a &le; a) \(\bigwedge\) (a &ne; a)<br />
    (&not; (a &ne; a) is part of \(\mathbb{D}\))<br />
    Why? This proof seems trivial to me.这个地方到底证明了什么? &gt;的定义已经很明显了，为什么还要证明?</li>
    </ol>
    
    </div>
2.  &larr;: Given <, $\mathbb{D}$ a &le; b := (a < b) $\bigvee$ (a=b)

$\mathbb{E}$ X is any set, S = $\mathbb{P}(x)$ i.e. power set. For A, B &isin; S, A &le; B := A \subseteq B defines a partial order. Is it total?  
Ans: not aways. It is not total when and only when |x| &le; 1.  
Note: Rudin only considers total strict orders, coz Rudin says &ldquo;order is transitive and trichotomous (i.e. a < b $\bigvee$ a = b $\bigvee$ a > b )&rdquo;


<a id="orgd04dab6"></a>

# Bounds

-   $\mathbb{D}$ Let <  be an order on S, say a &isin; S is **greatest** iff &forall; s &isin; S, s &le; a.
-   $\mathbb{E}$ How many greatest elements do S contain?
    Ans: There may be none. e.g. let S = $\mathbb{P}(x)\setminus\{x\}$ where $\mathbb{P}(x)$ denotes the power set of x. If there are greatest element, it will be unique.
-   $\mathbb{D}$ Let (S, &le;) be given and A \subseteq S. b &isin; S is an upper bound for A iff &forall; a &isin; A, a &le; b, and b needn&rsquo;t be an element of A.  
    We say A is bounded above iff such a b exists.
-   $\mathbb{D}$ Given (S, &le;), the **least upper bound** of A in S is the [least] [upper bound] of A in S, when such exists.   
    Note: the set of UBs for A may not have a least element. If it has one, it is unique and called the supremum of A (sup(A) or lub(A)).  
    Similar concepts exist for the greatest lower bound: inf(A) or glb(A).
-   **THM**: for (S, &le;), IF each nonempty subset of S that is bounded above has a lub, THEN, each nonempty subset of S that is bounded below has a glb.

