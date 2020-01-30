<font color = "white">

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








***THE END***
