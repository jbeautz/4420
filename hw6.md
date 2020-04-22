<font color = white>

Jack Beautz  
jpb375  

#MATH 4420 Homework 6

##Exercise 1
$$\chi_M (\lambda) = \sum_{A\subseteq X} (-1)^{|A|}\lambda^{r(X)-r(A)}$$

The coefficient of $\lambda^{r(X)-1}$ will be the number of $A\subseteq X$ which have $r(A)=1$ times.  
This coefficient must be negative because if $r(A)=1$, $|A|$ must be one in a simple matroid.
The set of distinct rank 1 subsets must be the set of singletons because there are no loops in a simple matroid. Hence, the cardinality of the set of rank 1 subsets is $|X|$. Thus, the next term of $\chi_M(\lambda)$ is $-|X|\lambda^{r(X)-1}$.  


##Exercise 2
We know $x,y$ are parallel, so they cannot be coloops.  
Without loss of generality choose $x$.
$$\chi_M(\lambda)=\chi_{M-x}(\lambda)+\chi_{M/x}(\lambda)$$
But upon the contraction of a $x$, $y$ becomes a loop. Thus, there is no proper coloring of the matroid with $x$ contracted. This part of the summation goes to zero.  
$$\chi_M(\lambda)=\chi_{M-x}(\lambda)$$

##Exercise 3








***THE END***
