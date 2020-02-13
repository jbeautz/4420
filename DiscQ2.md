<font color = black>

Jack Beautz  
jpb375  

#Discussion Question 1  
###(a)
Find the inverse of $\pmatrix{1&2\\3&4}$ in $\mathbb{Z}_7$.  

$$A^{-1} = {1\over 4-6}\pmatrix{4&5\\4&1}$$
$$A^{-1} = 3\pmatrix{4&5\\4&1}$$
$$A^{-1} = \pmatrix{5&1\\5&3}$$

###(b)
Find RREF and Ker(A) in $\mathbb{Z}_{11}$.

$$A\sim \pmatrix{2&1&6&9\\3&0&2&4\\8&1&10&6}$$
$$A\sim \pmatrix{2&1&6&9\\0&4&4&7\\0&1&1&10}$$
$$A\sim \pmatrix{2&1&6&9\\0&4&4&7\\0&0&0&0}$$
$$A\sim \pmatrix{1&6&3&10\\0&1&1&10\\0&0&0&0}$$
$$A\sim \pmatrix{1&0&8&5\\0&1&1&10\\0&0&0&0}$$
We have reached Reduced Row Echelon Form.  

Using the RREF
$$x_1 + 8x_3 + 5x_4 = 0$$
$$x_2 + x_3 + 10x_4 = 0$$
And therefore,
$ker(A) = span\{\pmatrix{-8\\-1\\1\\0}, \pmatrix{6\\1\\0\\1}\}$
