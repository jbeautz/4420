<font color = black>  

Jack Beautz  
jpb375

#MATH 4420 Homework 5

###Exercise 1
Consider a single component of $G$ called $G_1$.  
Choose an edge $e\in E(G_1)$ and inductively calculate the chromatic polynomial of $M(G_1)$ with two base cases by choosing new edges to remove.
The first base case, the single independent element where two vertices are connected by a single edge. Second, the single dependent element defined as a single vertex with a loop edge.  
As defined, all possible colorings of the graph $G$ with $k$ components is defined as $\chi_{M(G)}(\lambda) =\prod_{i=1}^k \chi_{M(G_i)}(\lambda)$ because the colorings of each component is independent of the other components as they are not connected.  
To translate this to the graph coloring, note that in each component there is an arbitrary initial vertex which can be colored any of the $\lambda$ colors. From this initial vertex coloring, matroid dependencies define the number of remaining possible coloring. Hence, for each component in the graph, multiply by $\lambda$ to account for this initial choice on each unconnected component.  
Thus,
$$P_G (\lambda) = \prod_{i=1}^k \lambda\chi_{M(G_i)}(\lambda)$$
$$P_G (\lambda) = \lambda^k \chi_G(\lambda)$$


##Exercise 2
Consider the edge set $E$ and corresponding columns $C(E)$ which forms a circuit in $G$. We know by Lemma that the summation of all columns is the zero vector so $C(E)$ is a dependent set of vectors. Remove one of the edges from the circuit. Let the associated column vector be $v$.  Now the summation of all vectors in the set is $-v$, so the new edge set $E'$ is linearly independent. Note that $E'$ is a minimum spanning tree on the original circuit. Thus, $E'\subseteq \mathcal{I}(G)$. Any subsequent edge removal will continue to result in linearly independent edge sets until all edges are removed. If $E'\subseteq \mathcal{I}(G)$, then for any subset $E''\subseteq E'$, it must follow that $E''\subseteq \mathcal{I}(G)$. Hence, if the edge set corresponds to a linearly independent set of column vectors, the edge set does not form a circuit.  

Given the edge set $E$ is a subset of $\mathcal{I}(G)$, we know that the linear combination of all edges in the set is nonzero due to Lemma. Because this is in $\mathbb{Z}_2$ there are no scalar multiples but 0 and 1. Thus, if the linear combination of all column vectors is a vector $v$ in the set, linear combination of $E-\{v\}$ is 0 and this set forms a circuit. But, if this set forms a circuit, then it could not have been a subset of $\mathcal{I}$ in the first place. Thus, the linear combination of column vectors associated with the edge set must be nonzero. Hence, if $E\in \mathcal{I}(G)$, then the corresponding column vectors must be linearly independent.

Lemma: The only linear combination of all column vectors associated with edges is 0 if and only if the edges form a circuit and nothing but the circuit in the graph.

The edge set forms a circuit if every vertex is the end point of two edges. Thus, for each vertex there are two column vectors which have 1 in the row corresponding to the vertex. The summation of the two column vectors will be $1+1=0$ in $\mathbb Z_2$. Note in $\mathbb Z_2$ the only possible scalar multiples are 0 and 1, so if the column vector is in the linear combination, it is not multiplied by anything. Therefore, if the edge set forms a circuit, the summation and only linear combination including all edges will be 0.

If the linear combination of all column vectors is 0, then for each vertex there must be an even number of edges which have an endpoint on the vertex. There cannot be more than two edges which meet on the vertex because then there would be more edges than there are vertices and the circuit would not form a polygon.  Thus, if the linear combination is 0, the edges must all be included in a complete circuit.  


##Exercise 3
(a)  
The inclusion of a loop in a flat does not change the rank of the flat because the loop has a rank of 0. Consider the flat $F$ such that $r(F)=n$ with elements $\{x_1,...,x_r\}$. Let $\{y\}$ be any loop then, $F\cup\{y\}=F$. We can join the set of all loops such that $F\cup\{y_1,...,y_m\}=F$ and $r(F)=n + 0 +...+0= n$. Hence, every flat includes the set of all loops just as all flats include the empty set.  

To find the minimal element of the combinatorical geometry, take the meet of all elements, or in this case the intersection of all sets of elements. As established above, the set of all loops in every subset. Thus, it is the intersection if there exists loops. Otherwise, the empty set is the intersection because it is included in every set, including the set of loops if loops exist.  

(b)  
Reflexive: $x \sim x$ because the relation is defined such that $x\sim y$ if $x=y$. $x=x$ so $x\sim y$.  

Symmetric: If $x\sim y$, then either $x=y$ or the set $\{x,y\}$ is dependent but $\{x\}$ and $\{y\}$ are independent. If $x=y$, then $y=x$ and $y\sim x$. If $\{x,y\}$ is dependent but $\{x\}$ and $\{y\}$, then $\{y,x\}$ is dependent and $\{y\}$ and $\{x\}$ are independent. Thus, $y\sim x$.  

Transitive: If $x\sim y$ and $y\sim z$, if there is any pair wise equality among $x,y,z$, then transitivity follows trivially. Otherwise, $\{x\}$,\{y\},\{z\}$ are all independent.  $\{x,y\}$ and $\{y,z\}$ are not independent sets. So $\{x,y,z\}$ is not an independent either. We know $\{y\}$ is independent so we remove that to the set and decrease the rank by 1. This leaves $\{x,z\}$ as a set of rank 1, thus the elements are dependent. $x\sim z$.  

$(c)$  
Suppose there exists a rank 1 element $\{x,y\}$ in the matroid which was not a parallel class. Because this element is not a parallel class, $r(x)+r(y)=r(\{x,y\})$. Hence, without loss of generality, say $r(x)=1$. Then, for $\{x,y\}$ to have rank 1, $r(\{y\})=0$. But there are no loops in the matroid. Hence, this is impossible. All rank one elements are parallel classes.  

Let $F$ be a flat which a union of parallel classes $\{x_1,y_1\},...,\{x_n,y_n\}$ and another element $z$ where $z$ is not a parallel class. As established above, this implies that $z$ has rank greater than 1, because all rank 1 elements are parallel classes and there are no loops. Because $r(\{z\})> 1$, $z$ must be the union of lower rank elements. These lower elements must be parallel classes because they are the only matroid elements of rank 1. Hence, $z$ is also the union of parallel classes. So the flat $F$ must be the union of parallel classes if it is the union of anything.   







***THE END***
