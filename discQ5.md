<font color = black>

Jack Beautz  
jpb375  

#March 3rd Discussion Question 4
###The Partition Lattice

The atoms of $\pi_n$ takes the form $\{\{a_1,a_2\},\{a_3\},...,\{a_n\}$. Where each unique atom contains a unique pair of two elements followed by the remaining singletons.  
First consider the closure of two atoms where the associated pairs have no intersection. In this case the closure of sets $X_a=\{\{a_i,a_j\},\{a_1\},...,\{a_n\}\}$ and $X_b=\{\{a_k,a_l\},\{a_1\},...,\{a_n\}\}$ is $\{\{a_i,a_j\},\{a_k,a_l\},\{a_1\},...,\{a_n\}\}$. The closure of a two of atoms is the pairs in each atom along with the remaining singletons.  
Next consider the closure of two atoms where the associated pairs have a nonempty intersection. In this case the closure of $X_a=\{\{a_i,a_j\},\{a_1\},...,\{a_n\}\}$ and $X_b=\{\{a_j,a_k\},\{a_1\},...,\{a_n\}\}$ is $\{\{a_i,a_j,a_k\},\{a_1\},...,\{a_n\}\}$. The closure of the atoms is one subset containing the elements which were in the pairs and then the singletons not included in this subset of three elements.  
Closures of more than two atoms can be constructed by finding the closure of the the first two atoms and then the closure of that closure with the next atom. Continue until every atom is built into the closure.  

###L(E)
The atoms of $L(E)$ are the singleton vectors $\{v_1,...,v_n\}$. To construct the closure of the set of vectors $\{v_a,v_b,...,v_r\}$, check for linear independence. If there is a vector in the set which is linearly dependent on the rest, remove it. Continue inductively until the remaining set of vectors is linearly independent. In this way, the closure of atoms in $L(E)$ is a constructed basis for the set of vectors.   
