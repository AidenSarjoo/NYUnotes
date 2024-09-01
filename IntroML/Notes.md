This follows Christopher Musco's class at NYU, [CS-UY 4563 Introduction to Machine Learning](https://www.chrismusco.com/introml2020/) through the online resources. Homework solutions are in the Problems folder or Code folder (.ipynb files cannot be viewed natively in Obsidian unfortunately). 

# Intro
>[!Sources]- 
>[Musco Lec 1](https://www.chrismusco.com/introml2020/lectures/lec1.pdf)
>[Musco Lec 2](https://www.chrismusco.com/introml2020/lectures/lec2_annotated.pdf)

We use Machine Learning to solve problems of the form:
- **Input**: A piece of data
- **Output**: A decision (what something is) or prediction (what something will be).

## Example: OCR
A common example problem is *OCR*, Optical Character Recognition, where given handwritten characters we attempt to identify the character, i.e. a series of handwritten numbers could be turned into their int representation.

The machine learning approach to this problem is as follows:
- **Input:** An image of a handwritten number
- **Output:** The integer representation of the image

We collect (input, output) pairs $(\vec{x_{i}} \in \mathbb{R}^{28 \times 28},y_{i}\in \{0,1,...,9\})$, also known as the *training dataset*. Now we seek to find a function $f(\vec{x})$ s.t. $f(\vec{x_{i}}) = y_i$%%(this is a function interpolation?)%%.  The standard dataset for this problem is [MNIST](http://yann.lecun.com/exdb/mnist/), and the images in MNIST are $28 \times 28$ (hence $\vec{x_{i}} \in \mathbb{R}^{28 \times 28}$).
## 
Learning a function $f$ from labeled data (an input/output pair) is known as supervised learning. There are two types of supervised learning we consider:
- **Classification:** Prediction of a discrete class label
- **Regression:** Prediction of a continuous value

Later, we dedicate time to *unsupervised learning*, and *reinforcement learning*.

Some questions we seek to answer through this course in pursuit of these functions $f(\vec{x})$ are:
- How do we parametrize a class of functions $f$?
- How do we efficiently find a suitable function $f$ in that class?
- How do we ensure that the function $f$ will perform well on data out of its training data?
- How do we deal with non-ideal training data? 

# Linear Regression
>[!Sources]- 
>[Musco Lec 2](https://www.chrismusco.com/introml2020/lectures/lec2_annotated.pdf)
>[[Freund.pdf|Fruend's Mathematical Statistics with Applications]]

## Introduction to Regression
Regression is a statistical method that seeks to predict the value of a dependent variable based on the values of independent variables. We might consider the *bivariate regression* on independent random variable $X$ and dependent random variable $Y$, with joint density function $f(x,y)$, and the conditional density of $Y$ given $X=x$ $w(y|x)$ where we evaluate the following integral:
- $\mu_{Y|x}=E(Y|x)=\int_{-\infty}^{\infty}y \cdot w(y|x)dy$

Recall the calculation of $w(y|x)$ where we use the marginal density of $X$: $g(x)$:
- $g(x) = \int_{-\infty}^{\infty}f(x,y)dy$
- $w(y|x) = \dfrac{f(x,y)}{g(x)}$

A linear regression is a regression equation of the form:
- $\mu_{Y|x}=\alpha+\beta x$

with regression coefficients $\alpha$ and $\beta$

## Simple Linear Regression
See the associated [[IntroML/Code/demo_auto_mpg.ipynb|demo]] for an introduction to pandas as well as demonstrations of the following material. 

