<font color = white>  

Jack Beautz  
jpb375  

#MATH 4420 Prelim 1
##Question 1
Proof by Induction:  
Base Case: $t=2$  

- Claim: If every two subset is in a unique block of $P$, then $b_{t,v} = v$. For $x\in P$, denote by $r_x$ the number of blocks containing $x$, and similarly for $B\in\mathcal B$, let $k_B=|B|$. This is not the trivial case so there is more than one block. If $x\not\in B$ then $r_x\geq k_L$ because there are $k_B$ other blocks containing $x$. Suppose $b\leq v$. Then $b(v-k_B)\geq v(b-r_x)$. Now counting this two ways we find
$$1= \sum_{x\in P}\sum_{B\ni x} {1\over v(b-r_x)}\geq \sum_{B\in\mathcal B}sum_{x\not\in B} {1\over b(v-k_L)} = 1$$
and this implies that in all inequalities, equalities must hold. Hence, $b= v$.  

Plugging in $b_{t,v}=v$ in the expression leads to
$$b_{t,v}(b_{t,v}-1) \geq t{v\choose t}$$
$$v(v-1)\geq {2v!\over 2!(v-2)!}$$
$$v(v-1)\geq v(v-1)$$

Hence, equality holds at the base case.  





The minimum size of a block is $2$ because it must at least contain one two subset. Let the first element of $P$ be $a_1$ such that $\{\{a_1,a_2\}, \{a_1, a_3\},...,\{a_1,a_v\}\subseteq \mathcal B$.  Then $|\mathcal B|=v-1$. But this pairing does no include the $t$-subsets $\{a_i,a_j\}$ for $1<i<j<v$. Including one more block in $v$ can
