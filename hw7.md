<font color = white>  

Jack Beautz  
jpb375  

#MATH 4420 Homework 7

##Exercise 1
(a)  
$$\zeta\cdot\mu = I$$
The identity matrix has 1 only on the diagonal where row index $z$ equals column index $y$.  So,
$$\zeta(z,y)\mu(z,y) = 1$$
if $z=y$ and
$$\zeta(z,y)\mu(z,y) = 0$$
if $z<y$.  

Consider the case where $z=y$, then the summation occurs over one iteration, $\mu(y=y)=1$ which must be true by the definition of the mobius function on a poset. If $\mu(y,y)=0$, then there would be a zero at this spot on the diagonal because $z\leq y$ and therefore $\zeta(z,y)=1$.  

Now consider the summation which occurs when $x<y$
$$\sum_{z\leq x\leq y} \mu(z,y)=0$$
In the case where $z\neq y$ we know $z< y$ and thus, the coefficient at the $z$ row and $y$ column is $0$. We know $\zeta(z,y)=1$ at this spot because $z\neq y$. Thus, $\mu(z,y)=0$ so that $\zeta(z,y)\mu(z,y)=0$. $z<y$ for all parts of the sum so $\zeta(z,y)=1$, but we know the summed coefficients in the matrix never crossed the matrix diagonal, thus every coefficient is 0. Hence, the mobius function must be 0 so that $\mu(z,y)\zeta(z,y)=0\times 1 = 0$.  

(b)  
Denote $\zeta(x,y)$ over the poset as the matrix of all outputs for row $x$ and column $y$. Let this be $Z_p$. Denote the mobius function over the poset similarly. Let this matrix of possible outputs be $M_p$. Note, both matrices are of full rank because for both $M_P$ and $Z_P$, the diagonal entries at least are nonzero.
Using this notation we rewrite
$g(x)=\sum_{y\leq x}f(y)$ as
$$g = Z_P f$$
And $f(y)=\sum_{x\leq y}g(x)\mu(x,y)$ as
$$f = M_P g$$
where the rows of $f$ and $g$ index all elements of the poset.  
Note, $M_P$ and $Z_P$ are invertible so it suffices so show $M_P^{-1}=Z_P$. By defintion of the mobius function this is true, thus the statement is true.
$$M_pg = f$$
$$g=M_p^{-1}f$$
$$g=Z_p f$$  

##Exercise 2
$$\chi_M(\lambda)=\prod_{i=1}^{n-1} (\lambda-i)$$



complete graph has chromatic polynomial $(x)_ k$.
The partition matrix has 








##Exercise 3
Assume $\mu(x,y)=(-1)^{r_P(y)-r_P(x)}$ for all $x\leq y$. Consider the case where $x=y$, then $\mu(x,x)=1=(-1)^0$. If $x<y$, then $\sum_{x\leq z\leq y}\mu(z,y)=0$. Suppose without loss of generality that in the interval $[x,y]$ there are more even rank elements than odd rank elements. Because the lattice is graded, the length of the maximal path between $x$ and $y$ is $l = r_P(y)-r_P(x)$. There are more even rank elements than odd rank elements in the interval so the summation over the whole interval will be not equal to 0. Consider that $\sum_{x\leq x\leq y}\mu(x,y)=0$ implies that the summation elements will negate each other. Hence, there must be an equal number of odd and even rank elements in the interval.

Assume there is an equal number of even rank subsets and odd rank subsets in any interval $[x,y]$ of the poset $P$. We know $\sum_{x\leq x\leq y}\mu(x,y)=0$. Use induction on $z\in [x_1,x_k]$ where $x_k=y$. Base case has $z=x_1$ which leads $\mu(x_1,z)=1$. The defintion of the mobius function requires $\sum_{x\leq x\leq y}\mu(x,y)=0$ so $\mu(x_1,x_1)+\mu(x_1,x_2)=0$. This requires that $\mu(x_1,x_2)=-1$. Now in general consider the summation over the interval $[x_i,x_{i+1}]$. This must also be 0. Thus, at each interval in the value of the summation on the mobius function must be 0 and the individual mobius function outputs must be either 1 or -1 for each step. Now, consider the generic case where we sum over $[x_1,x_k]$. There is an equal number of odd and even rank elements in the interval so the positive and negative ones will cancel each other out along the way. Thus, $\mu(x,y)=(-1)^{r_p(x_k)-r_p(x_1)}$.















***THE END***
