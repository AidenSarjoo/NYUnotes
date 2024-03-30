This is based off the *Numerical Analysis* course by Mingtao Xia at NYU Tandon. 

We refer primarily to the textbook [[SuliMayers.pdf|An Introduction to Numerical Analysis by Suli and Mayer]]. and briefly consult  [[Miller.pdf|Numerical Analysis for Engineers and Scientists by Miller]]
# Numerical Error
#todo
>[!Textbook]- 
><u>Textbook</u>: ![[Miller.pdf#page=15 | Chapter 1]]

# Iteration
>[!Textbook]- 
><u>Textbook</u>: ![[SuliMayers.pdf#page=12 | Chapter 1]]

**Brouwer's Fixed Point Theorem**: For a function $g$ defined and continuous on the interval $[a,b]$, where all $g(x) \in [a,b]$ for all $x \in [a, b]$. Then there exists $\xi \in [a,b]$ such that $\xi = g(\xi)$. The number $\xi$ is 
known as the fixed point of $g$.

Consider a function $f(x)$, where we want to find the solution $f(x) = 0$. Solve for $x$ algebraically as a function of itself, in the form $x = g(x)$. Apply the method of fixed point iteration to approximate a solution:

$x_{k+1}=g(x_k)$
## Newton's Method
>[!Textbook]- 
><u>Textbook</u>: ![[Textbooks/SuliMayers.pdf#page=32|Chapter 1.4]]  

$x_{k+1} = x_{k}- \dfrac{f(x_k)}{f'(x_k)}$

Converges quadratically for sufficiently large $k$

## Secant Method
>[!Textbook]- 
><u>Textbook</u>: ![[Textbooks/SuliMayers.pdf#page=36|Chapter 1.5]]  

Note the derivative approximation:

$f'(x_{k})\approx \dfrac{f(x_k)-f(x_{k-1})}{x_{k} - x_{k-1}}$

Apply the above to Newton's Method and define the Secant Method as:

$x_{k+1} = x_{k}- f(x_{k}) (\dfrac{x_{k}- x_{k-1}}{f(x_{k}) - f(x_{k-1})})$

## Bisection Method
>[!Textbook]- 
><u>Textbook</u>: ![[Textbooks/SuliMayers.pdf#page=39|Chapter 1.6]]  


Choose $a_0,b_0$ where $f(a_0)f(b_0) \lt 0$

$c_k = \dfrac{a_k+b_k}{2}$
1. if $f(b_k)f(c_{k}) > 0, (a_{k+1}, b_{k+1}) = (a_k, c_k)$
2. if $f(b_k)f(c_{k}) < 0, (a_{k+1}, b_{k+1}) = (c_k, b_k)$

Essentially, this is a binary search for roots

# Linear System of Equations 

## LU Decomposition
Consider a Matrix $A$, and the equation $A\vec{x} = \vec{b}$. We can decompose this matrix $A$ into two triangular matrices, specifically *lower triangular matrix* $L$ and *upper triangular matrix* $U$ so we arrive at the form $LU\vec{x} = \vec{b}$. We then solve as $U\vec{x} = \vec{y}, L\vec{y} = \vec{b}$, then solve $U\vec{x}=\vec{y}$ similarly. 

We can check the existence of this solution by *the leading principal submatrices*. If all leading principal submatrices $A_{i}$ of $A$ are non-singular ($det(A_{i})\neq0$), then this decomposition exists. If this decomposition does not exist, apply a *permutation matrix* $P$ such that the leading principal submatrices are non-singular. 

Calculate the values $l_{ij}$ of matrix $L$ and $u_{ij}$ of matrix $U$ with the following formulas:

$l_{ij} = \dfrac{1}{u_{jj}}(a_{ij})-\sum\limits_{k=1}^{j-1}l_{ik}u_{kj}$
$u_{ij} = a_{ij} - \sum\limits_{k=1}^{i-1}l_{ik}u_{kj}$

The total computational cost is then
$\sum\limits_{i=1}^{n} \sum\limits_{j=1}^{i}(2j-1)+\sum\limits_{i=1}^{n}\sum\limits_{j=1}^n(2i-2)$

We find the solution of the above method with:
$y_{i} = \sum\limits_{j=1}^{n}u_{ij}x_{j}$
$x_{i}=\dfrac{1}{u_{jj}}(y_{i}-\sum\limits_{j=i+1}^{n}u_{jj}x_{k})$

in total this is $O(n^2)$ 
# Matrix and Vector Norms

# QR Decomposition

# SVG Decomposition

# Least-Squares 

# Power Method 