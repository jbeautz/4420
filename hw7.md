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

##Exercise 2
