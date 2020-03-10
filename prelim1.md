<font color = white>  

Jack Beautz  
jpb375  

#MATH 4420 Prelim 1
##Question 1
Proof by Induction:  
Base Case: $t=2$  

Claim: If every two subset is in a unique block of $P$, then $b_{t,v} = v$. For $x\in P$, denote by $r_x$ the number of blocks containing $x$, and similarly for $B\in\mathcal B$, let $k_B=|B|$. This is not the trivial case so there is more than one block. If $x\not\in B$ then $r_x\geq k_L$ because there are $k_B$ other blocks containing $x$. Suppose $b\leq v$. Then $b(v-k_B)\geq v(b-r_x)$. Now counting this two ways we find
$$1= \sum_{x\in P}\sum_{B\ni x} {1\over v(b-r_x)}\geq \sum_{B\in\mathcal B}\sum_{x\not\in B} {1\over b(v-k_L)} = 1$$
This implies that in all inequalities, equalities must hold. Hence, $b= v$.  

Plugging in $b_{t,v}=v$ in the expression leads to
$$b_{t,v}(b_{t,v}-1) \geq t{v\choose t}$$
$$v(v-1)\geq {2v!\over 2!(v-2)!}$$
$$v(v-1)\geq v(v-1)$$

Hence, equality holds at the base case.  

Step Case:
Count the number of ordered triples $(x,A,B)$ such that $x\in A,B$ and $A,B\in \mathcal B$ and $A\neq B$. Note that this is an upper bound on the number of elements in any $T$-subset because it represents the case where each subset is contained in one unique block which contains nothing else.

$$\sum_{B\in \mathcal B}\sum_{A\neq B} 1 \geq \sum_{T\in \mathcal  T}\sum_{x\in T} 1$$

By the LHS of the inequality,
$$N=\sum_{B\in \mathcal B}\sum_{A\neq B} 1 $$
There are $v\choose t$ unique $t$-subsets to be concerned about.
$$N= b_{t,v}\sum_{A\neq B} 1$$
Now we count all blocks execpt for the one block already counted.  
$$N= b_{t,v}(b_{t,v}-1)$$

By the RHS of the inequality,
$$M= \sum_{T\in \mathcal  T}\sum_{x\in T} 1$$
There are $v\choose t$ possible $t$-subsets to count through
$$M = {v\choose t}\sum_{x\in T} 1$$
And there are $t$ elements in each $t$-subset.
$$M = {v\choose t}t$$

Therefor we arrive at the desired result
$$b_{t,v}(b_{t,v}-1)\geq t{v\choose t}$$
Because the upper bound on ways to count elements in each $t$-set is all possible combinations of 2 different blocks.


##Question 2
(a) Suppose there exists $x\not\in L_1$ such that there is no line containing $x$ in the space $A_L$. $A_L$ is a linear space so every pair of points is in exactly one line. Consider the pair $(x, y)$ which must be in one line. But $x$ is not in any lines. Thus there is a contradiction. There must exist a line $L_2$ such that $x\in L_2$.

Because $A_L$ is a linear space, there must exist a line $L_2$ between points $(x,y)$. Let $z$ be another point such that there exists another line $L_z$ defined by the pair $(y,z)$.  The smallest projective plane conatains $7$ points and results in $A_L$ containing 4 points as stated in the problem description. Thus, there is at least one other point $a$, in all cases, such that $(a,z)$ is contained in a line. Call this line $L_1$ and let it contain no other elements such that $L_1\cap L_2 = \emptyset$.  

Fix $L_1$. $L_2$ must be unique. Suppose there is another line $L_2'$ such that $x\in L_2'$ and $L_1\cap L_2' = \emptyset$. Chapter 23 of the text states on page 322 that every line in a projective geometry of order $n$ have lines of size $n+1$. There are no sets of more than two parallel lines $A_L$ derived from the fano plane. Thus, every parallel line defined by a point not in a line is unique. Removing a line from a projective plane with order $n\geq 3$ will result in all lines having size $n$.  

Consider $L_0\in \mathcal{L}-L$ and $x\not\in L_0$ . There are $n^2-1$ points in $P-L- \{x\}$ and $n-1$ points in each line, not including $x$.  Hence, there must be ${n^2-1\over n-1} = n+1$ lines going through $x$. We established earlier the line $L_0$ has $n$ points. And therefore there exist $n$ unique lines passing through $x$ which contain points on $L_0$. Hence, there is only one line remaining such that $x\not\in L_1$ and $L_1\cap L_0 = \emptyset$. Therefore for each line $L_0$ and point $x\not\in L_0$, there exists one distinct line $L_1$ such that $L_1\cap L_0 = \emptyset$ and $x\in L_0$.  


