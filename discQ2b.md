<font color = black>  

Jack Beautz  
jpb375  

#Discussion Question 2b
####Prove that an edge of G is a coloop of M(G) if and only if removing it from the graph (but leaving all vertices intact) increases the number of components of G by one.

$$\to$$
Removing an edge $e$ from the graph increases the number of components by one.
Therefore the edge must be an isthmus which is not part of a cycle and both sides of the edge are the same outer space of the graph.
Graphically, the dual $G^{* }$ will contain the corresponding dual edge $e^{* }$ where the the dual edge begins in the space around the graph, crosses $e$ and then connects back to the same outer space, forming a loop.  

Therefore $e$ corresponds to a loop in the dual graph and is by definition a coloop.  

$$\leftarrow$$
An edge $e$ of $E(G)$ is a coloop of $M(G)$.
Then there is a corresponding edge in the dual graph of $G$ which is a loop.
We know the dual of the dual is the original matroid.
So $e$ is an edge which connects the space inside the loop in the dual to the space outside the loop in the dual.
$e$ is the only edge with a vertex corresponding to the space inside the loop.
Hence, $e$ is an isthmus and its removal would separate the component it is contained in.  

Finally, this results in an additional component when removed.  


***THE END***
