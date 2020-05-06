<font color = black>

Jack Beautz  
jpb375
#May 5 Discussion Question 3

Let $A$ be a rank $r$, $r\times n$ totally unimodular matrix.  Find a simple formula involving a determinant which computes the number of bases for the matroid we usually associate to this matrix.  

##Solution
$A$ is a totally unimodular matrix, so it must be regular. Consider the graph associated with the matroid. The spanning trees over this graph form the bases of the matroid. Thus, using Matrix Tree Theorem, we can count the number of bases, which is equivalent to the number of spanning trees, by calculating the determinant of the matrix $D-A$.  
