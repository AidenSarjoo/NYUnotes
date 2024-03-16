This is based off the *Design and Analysis of Algorithms* course by Boris Aronov at NYU Tandon. 

This document also borrows heavily from Greg Aloupis' former *Design and Analysis of Algorithms* course. Refer to [his course overview](https://research.engineering.nyu.edu/~greg/algorithms/2413/resources.html) and [explanations](https://research.engineering.nyu.edu/~greg/algorithms/scribbles.pdf).

We also consult [the Holy Bible](obsidian://open?vault=Algo&file=Textbooks%2FCLRS.pdf) 

# Syllabus
- [[Notes#Pre-requisites|Pre-Requisites]]
- [[Notes#Big O Notation|Big O Notation]]
- [[Notes#Recurrence|Recurrence]] 
	- [[Notes#Recurrence#Master Theorem |Master Theorem]] 
	- [[Notes#Recurrence#Inductive Proof|Inductive Proof]] 
- [[Notes#Merge Sort|Merge Sort]]
- [[Notes#Heaps and Heap Sort|Heaps]]
- [[Notes#Selection|Selection]] 
- [[Notes#Quick Sort|Quick Sort]] 
- [[Notes#Linear-Time Sorting|Linear-Time Sorting]]
# Pre-requisites
#todo 

# Big O Notation

>[!Textbook]- 
><u>Textbook</u>: ![[CLRS.pdf#page=64 |CLRS Chapter 3]]  

Consider a function $f(n)$, some constant $n_0$ where $n > n_0$, and constants $c,d$:
- If $f(n) \leq c\cdot g(n)$, then $f(n) = O(g(n))$
- If $f(n) \geq d\cdot g(n)$, then $f(n) = \Omega(g(n))$
-  If $f(n) \leq c\cdot g(n)$ and $f(n) \geq d\cdot g(n)$, then $f(n) = \Theta(g(n))$

When proving these bounds, let $n_0$ be any value sufficient to do so
# Recurrence

## Master Theorem:

>[!Textbook]- 
><u>Textbook</u>: ![[CLRS.pdf#page=115 |CLRS Chapter 4.3]]
>

For the recurrence relation $T(n) = aT\left(\frac{n}{b}\right)+ f(n)$, the run-time is given by one of three cases:
1. If $f(n) = O(n^{\log_{b}a-\epsilon}), \text{ then } T(n) = \Theta(n^{\log_{ b }a})$    
2. If $f(n) = O(n^{\log_{b}a}), \text{ then } T(n) = \Theta(n^{\log_{ b }a} \  lg(n))$ 
3. If $f(n) = O(n^{\log_{b}a+\epsilon}), \text{ and if } a f\left(\frac{n}{b}\right)\leq c f(n) \text{, then } T(n) = \Theta(f(n))$ 
## Inductive Proof

For the recurrence relation $T(n) = a_{1}T\left(\frac{n}{b_{1}}\right) + a_{2}T\left(\frac{n}{b_{2}}\right) + ... + a_{m}T\left(\frac{n}{b_{m}}\right) + O(g(n))$   
1. Claim a solution: $T(n) = O(f(n))$ 
2. $T(n) \leq cf(n)$ 
3. Assume $T(k) \leq cf(k)$ for $k \lt n$
4. Prove that the claim holds for $n$:
	1. $T(n) \leq a_{1}cf(\frac{k}{b_{1}}) + a_{2}cf(\frac{k}{b_{2}}) + ... + a_{m}cf(\frac{k}{b_{m}}) + O(g(k))$  
	2. Choose some $c \ \text{s.t.}$ : $a_{1}cf(\frac{k}{b_{1}}) + a_{2}cf(\frac{k}{b_{2}}) + ... + a_{m}cf(\frac{k}{b_{m}}) + O(g(k)) \leq f(n)$ 

# Merge Sort
#todo
>[!Textbook]- 
><u>Textbook</u>: ![[CLRS.pdf#page=51 |CLRS Chapter 2]]  

# Heaps and Heap Sort
#todo
>[!Textbook]- 
><u>Textbook</u>: ![[CLRS.pdf#page=172 |CLRS Chapter 6]]  

# Selection
#todo
>[!Textbook]- 
><u>Textbook</u>: ![[CLRS.pdf#page=234 |CLRS Chapter 9]]  

# Quick Sort
#todo
>[!Textbook]- 
><u>Textbook</u>: ![[CLRS.pdf#page=191 |CLRS Chapter 7]]  

# Linear-Time Sorting
#todo
>[!Textbook]- 
><u>Textbook</u>: ![[CLRS.pdf#page=212 |CLRS Chapter 8]]  
> 