(b) For each line in $\mathcal{L}-L$, there exists a unique point not in the line which is in the parallel line. We can build any three lines using part (a).  
Let $L_1,L_2,L_3\in \mathcal{L}-L$ be distinct lines. By part (a) of this question we know that for $L_1$ and a point $x\not\in L_1$, there must exist a unique line $L_2$ such that $x\in L_2$ and $L_2\cap L_1 = \emptyset$. For $L_2$ and some point $y\not\in L_2$ there exists a line $L_3$ such that $L_3\cap L_2 = \emptyset$.
There is unique line corresponding to $L_1$ and the point $y\not\in L_1$. This line is $L_3'$ and $L_3'\cap L_1 = \emptyset$. Assume this line $L_3'$ was not the same as  $L_3$.   
As shown in part (a) there are $n+1$ lines which include $y$ in $\mathcal{L}-L$. By assumption we know $L_3'$ cannot be $L_3$, the line parallel to $L_2$. So, $L_3'$ must be one of the $n$ remaining lines which pass through $y$. But there must also be a line containing $y$ and each point in $L_1$.  There are $n$ points in $L_1$. Thus, there are no possible lines left to be $L_3'$. It cannot exist.  

Hence, if $L_1\cap L_2 = \emptyset$ and $L_2\cap L_3 = \emptyset$, then $L_1\cap L_3 = \emptyset$.  


***THIS NEEDS TO BE GENERALIZED FOR N>2***
###Question 3
Let $L^ {* }$ be the poset dual of $L$, a geometric lattice.  

Let $A^{* }$ denote the set of atoms of $L^ {* }$. Let $z\in L^ {* }$. Because $z\in L^ {* }$, it must also have been in the geometric lattice $L$. Let $A\subset L$ be the set of atoms of $L$. These atoms in $L$ are the elements covered by the maximal element in $L^{* }$. Because of semimodularity, if there exists $x,y\in L$ which cover $z$, there must also be $a\in L$ which covers $x$ and $y$.  
In the geometric lattice, there may be other elements which cover $x$ or $y$. Move up the lattice iteratively using semimodularity. Let $A'$ be the set of all elements in $A^{* }$ such that the meets of these elements is $x$. This set must exist due to the semimodularity of $L$ and it is equivalent to the atoms which join together to form $z$ in $L^{* }$. Thus, for any element $z$ in a lattice, the set of atoms which join together to make up $z$ can be constructed using the semimodularity and meets of elements in the geometric poset dual $L^ {* }$.


###Question 4
(a) A lattice is a poset $L$ such that $\forall x,y\in L$, $x\land y$ and $x\lor y$ exist.  

Let $A,B\in X$. Define $A\lor B$ as the smallest set $Z$ such that $A\cup B \subseteq Z$.  But $A\cup B\subseteq X$ so $Z$ exists.  
Define $A\land B$ as the maximal set $W$ such that $W\subseteq A\cap B$. Because $A, B\subseteq X$, $W$ exists.  

(b) $c$ is a closure operator if for all $A,B\subseteq X$,  
(i) $A\subseteq c(A)$  
(ii) If $A\subseteq B$, then $c(A)\subseteq c(B)$  
(iii) $c(c(A)) = c(A)$  
$$c(A) = \{y\in J: y\leq\bigvee A\}$$

First, suppose there exists $A\subseteq L$ such that $A\not\subseteq c(A)$ such that $(i)$ is not true.
We know for every element $x\in c(A)$, $x\in J$. We also know $A\subseteq c(A)$, which means for $\bigvee A\leq \bigvee c(A)$ so if $x\leq \bigvee A$, $x\leq \bigvee c(A)$. Hence, $\forall x\in c(A)$, $x\in J$ and $x\leq \bigvee c(A)$. Thus, if $x\in A$, $x\in c(A)$.  $A\subseteq c(A)$. So $(i)$ holds.  

Next, suppose there exists $A,B\subseteq L$ such that $A\subseteq B$ and $c(A)\not\subseteq c(B)$. There must be an element $x\in c(A)$ such that $x\not\in c(B)$. $x\in c(A)$ so $x\in J$ and $x\leq \bigvee A$. Hence, if $x\not\in c(B)$, then $x> \bigvee B$. But $A\subseteq B$ so $\bigvee A \leq \bigvee B$. Thus, $x\leq \bigvee A \leq \bigvee B$ and $x\in c(B)$. So, (ii) holds.  

