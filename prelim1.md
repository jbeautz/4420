<font color = white>  

Jack Beautz  
jpb375  

#MATH 4420 Prelim 1
##Question 1
Proof by Induction:  
Base Case: $t=2$  

- Claim: If every two subset is in a unique block of $P$, then $b_{t,v} = v$. For $x\in P$, denote by $r_x$ the number of blocks containing $x$, and similarly for $B\in\mathcal B$, let $k_B=|B|$. This is not the trivial case so there is more than one block. If $x\not\in B$ then $r_x\geq k_L$ because there are $k_B$ other blocks containing $x$. Suppose $b\leq v$. Then $b(v-k_B)\geq v(b-r_x)$. Now counting this two ways we find
$$1= \sum_{x\in P}\sum_{B\ni x} {1\over v(b-r_x)}\geq \sum_{B\in\mathcal B}\sum_{x\not\in B} {1\over b(v-k_L)} = 1$$
- this implies that in all inequalities, equalities must hold. Hence, $b= v$.  

- Plugging in $b_{t,v}=v$ in the expression leads to
$$b_{t,v}(b_{t,v}-1) \geq t{v\choose t}$$
$$v(v-1)\geq {2v!\over 2!(v-2)!}$$
$$v(v-1)\geq v(v-1)$$

Hence, equality holds at the base case.  

Step Case:
- Count the number of ordered subsets containing all $t$-subsets.  Let this number be $N$. Let $\mathcal T$ be the set of all $t$-subsets of $P$. For any $t$ count $N$ two ways: $\forall T\in \mathcal T$, number of $B$ containing $T$, and $\forall B\in \mathcal B$, number of $t$-subsets contained in $B$.  

$$\sum_{T\in \mathcal T}\sum_{B\supseteq T} 1 \geq \sum_{B\in \mathcal B}\sum_{T\subseteq B} 1$$

By the LHS of the inequality,
$$N= \sum_{T\in \mathcal T}\sum_{B\supseteq T} 1 $$
There are $v\choose t$ unique $t$-subsets to be concerned about.
$$N= {v\choose t}\sum_{B\ni x} 1$$
But there can only be 1 block which contains each $t$-subset.  
$$N= {v\choose t}$$

By the RHS of the inequality,
$$N= \sum_{B\in \mathcal B}\sum_{T\subseteq B} 1$$
But we know there are a minimum of $b_{t,v}$ blocks to sum through.  
$$N = b_{t,v}\sum_{T\subseteq B} 1$$
Let $l_i$ be the cardinality of the $i$th block. In this block there are $l_i\choose t$ $t$-subsets. Then the maximum size of a block is $v\over b_{t,v}$. Thus the maximum number of subsets is ${v\over b_{t,v}}\choose t$




##Question 2














**THE END**
