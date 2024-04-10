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

Point estimation concerns using a statistic to estimate a parameter of the distribution of some population. Commonly, we use the sample mean $\bar{X}$, though occasionally also sample standard deviation $s$. Notationally, $\theta$ is the parameter to be estimated and $\hat{\theta}$ is the estimation

## Bias
An *unbiased estimator* is an estimator $\hat{\theta}$ of some parameter $\theta$ such that:
- $E[\hat{\theta}] = \theta$ 

We define any other estimator to be a biased estimator. A parameter may have multiple unbiased estimators.

## Efficiency
Efficiency is the variance of the estimator $\hat{\theta}$. 

We often consider relative efficiency, where we compare two estimators $\hat{\theta_{1}},\hat{\theta_{2}}$. We calculate the efficiency of $\hat{\theta_{1}}$ *relative to* $\hat{\theta_{2}}$ as:
- $\dfrac{\text{Var}(\hat{\theta_{2}})}{\text{Var}(\hat{\theta_{1}})}$

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

Interval estimation is a common method for estimation where we consider a range of values with some degree of confidence, as opposed to point estimation where we consider a single value. We consider:
- $P(\hat{\theta_{1}} < \theta < \hat{\theta_{2}}) = 1 - \alpha$

and denote the interval $\hat{\theta_{1}} < \theta < \hat{\theta_{2}}$ as the $100(1-\alpha)\%$ confidence interval. Commonly, the interval takes the form:
- $\left(\hat{\theta} - \epsilon, \hat{\theta} + \epsilon\right)$

For some calculated error value $\epsilon$. The majority of this content will be the various error values $\epsilon$

## Estimation of Means
The most common value to estimate is the mean of a population. We do this by transforming the sample mean $\bar{X}\sim N(\mu,\dfrac{\sigma^{2}}{n})$ to the standard normal $Z$. For a confidence interval of confidence $100(1-\alpha)\%$, we define our $\epsilon$ as:
- $\epsilon = Z_{\frac{\alpha}{2}}\dfrac{\sigma}{\sqrt{n}}$ 
And thus, the confidence interval as:
- $\left(\bar{X}-Z_{\frac{\alpha}{2}}\dfrac{\sigma}{\sqrt{n}},\bar{X}+Z_{\frac{\alpha}{2}}\dfrac{\sigma}{\sqrt{n}}\right)$ 
And a one-sided bound:
- $\left(\bar{X}\pm Z_{\alpha}\dfrac{\sigma}{\sqrt{n}}\right)$

We may also want to estimate the difference in two means $\bar{X_1},\bar{X_2}$, which is a trivial extension of the above concept. On most occasions (with population variance $\sigma^2$ given or sample variances $s_1^2,s_2^2$ given with sample sizes $n_1,n_2$ sufficiently large), we standardize through the form:
$Z = \dfrac{(\bar{X_{1}}-\bar{X_{2}})-(\mu_{1} -\mu_{2})}{\sqrt{\dfrac{\sigma_1^2}{n_1}+\dfrac{\sigma^2_2}{n_2}}}$
And thus derive the $100(1-\alpha)\%$ confidence interval as:
- $\left((\bar{X_1}-\bar{X_2})-Z_{\frac{\alpha}{2}}\sqrt{\dfrac{\sigma_1^2}{n_1}+\dfrac{\sigma^2_2}{n_2}},(\bar{X_1}-\bar{X_2})+Z_{\frac{\alpha}{2}}\sqrt{\dfrac{\sigma_1^2}{n_1}+\dfrac{\sigma^2_2}{n_2}}\right)$ 
And the one-sided bound as:
- $\left((\bar{X_1}-\bar{X_2})\pm Z_{\alpha}\sqrt{\dfrac{\sigma_1^2}{n_1}+\dfrac{\sigma^2_2}{n_2}}\right)$ 

However, we may not meet the above conditions always, and thus we use the t-distribution $t$ to construct a confidence interval, in the form:
- $\left((\bar{X_1}-\bar{X_2})-t_{\frac{\alpha}{2}}(n_1+n_2-2)\sqrt{\dfrac{(n_1-1)s_{1}^{2}+(n_2-1)s_{2}^{2}}{n_{1}+n_{2}-2}} \cdot\sqrt{\dfrac{1}{n_1}+\dfrac{1}{n_2}},(\bar{X_1}-\bar{X_2})+t_{\frac{\alpha}{2}}(n_1+n_2-2)\sqrt{\dfrac{(n_1-1)s_{1}^{2}+(n_2-1)s_{2}^{2}}{n_{1}+n_{2}-2}} \cdot\sqrt{\dfrac{1}{n_1}+\dfrac{1}{n_2}}\right)$ 
With the one-sided bound as:
- $\left((\bar{X_1}-\bar{X_2})\pm t_{\alpha}(n_1+n_2-2)\sqrt{\dfrac{(n_1-1)s_{1}^{2}+(n_2-1)s_{2}^{2}}{n_{1}+n_{2}-2}} \cdot\sqrt{\dfrac{1}{n_1}+\dfrac{1}{n_2}}\right)$ 
# Hypothesis Testing
 >[!Textbook]- 
><u>Chapter 12</u>: ![[Freund.pdf#page=343|Chapter 12]] 
