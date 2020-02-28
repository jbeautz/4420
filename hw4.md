<font color = "white">  

Jack Beautz  
jpb375  

#MATH 4420 Homework 4

##Exercise 1
Let $\{a_1,...,a_r\}$ be the set of points which cover $a$.  
Let $x\in \{a_1,...,a_r\}$ and $y\in [a,b]$.  
The interval of $L$ is atomic if $y$ can be written as the join of points in $[a,b]$.  

Consider $y_1$ which covers $a$. By semi modularity, we know $x\lor y_1$ covers $y_1$.  

Next consider $y_k$ which covers $y_{k-1}$. Since $x\lor y_{k-1}$ covers $y_{k-1}$, by semimodularity $x\lor y_k$ covers $y_k$.  

Continue inductively until you find that $y_k = y$. Thus $y$ is a join of points which cover $a$.  

Any $y\in [a,b]$ can be constructed in this way because of the semimodularity and lattice structure of the geometric lattic $L$.  


Consider $y_0\in [a,b]$ such that it cannot be constructed in this way. $y_0 > a$ and greater than each $a_i$. Let $z\in L$ be an element outside the interval such that $y_0\land z = a$. By definition, $z\not\in [a,b]$. Consider without loss of generality that $z<a$. Then, $z \land y_0 < a$. This is a contradiction to the assumption that $z\land y_0 = a$.  

Therefore, the interval of the lattice is atomic.  

##Exercise 2
Because $E$ is finite, $(E, F_E)$ is a combinatorical design if   
(i) $F_E$ is closed under intersection  
(ii) $\emptyset$,$E$ and singletons $\{x\}\in F_E$ are contained in $F_E$.  
(iii) $\forall x\in E-G$, $\exists ! H\in F$ such that $H$ covers $G$ and $x\in H$.  

First consider (i). Let $U$ and $W$ be subspaces of $V$. Let $G\in F_E$ and $H\in F_E$ such that they correspond with the intersection of $E$ and $W$ or $U$ respectively.  $H\cap G$ is defined as $\{E\cap U \cap W: U,W\subseteq V\}$. Note that $U\cap W\subseteq V$ because $U\subseteq V$ and $W\subseteq V$. Thus the intersection of flats $H$ and $G$ is a flat $F'$ such that $F'$ corresponds to the intersection of $E$ and $(U\cap W)$.  

Now consider (ii). $\emptyset\in F_E$ is defined as $\{E\cap U: U\subseteq V\}$ where $U\cap E = \emptyset$. $E\in F_E$ is defined as $\{E\cap E: E\subseteq V\}$. Every vector in $E$ is included in the intersection. Finally, define the set of subspaces $U_1,...,U_n$ such that $U_i = span(v_i)$, $\forall v_i\in E$. There exists a flat corresponding to each singleton $v_i$ defined as $\{E\cap U_i: U_i \subseteq V\}$.  

Finally consider (iii). Let $v_k\in E-G$ such that $H$ covers $G$ and $\{v_k\}$. If $H$ covers $G$ and $\{v_k\}$ then $H$ is defined as $\{E\cap ((E-G) \cap \{v_k\}):((E-G) \cap \{v_k\})\subseteq V\}$. Hence, $H$ exists. Suppose $H$ was not unique for each $v_k$. 





***THE END***
