This is based off the course by Jinghua Qian at NYU Tandon and closely follows [[Freund.pdf|Freund's Mathematics Statistics with Applications]] 

# Syllabus
- Probability
- Chapter 7: Functions of Random Var.
- Chapter 8: Sampling
- Chapter 10: Point Estimation
- Chapter 11: Interval Estimation
- Chapter 12: Hypothesis Testing

# Probability 

# Functions of Random Variables
>[!Textbook]- 
><u>Chapter 7</u>: ![[Freund.pdf#page=213|Chapter 7]] 

# Sampling
>[!Textbook]- 
><u>Chapter 8</u>: ![[Freund.pdf#page=239|Chapter 8]] 

# Point Estimation
>[!Textbook]- 
><u>Chapter 10</u>: ![[Freund.pdf#page=289|Chapter 10]] 

Point estimation concerns using a statistic to estimate a parameter of the distribution of some population. Commonly, we use the sample mean $\bar{X}$, though occasionally also sample standard deviation $s$. Notationally, $\theta$ the parameter to be estimated and $\hat{\theta}$ is the estimation

## Bias
An *unbiased estimator* is an estimator $\hat{\theta}$ of some parameter $\theta$ such that:
- $E[\hat{\theta}] = \theta$ 

We define any other estimator to be a biased estimator. A parameter may have multiple unbiased estimators.

## Efficiency
Efficiency is the variance of the estimator $\hat{\theta}$. 

We often consider relative efficiency, where we compare two estimators $\hat{\theta_{1}},\hat{\theta_{2}}$. We calculate the efficiency of $\hat{\theta_{1}}$ *relative to* $\hat{\theta_{2}}$ as:
- $\dfrac{\text{Var}(\hat{\theta_{2}})}{\text{Var}(\hat{\theta_{2}})}$

We are often interested in the minimum variance, or the maximally efficient, unbiased estimator $\hat{\theta}$ for some parameter. We then consider the Cramer-Rao bound:
- $\text{Var}(\hat{\theta}) \geq \dfrac{1}{n \cdot E\left[\left(\dfrac{\partial \ln f(X)}{\partial \theta}\right)^{2}\right]}$

If the left and right side are equal, then $\hat{\theta}$ is the minimum variance estimator of $\theta$. If $\hat{\theta}$ is also unbiased, then we say it is the minimum variance unbiased estimator. 

## Method of Moments
We can generate an estimators $\hat{\theta}$ for the parameters $\theta$ through calculating the moments of the sample, matching them accordingly to the parameters, then solving the system of equations. Commonly, we use the first moment $E[X]$ and second moment $E[X^{2}]$ and match them to the mean and variance of the population:
- $E[X] = \mu$
- $E[X^{2}] = \mu^{2} + \sigma^{2}$

## Method of Maximum Likelihood
We consider the likelihood function:
- $L(\theta) = f(x_{1}, x_{2},...,x_{n};\theta) = \prod\limits_{i=1}^{n}f(x_{i},\theta)$

Where we then maximize this function, solving for $\theta$ when:
- $L'{\theta} = 0$

Occasionally, this function may be hard to differentiate, so we also consider:
- $\dfrac{d \ln(L(\theta))}{d \theta} = 0$

# Interval Estimation
>[!Textbook]- 
><u>Chapter 11</u>: ![[Freund.pdf#page=323|Chapter 11]] 

# Hypothesis Testing
>[!Textbook]- 
><u>Chapter 12</u>: ![[Freund.pdf#page=343|Chapter 12]] 