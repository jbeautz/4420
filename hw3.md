<font color = white>  

Jack Beautz  
jpb375  

#MATH 4420 Homework 3

##Exercise 1

##Exercise 2
(a) There are $q^n$ was to choose $n$ elements out of the $q$ possibilities in the field.  
But to create a subspace we should only consider the $q^n-1$ possibilities not including all all $0$ elements for the $n$ elements.  

Now, there are $q-1$ ways to multiply a vector by a nonzero scalar in $F_q$.  

Hence, for each one dimensional vector in $F_q$ there are ${q^n-q}\over q-1$ forms.  
This defines $(n) = 1 + ... + q^{n-1}$.  

Now that we have adjusted for the finite field with $q$ elements, we can consider this problem in the standard sense of choosing $k$ linearly independent vectors to form a $k$ dimensional space in $F^n$.  

The number of ways to do this is the standard $n\choose k$ formula but with the $q^n-1\over q-1$ forms of each vector selected in $F_q$ we have the given formula.  

(b)  
Consider any $n$ linearly independent vectors which span $F^n$. Form a $k\times n$ matrix such that the entries to each column index the $n$ linearly independent vectors such that each column denotes a $k$-dimensional subspace spanned by $k$ out of the $n$ vectors.  
The number of $k$ dimensional subspaces of $F_n^k$ is equivalent to all $k\times n$ matrices with an equivalent row space to the matrix formed above.  
Thus, there are $q-1$ non zero scalars to multiply the first row by and $q-2$ scalars remaining to multiply the second matrix by and so on. This pattern continues until all rows have been rearranged using row operations to create all possible matrices with equivalent row spaces.
Therefore $[{n\choose k}]_ q$ is the number of row rearrangements to $k\times n$ matrix in $F_q$.  

##Exercise 3
(a)  
By Inclusion Exclusion.  
$$dim U + dim W = dim(U\cup W) + dim(U\cap W)$$
$$dim U + dim W - dim(U\cap W) = dim(U\cup W)$$
When rearranged it becomes clear that the dimension of $U\cup W$ is equivalent to the dimension $U$ plus the dimension of $W$ minus the dimension of $U\cap W$. Consider $v\in U\cap W$ such that $v$ is a basis vector in basis $B_W$ and a basis vector in $B_U$.  If we count the 1 dimension defined by $v$ in both $U$ and $W$ it will be double counted as that 1 dimension is spanned by 1 basis vector $v\in U\cap W$.  

(b)  
Assume for the sake of contradiction that
$$r(A) + r(B) < r(A\cup B) + r(A\cap B)$$
Part (a) demonstrated that for finite $V$,
$$dim(A) + dim(B) = dim(A\cup B) + dim(A\cap B)$$
Hence, the initial assumption was false. Therefore,
$$r(A) + r(B) \geq r(A\cup B) + r(A\cap B)$$







***THE END***
