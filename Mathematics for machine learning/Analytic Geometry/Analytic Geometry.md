#### Norms
Норма [[Vector]] в векторном пространстве V определяется следующим образом:
$$
||.||:V\rightarrow\mathbb{R},
$$$$
x\rightarrow ||x||
$$
т.е. норма - это функция, которая дает вектору x его длину, и имеет следующие свойства:
![[Pasted image 20250504122531.png]]

Виды норм:
1. [[Manhattan Norm]]
2. [[Euclidean Norm]]

#### Inner Products
##### Dot Product
[[Multiplication]]
##### General Inner Products
В обычных [[Linear Algebra#Linear Mappings]] на вход функции подавался только один параметр. В билинейном отображении два аргумента, и оба линейные:
$$
\Omega(\lambda x + \psi y, z)= \lambda\Omega(x, z) + \psi\Omega(y, z)
$$
$$
\Omega(x, \lambda y + \psi z) = \lambda\Omega(x, y) + \psi\Omega(x, z)
$$
Билинейное отображение может быть симметричным, если $\Omega(x, y) = \Omega(y, x)$ и положительно определенным, если $$
\forall x\in V /\{0\}:\Omega(x, x)> 0, \Omega(0, 0)= 0
$$
##### Symmetric, Positive Definite Matrices
Симетричная матрица - матрица с одинаковыми значениями по сторонам от главной диагонали.
Симметричная матрица А считается положительно направленной, если
![[Pasted image 20250506102550.png]]
больше 0 для любого x из V\\{0}.

