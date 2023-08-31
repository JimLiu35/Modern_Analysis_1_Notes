
# Table of Contents

1.  [Minimal](#orgd0ba902)
2.  [Least vs Minimal](#orga75d778)
3.  [Compatibility](#orge1591a3)
4.  [Negative Elements](#orge8d3ca7)



<a id="orgd0ba902"></a>

# Minimal

-   $\mathbb{D}$ B is an ordered set, say $ \alpha \in B $ is minimal iff $ \forall x \in B, (x \leq \alpha \Rightarrow x = \alpha) $.
-   Claim: Let B be the set of all upper bds for $ A \subseteq S $. For $ \alpha \in B $, the following are equivalent.
    1.  $ \alpha $ is minimal;
    2.  $ \forall x (x < \alpha \Rightarrow x \notin B) $ This is Rudins $\mathbb{D}$ of least UB.
-   Proof of the Claim:  
    We want to show that $ x < \alpha \Rightarrow x \notin B $ is equivalent to $ \alpha $ is minimal, i.e. $ x < \alpha \Rightarrow x \notin B \equiv x \in B \Rightarrow (x \leq \alpha \Rightarrow x = \alpha) $   
    From right to left:  
    $ x \in B \Rightarrow (x \leq \alpha \Rightarrow x = \alpha)$
    $ \equiv (x \in B $ $\bigwedge$ $ x \leq \alpha) \Rightarrow x = \alpha $   
    $ \equiv (x \leq \alpha \bigwedge x \in B) \Rightarrow x = \alpha $  
    $ \equiv x \leq \alpha \Rightarrow (x \in B \Rightarrow x = \alpha) $  
    $ \equiv x \leq \alpha \Rightarrow (x \neq \alpha \Rightarrow x \notin B ) $  
    $ \equiv x \leq \alpha \bigwedge x \neq \alpha \Rightarrow x \notin B $  
    $ \equiv x < \alpha \Rightarrow x \notin B $


<a id="orga75d778"></a>

# Least vs Minimal

-   THM: Least $ \Rightarrow $ Minimal. In a total ordered set, Least $ \Leftrightarrow $ Minimal.
    -   $\mathbb{M}$ For partially ordered set S, if $ s \in S $ is the least element, then it is also a minimal element. In a total order set S, if $ s \in S $ is a minimal element, then it is also a least element and vice versa.
    -   $\mathbb{M}$ For a poset, if there exists a least element, then it is unique. Set $ \{0, 0, 1\} $ is not a counterexample becaues according to the $\mathbb{D}$ of set, &ldquo;In mathematics, a set is defined as a collection of **distinct**, well-defined objects forming a group.&rdquo;, $ \{0, 0, 1\} \equiv \{0, 1\} $. Hence, the least element is still unique!
    -   $\mathbb{M}$ in a poset, minimal element may not unique. For example:  
        
            C1 C2 C3 C4 C5 C6
              \ | /    \ | /
               \|/      \|/
                B1      B2
                 \     /
                  \   /
                   \ /
                    A
        
        In this case, if we define set S s.t. S contains all sets above A. Then B1 and B2 are the minimal elements of set S. Here, $ A \leq B = A \subseteq B $.


<a id="orge1591a3"></a>

# Compatibility

-   $\mathbb{D}$ Let F be a field. The total strict order > on F is compatible iff $ \forall a,b,c \in F $,
    1.  $ a > b, c \Rightarrow a+c > b+c $
    2.  $ a > 0, b > 0 \Rightarrow ab > 0 $

-   Remarks
    1.  $ a > 0 \Rightarrow -a < 0 $  
        Proof:  
        $ a + (-a) > 0 + (-a) \Rightarrow 0 > -a \equiv -a < 0$
    2.  $ a \neq 0 \Rightarrow a^{2} > 0 $   
        Proof:  
        $ a \neq 0 \Rightarrow a > 0 \bigvee a < 0 $  
        -   case 1: $ a > 0 $. Replace b = a of the 2 in $\mathbb{D}$, i.e. $ a > 0, a >0 \Rightarrow aa > 0 \equiv a^{2} > 0 $
        -   case 2: $ a < 0 $. It implies that $ -a > 0 $. Again, by replacing $ b = -a $ of the 2 in $\mathbb{D}$, then 2 becomes $ -a > 0, -a >0 \Rightarrow (-a)(-a) >0 $.  
            But, $ (-a)(-a) = a\cdot a $  
            Proof this &ldquo;But&rdquo;:  
            -   Option 1:  
                First, $ a(-a) + (-a)(-a) = (a + (-a))(-a) = 0(-a) = 0 $. This implies that $ (-a)(-a) $ is the additive inverse of $ a(-a) $.  
                Second, $ a(-a) + aa = a(-a + a) = a\cdot 0 = 0 \Rightarrow a\cdot a$ is also the additive inverse of $ a(-a) $.  
                But the additive inverse is unique.  
                Thus, $ (-a)(-a) = a\cdot a = a^{2} $
            
            -   Option 2:  
                First, prove $ (-1)a = -a $.  
                
                -   $\mathbb{E}$ Prove the above statement.
                
                Then, $ (-a)(-a) = (-1)a(-1)a = a^{2} $.


<a id="orge8d3ca7"></a>

# Negative Elements

-   $\mathbb{D}$ $ P=\{x\in F | x>0\} $ the positive elements of F. Then, $ -P = \{-x | x \in P\} = \{x \in F | x < 0\} $.
-   Claim: $ F = P \cup \{0\} \cup -P $. In other words, F can be written as a disjoint union and P, the set of all positive elements of F, is closed under $ + $ and $ \cdot $.  
    Proof:
    1.  P is closed under addition, i.e. $ a >0, b>0 \Rightarrow a+b > 0 $  
        $ a > 0 \Rightarrow a+b > 0 + b $   
        and $ b > 0 \Rightarrow 0 + b > 0 + 0 $  
        $ \Rightarrow a+b > 0 $  
        Thus, P is closed under addition.
    2.  P is closed under multiplication. According to the second property of the $\mathbb{D}$ of compatibility, it is closed.
-   THM: (No Order) Let $ F = P \cup \{0\} \cup -P $ be a disjoint union in which P is closed under &ldquo;$ + $&rdquo; and &ldquo;$ \cdot $&rdquo;.   
    Then, the rule, $ a > b := a-b\in P $, defines a compatible total (strict) order on F.
    -   Proof: We must show > satisfies trichotomy, transitivity, and the compatibility. Note: trichotomy + transitivity $ \equiv $ totality!
        1.  Trichotomy:  
            let $ a, b \in F $, then $ a -b \in P \cup\{0\}\cup -P $  
            $ a-b\in P \Rightarrow a >b $  
            $ a-b \in \{0\} \Rightarrow a = b $  
            $ a- b \in -P \Rightarrow a < b $  
            Thus, trichotomy is satisfied.
        2.  Transitivity:  
            $ a > b, b > c \Rightarrow a-b, b-c \in P $  
            Then, the summation $ (a-b) + (b-c) = a-c \in P $ since $ P $ is closed under addition.
            Thus $ a-c\in P \Rightarrow a > c $, i.e. transitivity is satisfied.
        3.  Compatibility:  
            Coming next lecture!

