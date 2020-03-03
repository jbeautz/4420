<font color = "white">  

Jack Beautz  
jpb375  

#MATH 4420 Homework 4

##Exercise 1
Let $\{a_1,...,a_r\}$ be the set of points which cover $a$.  
Let $x\in \{a_1,...,a_r\}$ and $y\in [a,b]$.  
The interval of $L$ is atomic if $y$ can be written as the join of points in $[a,b]$.  

Consider $y_1$ which covers $a$. By semi modularity, we know $x\lor y_1$ covers $y_1$.  

Next consider $y_k$ which covers $y_{k-1}$. Since $x\lor y_{k-1}$ covers $y_{k-1}$, by semimodularity $x\lor y_k$ covers $y_k$.  

Continue inductively until you find that $y_k = y$. Thus $y$ is a join of points which cover $a$.  

Any $y\in [a,b]$ can be constructed in this way because of the semimodularity and lattice structure of the geometric lattic $L$.  


Consider $y_0\in [a,b]$ such that it cannot be constructed in this way. $y_0 > a$ and greater than each $a_i$. Let $z\in L$ be an element outside the interval such that $y_0\land z = a$. By definition, $z\not\in [a,b]$. Consider without loss of generality that $z<a$. Then, $z \land y_0 < a$. This is a contradiction to the assumption that $z\land y_0 = a$.  

Therefore, the interval of the lattice is atomic.  

##Exercise 2
Because $E$ is finite, $(E, F_E)$ is a combinatorical design if   
(i) $F_E$ is closed under intersection  
(ii) $\emptyset$,$E$ and singletons $\{x\}\in F_E$ are contained in $F_E$.  
(iii) $\forall x\in E-G$, $\exists ! H\in F$ such that $H$ covers $G$ and $x\in H$.  

First consider (i). Let $U$ and $W$ be subspaces of $V$. Let $G\in F_E$ and $H\in F_E$ such that they correspond with the intersection of $E$ and $W$ or $U$ respectively.  $H\cap G$ is defined as $\{E\cap U \cap W: U,W\subseteq V\}$. Note that $U\cap W\subseteq V$ because $U\subseteq V$ and $W\subseteq V$. Thus the intersection of flats $H$ and $G$ is a flat $F'$ such that $F'$ corresponds to the intersection of $E$ and $(U\cap W)$.  

Now consider (ii). $\emptyset\in F_E$ is defined as $\{E\cap U: U\subseteq V\}$ where $U\cap E = \emptyset$. $E\in F_E$ is defined as $\{E\cap E: E\subseteq V\}$. Every vector in $E$ is included in the intersection. Finally, define the set of subspaces $U_1,...,U_n$ such that $U_i = span(v_i)$, $\forall v_i\in E$. There exists a flat corresponding to each singleton $v_i$ defined as $\{E\cap U_i: U_i \subseteq V\}$.  

Finally consider (iii). Let $v_k\in E-G$ such that $H$ covers $G$ and $\{v_k\}$. If $H$ covers $G$ and $\{v_k\}$ then $H$ is defined as $\{E\cap ((E-G) \cap \{v_k\}):((E-G) \cap \{v_k\})\subseteq V\}$. Hence, $H$ exists. Suppose $H$ was not unique for each $v_k$. There must also exist $H'$ such that $H'$ covers $E-G$ and $v_k$. The only way to define this flat however is $\{E\cap ((E-G) \cap \{v_k\}):((E-G) \cap \{v_k\})\subseteq V\}$.  Hence, $H' = H$ and therefore the covers of $G$ partition $E-G$.  

Because these criteria are met $(E, F_E)$ is a combinatorical geometry.


##Exercise 3
First prove there exists $m$ and $E = \{v_1,...,v_n\}$ such that $(E,F_E)$ is isomorphic to $([n],F)$ if $|F|\geq n-1$.  
The flats of $([n],F)$ are the empty set, $[n]$, and each of the $n$ singletons. Hence, there are $n+2$ flats.  
Let $f$ be the bijective function which maps flats from $([n],F)\to (E,F_E)$.  
Define $f:\{i\}\to F_i$, $\forall i\in [n]$, where $F_i=\{E\cap span(v_i)\}$. Define $f:[n]\to F_V$ where $F_V=\{E\cap V\}$. And define $f:\emptyset\to F_\emptyset$ where $F_\emptyset = \{E\cap \emptyset\}$.  


Now prove if there exists $m$ and $E = \{v_1,...,v_n\}$ such that $(E,F_E)$ is isomorphic to $([n],F)$ then $|F|\geq n-1$.  
Consider the case where $|F|<n-1$. Then scalar multiplication to $v_i\in F^m$ could result in another vector $v_j\in F^m$ such that $v_j\in span(v_i)$. In this case the function $f$ as described is not a bijection and there is no isomorphism. For $|F|\geq n-1$ and a specific $m$, all vectors are linearly independent in $F^m$.  

Because the flats can be mapped bijectively between geometries, $(E,F_E)$ and $([n],F)$ are isomorphic if $|F|\geq n-1$.  


##Exercise 4
$(X, F-H)$ is a combinatorical geometry if it satisfies
(i) $F_E$ is closed under intersection  
(ii) $\emptyset$,$E$ and singletons $\{x\}\in F_E$ are contained in $F_E$.  
(iii) $\forall x\in E-G$, $\exists ! K\in F$ such that $K$ covers $G$ and $x\in K$.  

First, (i). $F-H$ is closed under intersection such that for $U,W\in F-H$, $U\cap W\in F-H$. We know that $F$ must be closed under intersection because $(X,F)$ is a combinatorical geometry.  
Suppose there exists $U,W\in F-H$ such that $U\cap W\in H$, then $F-H$ would not be closed under intersection.  
Then $U\cap W$ is one of the maximal elements of $F$ with regard to set inclusion. There exists no $Y\in X$ such that $U\cap W\subset Y$. But, by definition, $U\cap W\subset U$ so it is not a maximal element. Hence, $F-H$ is closed under intersection.  

Next, (ii). $(X,F)$ is a combinatorical geometry. $F-H$ does not contain the empty set, $X$ by definition. If $H$ contains all of the singletons, then the remaining combinatorical geometry is $(X,F_0)$ where $F_0$ contains two flats, the empty set and the maximal set. Therefore (ii) is satisfied.  

Finally, (iii). Suppose $(X,F-H)$ is a combinatorical geometry such that there is no independent set of $(X,F)$ with at least three elements.  
Then every flat with at least three elements has a dependency.
Consider the flat $F = \{X_1,X_2, X_3, ..., X_n\}$. Then without loss of generality there must be a dependency such that $X_1\subseteq X_2\cup X_3$. Because $(X,F-H)$ is a combinatorical geometry, $F_n = \{X_n\} = F - \{X_1,X_2, ..., X_{n-1}\}$ must be covered by the unique flats $F_n \cup \{X_1\}$ and $F_n\cup \{X_2\}$ and $F_n\cup \{X_3\}$. But there is a dependency between these "unique" flats such that $F_n\cup \{X_1\}\subseteq (F_n\cup\{X_2\})\cup (F_n\cup\{X_3\})$

THIS DOES NOT WORK YETT

Let three of the elements be $\{X_1,X_2,X_3\}$ such that $X_1\subset X_2\cup X_3$.  
Let $X_2$ be a maximal element such that $X_2\in H$.




***THE END***
