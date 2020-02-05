<font color = "black">

Jack Beautz  
jpb375  

#Math 4420 Homework 1

##Exercise 1
Take the edges of K 7 as points of an incidence structure.
The blocks are to be all sets of five edges of these three types: (a)
‘claws’ with five edges incident with a common vertex, (b) edge sets
of pentagon subgraphs, and $(c)$ five edges that form a triangle and
two disjoint edges. Show that this is an $S_3(3, 5, 21)$ design.

$K_7$ has ${7(7-1)\over 2} = 21$ edges. Hence, there are $v = 21$ points in $P$ to consider.  
Each block has 5 edges so the cardinality of each block is $k=5$.  
There are 3 types of 5-edge blocks. Hence, any 3-subset is contained in exactly $\lambda = 3$ possible 5-subsets.    


##Exercise 2
Non Trivial Combinatorical designs have both a divisibility restriction and an inequality restriction.  Adding a point $x$ to both the set $P$ and each block in $\beta$ will only form a combinatorical design if these constraints are satisfied.

Adding $x$ to the design changes the $t-(v,k,\lambda)$ design to $t+1-(v+1, k+1, \lambda)$ constraint.  

The first constraint states the number of blocks $b_i$ for a given $t$ must be an integer value. As shown in lecture for all $i\in \mathbb{Z}$ such that $0\leq i\leq t$,
$$b_i = {{v-i\choose t-i}\over {k-i\choose t-i}}$$

Adding the point $x$ changes the expression to be
$$b_i = {{v-i + 1\choose t-i+1}\over {k-i+1\choose t-i+1}}$$
$$b_i = {(v-i+1)!(k-t)!\over (k-i+1)!(v-t)!}$$
Hence, the following quotient of falling factorials must be an integer value for the new design to exist.
$$b_i = {(v-i+1)_ t \over (k-i+1)_ t}$$

Next, consider the inequality constraint on non-trivial designs.
$$v\geq (t+1)(k-t+1)$$
Adding the point $x$ changes the expression to be
$$v+1\geq (t+2)(k-t+1)$$
$$v\geq -t^2 + tk - t + 2k + 1$$

If a design satisfies the quotient and inequality constraint after the described addition of $\{x\}$, it is a valid combinatorical design.

##Exercise 3
Theorem 19.3 of the text states Given $i\in [0,t]$, the number of blocks incident with all the points of an $i$-subset $I$ of $P$ is
$$b_i = \lambda{{v-i\choose t-i}\over {k-i\choose t-i}}$$

$b_i$ must be an integer value so there is a division constraint on the design.

For $S(3,6,v)$, the expression becomes
$$b_i = {{v-i\choose 3-i}\over {6-i\choose 3-i}}$$
For $i\in [0,3]$.  
Setting $i = 1$ we find the following expression must be restricted to take on an integer value.
$$b_1 = {{v-1\choose 2}\over {5\choose 2}}$$
Simplifying we find
$$b_1 = {(v-1)(v-2)\over 20}$$

20 has a prime factorization of $20 = 2^2\cdot 5$.

Let $V = (v-1)(v-2)$ such that the design exists.
$V$ must have a prime factorization which includes $2^2\cdot 5$ because 20 divides V.

The value of $v$ in general will not produce a $V$ which 20 divides. In order to produce a $V$ with factors $2^2$  and $3$, $v = 20x + 6$ or $v = 20x + 2$. In this way only 20 is guaranteed to divide $V$.

##Exercise 4
(i)
A trivial design is a design with one block that contains all the points or a design that has all the k-subsets of the point set as blocks is of course a t-design for t ≤ k

If $v = k$, then there can only be one block in the design, so it is trivial.  

The number of blocks of an $S_λ (t, k, v)$ that are incident with none of the points of a $j$-subset $J$
of $P$ is
$$b^j = {{v-j\choose k} \over {v-t\choose k-t}}$$
To check trivial designs set $j=t$ and $t+k\geq v$ such that
$$b^t \geq {{k\choose k} \over {k\choose k-t}}$$
$$b^t \geq t!$$

Hence, every $k$-subset of $P$ must exist in $\beta$. The design is trivial.  

(ii)  The compliment of a $t$-design is a design such that each block is composed of the points not in the original block.  

Let $t'-(v',k',\lambda')$ denote the compliment of $t-(v,k,\lambda)$. Let $b = |\beta|$.  

Hence, $v$ remains the same in the compliment because the set $P$ has the same number of points.  

$k' = v - k$ because each block will now include the set of points which were not in the block. The compliment of each block in $\beta$ are the blocks of $\beta'$.

$t' = t$ because $t$-subsets were contained in $\lambda$ blocks. Hence, there are $b - \lambda$ $v-k$-subsets which contain $t$. If the set $\{B_1,...,B_\lambda\}$ contained a specific $t$-subset in the original design, then the set $\{B_{\lambda+1}', ..., B_b'\}$ will contain the same $t$-subset in the compliment.  

$\lambda' = b - \lambda$ because there will $\lambda$ compliment blocks which do not contain a specific $t$-subset because they were the $\lambda$ blocks which contained the $t$-subset in the original design.  

Hence, the compliment of a $t-(v,k,\lambda)$ design with $b = |\beta|$ is a $t-(v, v-k, b-\lambda)$ design.


##Exercise 5

Let $(P_0, \beta_0)$ and $(P_1, \beta_1)$ correspond to different combinatorial designs.  
As shown in discussion, combinatorial designs are isomorphic if and only if there exist bijective maps $f,g$ such that $f: P_0\to P_1$ and $g: \beta_0\to \beta_1$ such that the incidence relation is implied.  

Let the points on the fanoplane compose the set $P_0$. Let $\beta_0$ be a set of $3$-subsets of $P_0$ such that for each line in the fanoplane there exists $B_i\in \beta_0$ where $B$ is composed of the points on the line.  

Let $(P_1, \beta_1)$ be the incidence structure corresponding to a $2-(3,7,1)$ design.  

Let $f:P_0\to P_1$ be a mapping from the 7 points on the plane to $[7]$.  
Let $g:\beta_0\to\beta_1$ be a mapping from the subsets of points on each line to $3$-subsets of $[7]$ in the blocks of $\beta_1$.

Hence, there exists the necessary bijections for there to be an isomorphism between the fanoplane and a $2-(3,7,1)$ design.  

The incidence relation such that any $2$-subset of $P_0$ or $P_1$ is contained in exactly $1$ block of $beta_0$ or $\beta_1$ is implied by the isomorphism.





***THE END***
