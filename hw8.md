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








***THE END***
