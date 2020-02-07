<font color=black>

Jack Beautz  
jpb375  
#Discussion Questions Week 2
###1A+B
 $t-(v,k,\lambda)$ is also a $t-j$ design by thm 19.3, so every $t-j$ subset is in the same number $\mu_j$ of $k$-blocks. Remove the $\mu_j$ $k$-blocks that contain the $(t-j)$-subset and $J$. This union is a $t$-subset, because our $t-j$ were in $P'$ and hence disjoint from $J$. The number of blocks that contain a $t$-subset is $\lambda$, the same regardless of which $t-j$ set we chose. So, $\mu_j-\lambda$ $(k-j)$-blocks contain any given $(t-j)$-subset. 1(a) follows when $j=1$.

###1E
Formula 19.2 gives an expression for number of blocks incident with no points in a $i-subset$.
$$b_i = \lambda {{v-i\choose t-i}\over {k-i\choose t-i}}$$

Let $i=t-j$ and $\lambda' = b_i$.
$$\lambda' = \lambda {{v-t+j\choose j}\over {k-t+j\choose j}}$$
$$\lambda' = \lambda {{v-t+j\choose j}\over {k-t+j\choose j}}$$

$\mu_j=\lambda' - \lambda$ because the $t-1$ subsets should not be contained in blocks of $\mathcal{B}$ which have a nonempty intersection with $J$.

Hence,
$$\mu_j = \lambda - \lambda {{v-t+j\choose j}\over {k-t+j\choose j}}$$
$$\mu_j = \lambda(1-{{v-t+j\choose j}\over {k-t+j\choose j}})$$
