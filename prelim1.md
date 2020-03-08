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

***NEEDS WORK***


##Question 2
(a) Suppose there exists $x\not\in L_1$ such that there is no line containing $x$ in the space $A_L$. $A_L$ is a linear space so every pair of points is in exactly one line. Consider the pair $(x, y)$ which must be in one line. But $x$ is not in any lines. Thus there is a contradiction. There must exist a line $L_2$ such that $x\in L_2$.

Because $A_L$ is a linear space, there must exist a line $L_2$ between points $(x,y)$. Let $z$ be another point such that there exists another line $L_z$ defined by the pair $(y,z)$.  The smallest projective plane conatains $7$ points and results in $A_L$ containing 4 points as stated in the problem description. Thus, there is at least one other point $a$ such that $(a,z)$ is contained in a line. Call this line $L_1$ and let it contain no other elements such that $L_1\cap L_2 = \emptyset$.  

Fix $L_1$. $L_2$ must be unique. Suppose there is another line $L_2'$ such that $x\in L_2'$ and $L_1\cap L_2' = \emptyset$. Let $(a,z)\subseteq L_1$ and $(x,y')\subseteq L_2'$ and $(x,y)\subseteq L_2$, $y'\neq y$. Then,  
***UNIQUENESS NEEDED***

(b) For each line parallel to a line in $\mathcal{L}-L$, there exists a unique point not in the line which is in the parallel line. Hence, we can build any three lines using part (a).  
Let $L_1,L_2,L_3\in \mathcal{L}-L$ be distinct lines. By part (a) of this question we know that for $L_1$ and a point $x\not\in L_1$, there must exist a unique line $L_2$ such that $x\in L_2$ and $L_2\cap L_1 = \emptyset$. For $L_2$ and some point $y\not\in L_2$ there exists a line $L_3$ such that $L_3\cap L_2 = \emptyset$.
There is unique line corresponding to $L_1$ and the point $y\not\in L_1$. This line is $L_3$ and $L_3\cap L_1 = \emptyset$. Suppose this line was not $L_3$. Then, there is another line $L_4$ parallel to $L_1$ which contains $y$. But then $L_4$ is also parallel to $L_1, L_2$. So there must be a unique $z\not\in L_1$ such that $z\in L_4$ and $L_4\cap L_1 = \emptyset$.  
Hence, if $L_1\cap L_2 = \emptyset$ and $L_2\cap L_3 = \emptyset$, then $L_1\cap L_3 = \emptyset$.

###Question 3
Let $L^ {* }$ be the poset dual of $L$, a geometric lattice.  

Let $A^{* }$ denote the set of atoms of $L^ {* }$. Let $z\in L^ {* }$. Because $z\in L^ {* }$, it must also have been in the geometric lattice $L$. Let $A\subset L$ be the set of atoms of $L$. These atoms in $L$ are the elements covered by the maximal element in $L^{* }$. Because of semimodularity, if there exists $x,y\in L$ which cover $z$, there must also be $a\in L$ which covers $x$ and $y$.  
In the geometric lattice, there may be other elements which cover $x$ or $y$. Move up the lattice iteratively using semimodularity. Let $A'$ be the set of all elements in $A^{* }$ such that the meet of these elements is $x$. This set must exist due to the semimodularity of $L$ and it is equivalent to the atoms which join together to form $z$ in $L^{* }$. Thus, for any element $z$ in a lattice, the set of atoms which join together to make up $z$ can be constructed using the semimodularity and meets of the geometric poset dual $L^ {* }$.










**THE END**
