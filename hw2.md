<font color = white>  

Jack Beautz  
jpb375  

#MATH 4420 Homework 2  

###Exercise 1
Assume $v$ and $\lambda$ are odd.

Consider the $2$-set $T=\{a,b\}$ such that $T\subset B_1,...,B_\lambda$.  


Hence, any $2$-subset $T$ is contained in at most $\lambda=v-2$ blocks. Hence, $\lambda$ and $v$ can both be odd or even. The statement is false.


###Exercise 2
Prove there does not exist a 2 − (46, 10, 2) design with b = v.  

Theorem 19.1 from the text gives the expression for number of blocks in a design.

$$b = \lambda {{v\choose t}\over{k\choose t}}$$

Hence, the number of blocks in a $2 − (46, 10, 2)$ design is
$$b = 2 {{46\choose 2}\over{10\choose 2}}$$
$$b = 2{1035\over 45}$$
$$b = 46$$

Let $T=\{a,b\}$ such that $a,b\in P$.


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
Note that $b_1 = k$. Hence, every point is in exactly $b_1=k$ lines and every line has in exactly $b_1 = k$ lines. Thus, the definition of finite projective plane is satisfied.  

The definition requires there must exist four points such that no three share a line. Because the FPP of order $N=1$ has only $v=3$ points, there does not exist four points. Thus this is not an FPP. The smallest order FPP is the Fano Plane.



***THE END***
