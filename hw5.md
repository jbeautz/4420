<font color = white>  

Jack Beautz  
jpb375

#MATH 4420 Homework 5

###Exercise 1
Consider a single component of $G$ called $G_1$.  
Choose an edge $e\in E(G_1)$ and inductively calculate the chromatic polynomial of $M(G_1)$ with two base cases by choosing new edges to remove.
The first base case, the single independent element where two vertices are connected by a single edge. Second, the single dependent element defined as a single vertex with a loop edge.  
For multiple components, simply multiply these chromatic polynomials to get a new chromatic polynomial for the entire matroid of all components of the graph.  
To translate this to the graph coloring, note that in each component there is an arbitrary initial vertex which can be colored any of the $\lambda$ colors. From this initial vertex coloring, matroid dependencies define the number of remaining possible coloring. Hence, for each component in the graph, multiply by $\lambda$ to account for this initial choice on each unconnected component.  
As defined, all possible colorings of the graph $G$ with $k$ components is defined as $\chi_{M(G)}(\lambda) =\prod_{i=1}^k \chi_{M(G_i)}(\lambda)$ because the colorings of each component is independent of the other components as they are not connected. 


##Exercise 2
Consider the edge set $E$ and corresponding columns $C(E)$ which forms a circuit in $G$. We know by Lemma that the summation of all columns is the zero vector so $C(E)$ is a dependent set of vectors. Remove one of the edges from the circuit. Let the associated column vector be $v$.  Now the summation of all vectors in the set is $-v$, so the new edge set $E'$ is linearly independent. Note that $E'$ is a minimum spanning tree on the original circuit. Thus, $E'\subseteq \mathcal{I}(G)$. Any subsequent edge removal will continue to result in linearly independent edge sets until all edges are removed. If $E'\subseteq \mathcal{I}(G)$, then for any subset $E''\subseteq E'$, it must follow that $E''\subseteq \mathcal{I}(G)$. Hence, if the edge set corresponds to a linearly independent set of column vectors, the edge set does not form a circuit.  

Given the edge set $E$ is a subset of $\mathcal{I}(G)$, we know that the linear combination of all edges in the set is nonzero due to Lemma. Because this is in $\mathbb{Z}_2$ there are no scalar multiples but 0 and 1. Thus, if the linear combination of all column vectors is a vector $v$ in the set, linear combination of $E-\{v\}$ is 0 and this set forms a circuit. But, if this set forms a circuit, then it could not have been a subset of $\mathcal{I}$ in the first place. Thus, the linear combination of column vectors associated with the edge set must be nonzero. Hence, if $E\in \mathcal{I}(G)$, then the corresponding column vectors must be linearly independent.

Lemma: The only linear combination of all column vectors associated with edges is 0 if and only if the edges form a circuit and nothing but the circuit in the graph.

The edge set forms a circuit if every vertex is the end point of two edges. Thus, for each vertex there are two column vectors which have 1 in the row corresponding to the vertex. The summation of the two column vectors will be $1+1=0$ in $\mathbb Z_2$. Note in $\mathbb Z_2$ the only possible scalar multiples are 0 and 1, so if the column vector is in the linear combination, it is not multiplied by anything. Therefore, if the edge set forms a circuit, the summation and only linear combination including all edges will be 0.

If the linear combination of all column vectors is 0, then for each vertex there must be an even number of edges which have an endpoint on the vertex. There cannot be more than two edges which meet on the vertex because then there would be more edges than there are vertices and the circuit would not form a polygon.  Thus, if the linear combination is 0, the edges must all be included in a complete circuit.  





***THE END***
