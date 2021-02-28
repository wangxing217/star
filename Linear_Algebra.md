# 线性代数的本质
线性代数是什么？行列式里面用到了，矩阵乘法用到了，求特征值用到了  
[see the video](https://www.bilibili.com/video/BV1ys411472E)
## Chapter 1
Vector, what even they are ? 什么是向量
> 1.学物理的认为 它是有方向和长度决定的；学数学的认为它是由坐标系中的值决定的也就是一组列表圈起来的值.   
   2.向量的运算其实 无非就是加法和乘法。加法是位移，乘法是缩放，标量scalar 其实scaling 缩放。

## Chapter 2
Linear combinations spans and bases. 向量的**线性组合(Combinations)** 和它张成的 **空间(span)** 和 **基(basis)** 。    
1. 线性组合 $$ a*\vec{v}+b*\vec{w} $$
2. 空间(span)   
   The 'span' of $\vec{v}$ and $\vec{w}$ is the set of all their linear combinations.   
   这里的span就是指这两个向量的 **线性组合** 张成的空间，也就是所以线性组合的集合。  
3. 基(basis)   
   The basis of a vector space is a set of **linerly independent** vectors that span the full space.    
   向量空间的 **一组基** 是张成该 **空间** 的一个 **线性无关** 向量集

## Chapter 3
Matrix as linear transformations.  矩阵 和 线性变换 的关系   
1. Linear **transformations**   
   transformations 本质上就是函数，输入一个向量$\vec{v}$，经过函数$L(\vec{v})$，输出一个向量$\vec{w}$
$$
\begin{pmatrix}
2\\   
3
\end{pmatrix}
\rightarrow 
L(\vec{v})
\rightarrow 
\begin{pmatrix}
4\\   
25
\end{pmatrix} 
$$
$$
\begin{pmatrix}
x_{in}\\ 
y_{in}
\end{pmatrix}
\rightarrow 
???
\rightarrow 
\begin{pmatrix}
x_{out}\\ 
y_{out}
\end{pmatrix}
$$
变换矩阵中的给个列向量 可以看作是 **新基** 。
$$
\begin{bmatrix}
a &b \\     
c &d
\end{bmatrix}
\begin{bmatrix}
x \\     
y
\end{bmatrix}
=x
\begin{bmatrix}
a \\      
c
\end{bmatrix}
+y
\begin{bmatrix}
b \\      
d
\end{bmatrix}
=
\begin{bmatrix}
ax+by \\       
cx+dy
\end{bmatrix}
$$

2. 矩阵   
现在来理解一下 **矩阵** ，每一列其实就是变换后的新基，例如 $3\*3$ 的矩阵，那么表示的就是原始的三维空间中的三个基在变换后的基，如果此时是 $3\*2$，那么表示的就是原始的3个基在做变换的时候，向低维空间投影了，换句话数就是舍掉了一维。
## Chapter 4 
Matrix multiplication as composition 线性复合变换 和 矩阵乘法   
复合变换 和 矩阵乘法的关系就是 复合函数 $f(g(\vec{x}))$

## Chapter 5 
The determinant 行列式   
问题的引出：在我们知道了矩阵乘法是对向量进行 **旋转或者拉伸** 后，那么这个左乘的矩阵到底对向量影响多大呢？其实也就是对旧的基的影响。   
答案：行列式表示的就是这个影响，即 线性变换对旧基的 '空间' 造成的影响。 当行列式为0时，表示将空间压缩到了0. 也就是降维了。

## Chapter 6 
Inverse matrices, column space, rank and null space 逆矩阵，列空间，零空间 秩 和 零空间。   
逆矩阵：左乘一个矩阵等于一次变换，那么在左乘一个矩阵将它变回来就是这个矩阵的逆矩阵，也就是矩阵和逆矩阵的 乘积 等于什么也没做，这个什么也没做就是 单位阵。
$A^{-1}A=I$   

列空间：矩阵的列是 变换后的基向量，这些基向量张成的空间就交 列空间，也就是 $A\vec{x}$ 构成的空间。   
秩：就是压缩后的空间维数，其实也是 列空间 的维数。
零空间：变换后一些向量落在了零向量上面，这些向量构成的空间就是 **零空间[Null Space]** 

## Chapter 7
Dot products and cross products 点积与叉积

## Chapter 8 
Change of basis 基变换

## Chapter 9 
Eigenvectors and eigenvaluse 特征值和特征向量

## Chapter 10 
Abstract space vector spaces 抽象的向量空间





