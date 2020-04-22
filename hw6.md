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
The first term of the characteristic polynomial is $\lambda^{r(X)}$ for any matroid, so it must be for this one.  
As discussed in Exercise 1, the second term will be negative and count the number of distinct rank 1 subsets of the ground set.  There are no loops in $M$ so all subsets are of cardinality at least 1 so the only rank 1 subsets of $X$ are the parallel classes. Hence, the second term in the polynomial must be $-p\lambda^{r(X)-1}$, the number of parallel classes times $\lambda$ raised to the power of the rank of $X$ minus the rank of rank 1 subsets.  

##Exercise 4
Let $a_i=|A_i|$ where $A_i = \{Y\subseteq X: r(Y)=i\}$.  
By defintion of rank, if $r(Y)\leq |Y|$.  
As discussed earlier the absolute value of the coefficient of the $i$th term in the polynomial is $a_i$. The maximum value possible for $a_i$ occurs when all cardinality $i$ subsets have full rank.  In this case $a_i$ is the number of $i$ subsets in the base set $X$. Hence, $a_i\leq {|X|\choose i}$

Note, this maximal $a_i$ events occurs only when all $i$ subsets have full rank. 







***THE END***
