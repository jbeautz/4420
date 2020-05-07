<font color = white>  

Jack Beautz  
jpb375  

#MATH 4420 Homework 8

##Exercise 1
Proof by Induction  

Base case: $rank(A)=rank(X)=1$ for any $A\subset X$.  
Then,
$$\mu(\emptyset, X) = \sum_{\bar A = X} (-1)^{|A|}$$
$$\mu(\emptyset, X) = \sum_{\bar A=X} (-1)^1$$
But there is only one subset $A$ of $X$, and it is $X$.
$$\mu(\emptyset, X) = -1$$
Thus, $\mu(\emptyset, \emptyset) + \mu(\emptyset, X) = 1 + (-1) = 0$.  
The hypothesis holds for the base case.  

Step Case: $rank(X)=n$.  
Then for $\bar A = X$, $rank(A)=n$.  
Consider mobius function based formula for the characteristic polynomial of a matroid.  
$$\chi_M(\lambda) = \sum_{F\in\mathcal F}\mu(\emptyset, F)\lambda^{r(X)-r(F)}$$
Now consider the other formula for characteristic polynomial.  
$$\chi_M(\lambda) = \sum_{A\subseteq X}(-1)^{|A|}\lambda^{|X|-|A|}$$
Lets color the same matroid $(X,I)$ with both formulas.  
$$\sum_{F\in\mathcal F}\mu(\emptyset, F)\lambda^{r(X)-r(F)} = \sum_{A\subseteq X}(-1)^{|A|}\lambda^{|X|-|A|}$$
Let the subsets $A$ of $X$ form a combinatorical geometry with rank associated with their cardinality.  
$$\sum_{F\in\mathcal F}\mu(\emptyset, F)\lambda^{r(X)-r(F)} = \sum_{F\in\mathcal F}(-1)^{r(F)}\lambda^{r(X)-r(F)}$$
Thus,
$$\sum_{F\in\mathcal F}\mu(\emptyset, F) = \sum_{F\in\mathcal F}(-1)^{r(F)}$$
$$\mu(\emptyset, F) = (-1)^{r(F)}$$
By definition of the mobius function
$$\sum_{F\in F}\mu(\emptyset, F)  = 0$$
$$\sum_{F\in F}(-1)^{r(F)}  = 0$$
Since, ${n\choose k}= {n\choose n-k}$, the lattice structure of the combinatorical geometry is symmetric and the above statement holds for $r(F)=|F|$.  
Thus the induction hypothesis holds true at the $n$th step.  

##Exercise 2
The lattice of flats $\mathcal F$ is equivalent to the set of all subsets $A\subseteq X$ in this case. Let $r(F)$ be defined as $|A|$ the corresponding subset. By the results in exercise 1 we know $\mu(\emptyset, F) = (-1)^{r(F)}$. Thus,
$$\chi_M(\lambda)=\sum_{F\in\mathcal F}\mu(\emptyset, F)\lambda^{r(X)-r(F)} = \sum_{A\subseteq X}(-1)^{|A|}\lambda^{|X|-|A|}$$

##Exercise 3
By defintion:
$$\sum_{x\leq z\leq y} \mu(z,y)= 0$$
Let $a$ be any atom. Let $b$ be any rank 2 element. The matroid is rank 3 and simple so there are $3$ atoms.   
$$0 = \mu(\emptyset, \emptyset) + 3\mu(\emptyset,a) + r\mu(\emptyset,b) + \mu(\emptyset,X)$$
$$0 = 1 +3\mu(\emptyset,a) + r\mu(\emptyset,b) + \mu(\emptyset,X)$$
Because $\emptyset \leq a$, $\mu(\emptyset,\emptyset)+\mu(\emptyset,a)=0$. So, $\mu(\emptyset,a)=-1$.  
$$0 = 1+r\mu(\emptyset,b) + \mu(\emptyset, X)-3$$
So now we just need $\mu(\emptyset, b)$
$$0=\sum_{\emptyset\leq z\leq b} \mu(z,b)$$
$$0=1+\sum_{a\leq z\leq b} \mu(z,b)$$
$$0=1-n+\sum_{b\leq z\leq b} \mu(z,b)$$
$$0=1-n+\mu(z,b)$$
$$\mu(z,b)=n-1$$
So,
$$0 = r(n-1)+ \mu(\emptyset, X)-3+1$$
$$r={2-\mu(\emptyset,X)\over n-1}$$



##Exercise 4
(a)
$$s(i)=\sum_{j=1}^i f(j)$$
So, by mobius inversion:
$$f(n) = \sum_{j=1}^n \mu(j,n)s(j)$$
Pulling out the $j=n$ term of the sum
$$f(n) = \mu(n,n)s(n)-\sum_{j=1}^{n-1}\mu(j,n-1)s(j)$$
$$f(n) = s(n)-\sum_{j=1}^{n-1}\mu(j,n-1)s(j)$$
$$f(n) = s(n)-s(n-1)$$

(b)  
$$g(n) = \sum_{d|n}\mu(1,n/d)[ev(d)-od(d)]$$
(i)  
$g(1) = \mu(1,1)[0-1] = -1$  
$g(2) = \mu(1,2)[0-1] +\mu(1,1)[1-1]=1$  
$g(3) = \mu(1,3)[0-1]+\mu(1,1)[0-2]=-1$  
$g(4) = \mu(1,4)[0-1]+\mu(1,2)[1-1]+\mu(1,1)[2-1]=1$  

(ii)  
$$g(n) = \sum_{d|n}\mu(1,n/d)[ev(d)-od(d)]$$
Hypothesis: $g(n)=(-1)^n$  
So, by mobius inversion:  
$$[ev(n)-od(n)] = \sum_{d|n}g(d)$$
By hypothesis:
$$[ev(n)-od(n)] = \sum_{d|n}(-1)^d$$
$(-1)^n$ will be 1 for even numbers and -1 for odd. Thus, both sides of this equation count the number of even divisors minus number of odd divisors.  

$$g(n)=(-1)^n$$


***THE END***
