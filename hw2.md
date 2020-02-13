<font color = white>  

Jack Beautz  
jpb375  

#MATH 4420 Homework 2  

###Exercise 1
Assume $v$ and $\lambda$ are odd.

Consider the $2$-set $T=\{a,b\}$ such that $T\subset B_1,...,B_\lambda$.  


Hence, any $2$-subset $T$ is contained in at most $\lambda=v-2$ blocks. If $\lambda$ is odd, it is possible that $v$ is too.  Hence, $\lambda$ and $v$ can both be odd or even. The statement is false.


###Exercise 2
Prove there does not exist a 2 − (46, 10, 2) design with b = v.  

Theorem 19.1 from the text gives the expression for number of blocks in a design.

$$b = \lambda {{v\choose t}\over{k\choose t}}$$

Hence, the number of blocks in a $2 − (46, 10, 2)$ design is
$$b = 2 {{46\choose 2}\over{10\choose 2}}$$
$$b = 2{1035\over 45}$$
$$b = 46$$

Let $T=\{a,b\}$ such that $a,b\in P$. By definition, $T\subset B_0$ and $T\subset B_1$ where $B_0,B_1$ are the only two blocks containing $T$. The other 44 blocks must not contain both $a$ and $b$. Of the blocks that contain $a$ or $b$ but not both we have a $2-(44, 9, 2)$ design on $P'=P-(\{a\}\cup\{b\})$ and $\mathcal B' = \{B-(\{a\}\cup\{b\}): B\in \mathcal B\}$.  
We can continue selecting 2-subsets such that each time we create a new deign $(P',\mathcal B')$ such that those 2 points are not both contained in the remaining blocks.  

Consider the design $2-(28,2,2)$. Here each 2-subset is contained in two different blocks, but the blocks have cardinality 2. Hence, each two subset can only be contained in at most one unique block.  This design does not exist. But it is derived from $2-(46,10,2)$. Hence, there does not exist a $2-(46,10,2)$ design.


##Exercise 3  
The finite projective plane is a $2-(v,k,\lambda)$ design such that there exists 4 points such that no 3 of the points are in the same line.  

From discussion question 2 we know every line contains the same number of points, k. Every pair of points is in one line so $\lambda = 1$. Suppose $v=n^2 + n + 1$ for some $n\in \mathbb{Z}$.

Hence, the FPP is a $2-(n^2+n+1, k, 1)$ design.
The number of blocks incident with any given point is given by formula 19.2
$$b_1 = \lambda {{v-1\choose t-1}\over {k-1\choose t-1}}$$
$$b_1 = {{n^2 + n\choose 1}\over {k-1\choose 1}}$$
$$b_1 = {n^2 + n \over k-1}$$

Now, suppose every $k=n+1$.
$$b_1 = {n^2 + n\over n}$$
$$b_1 = n + 1$$
Note that $b_1 = k$. Hence, every point is in exactly $b_1=k$ lines and every line has in exactly $b_1 = k$ lines. Thus, there exists 3 points such that they are no on the same line and the definition of finite projective plane is satisfied.  

The definition requires there must exist four points such that no three share a line. Because the FPP of order $N=1$ has only $v=3$ points, there does not exist four points. Thus this is not an FPP. The smallest order FPP is the Fano Plane.

##Exercise 4  
a) If no two columns are multiples of each other, then each basis $B_{i,j}$ has two elements.  

Suppose two bases intersect at more than one column. Then both bases contain the same set of vectors $v_i$ and $v_j$ such that $span\{v_i, v_j\} = span\{v_i\}$. Hence, $v_i$ is a scalar multiple of $v_j$. This contradicts the initial statement. Thus, two blocks intersect at exactly 1 or no column vectors.  

Suppose a set of two column vectors $\{v_i, v_j\}$ were contained in two different bases $B_a, B_b$. Let $B_a = \{i, j\}$ and $B_b = \{i, k\}$. Then, either $v_i$ or $v_j$ must be a scalar multiple of $j$. This contradicts the initial statement. Thus, every two points are contained in exactly one line.

By definition, this design is a linear space.  

b) $\mathcal{L_A}$ is defined by the linear dependence relation in the column vectors of $A$. Doing elementary row operations applies linear operations to the rows. Thus, $row(A) = row(B)$ and as a result $col(A) = col(B)$. Using the indices in the blocks of $\mathcal L_A$ and $\mathcal L_B$ to take subsets of $col(A)$ and $col(B)$ will result in equivalent subsets because the linear dependence relations are maintained through elementary row operations.

c) $\mathcal{L_A}$ is defined by the linear dependence relations between column vectors. Multiplying a single vector by a non zero scalar will not change the span of that vector. The incidence relation of bases is derived only from the span of each column vector which is unchanged by scalar multiplication.


##Exercise 5
The fano plane is of order 2 so if there exists a matrix corresponding to the linear space it will be $3\times 7$. As shown in part a of the last exercise if a matrix corresponds to a linear space no two column vectors can be scalar multiples of each other. $B$ is a $3\times 7$ matrix such that this condition is met. Thus there is a corresponding linear space of with 7 points, just like the fano plane.

a)
- $a=d$: If $a\neq d$, then then the column vector would become linearly independent on two other vectors. This would violate the 2-design. Hence, $a = d = 1$.  
- $e=b$: $e=1$. Otherwise the fourth column could be a scalar multiple of the sixth.
- $e=cd$: Otherwise the fourth and fifth column vectors could be scalar multiples of each other.  
- $e=ca$: Otherwise the third and fourth column vectors could be scalar multiples of each other.  

b) Assume $2ca \neq 0$. Suppose the fourth or fifth column vectors are multiplied by $2c$ or $2a$ respectively. Then, the vectors would have a nonzero value in each row.  These values will not be equivalent so the vector is a linear combination of the first three column vectors. But the laws of linear spaces require each column to be a linear combination of exactly two other vectors. This is not possible if $2ca \neq 0$.  

c) $c,a$ are defined to be nonzero scalars hence, $2ca \neq 0$. Therefore there is no such matrix $A$ which corresponds to the fanon plane.  




***THE END***