Finally, (iii) is proven by showing $c(A)\subseteq c(c(A))$ and $c(c(A))\subseteq c(A)$. First, $c(A)\subseteq c(c(A))$. This was proved in (ii) so it must be true.  Next, $c(c(A))\subseteq c(A)$. Suppose there exists $x\in c(c(A))$ such that $x\not\in c(A)$. $x\in c(c(A))$ so it must also be true that $x\in J$.  Both $\bigvee c(A)$ and $\bigvee c(c(A))$ are the join of $x\leq \bigvee A$. Thus, $\bigvee c(A)= \bigvee c(c(A))$. Hence, $x > \bigvee c(A)$ and $x \leq \bigvee A$. This is a contradiction. Therefore $c(A)=c(c(A))$. So, (iii) holds.  

Because all three properties of the defintion of a closure operator hold for $c(A)$, $c$ must be a closure operator.  

$(c)$ Let $A$ be a closed set of $L$ such that $A$ is not defined by $D(x) = \{y\in J: y\leq x\}$ for some $x\in L$. $c(A)$ is a closure operator by part (b). This means $A=c(A)=\{y\in J: y\leq \bigvee A\}$. $A$ is a subset of lattice elements so by definition $\bigvee A\in L$ must exist. Let $x_0 = \bigvee A$. Then, $A = D(x_0)$. Thus all closed sets of $L$ are of the form $D(x)$ for some $x$.  

(d) For each $x\in L$, there is a unique result of the function $D(x) = \{y\in J: y\leq x\}$. $D(x_0)$ and $D(x_1)$ where $x_0\neq x_1$ and without loss of generality, $x_0<x_1$. Suppose $D(x_0)=D(x_1)$, then $\{y\in J:y\leq x\}=\{y\in J:y\leq x_1\}$. But $x_0<x_1$ so there exists some $y\in J$ such that $x_0<y\leq x_1$. So $y\in D(x_1)$ but $y\not\in D(x_0)$. Thus the sets are not equal. Hence, $D$ is injective.  

Suppose there exists $D(x_0)\in c$ such that $x_0\not\in L$.  Then $D(x_0)$ is a closed set not of the form $D(x)$ for some $x\in L$. In part $(c)$ this was shown to be impossible. Thus, the function $D$ is sujective.  

Suppose the relation of the posets $c$ and $L$ was not maintained under the function $D$. Then for $a,b\in L$ where $a\leq b$ we have $D(a)> D(b)$. This relation is equivalent to $\subset$ and it must exist because this is a lattice as shown in part (a). Hence, $D(b)=\{y\in J: y\leq b\}\subset \{y\in J: y\leq a\}=D(a)$. Then there exists $y\in D(a)$ such that $y\not\in D(b)$. This means $y\leq a$ and $y>b$ for some $y\leq a \leq b$. This is a contradiction. Thus the poset relations are maintained.  

Because $D$ is both injective and surjective and the relation is maintained it is a poset isomorphism.


##Question 5
The set of edges $E$ of spanning tree $T$ is a basis for $L(G)$ if it is an independent set of edges and it contains every element in $V(G)$.  

Assume $E$ is not independent. Then there exists an edge $e$ such that $e$ connects two vertices $(x,y)$ which are already connected in the tree. There must exist a cycle which contains $(x,y)$ because these vertices are now connected to the rest of the tree in two different ways. But the tree is supposed to be the maximal edge set such that no cycles are formed. Thus, the edge set is independent.  

$E$ must contain every element in $L(G)$. The elements of $L(G)$ are to be all those partitions $\mathcal A$ of $V(G)$ such that the subgraph of $G$ induced by each block of $\mathcal A$ is connected. Thus the spanning tree corresponds to the partition of $E = \{\{v_1,...,v_n\}\}$ where every element is in one block and every element is connected. Note in the lattice $L(G)$ for any element $X\in L(G)$, $X\leq E$.  

Thus, every spanning tree is a basis.  

Suppose there is a basis $B$ of $L(G)$ which is not a spanning tree. Then $B$ contains every point in the graph and $B$ is independent.  

Construct $B$ such that we continuously add independent edges until every vertex is included in the basis. This will form a tree because independent edges will never form a cycle. It will span the graph because we continue iteratively until every vertex is included. Therefore $B$ is a spanning tree.  

Hence, every basis of $L(G)$ is a spanning tree.  

The set of bases of $L(G)$ must be exactly the set of spanning trees of $G$.  



**THE END**
