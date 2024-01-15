---
tags: statistics
title: Distribuições Discretas e Contínuas
#published: false
sidebar:
    nav: docs-en
---

## Distribuição Uniforme

$$\begin{gathered}
f\left(x \mid \theta_1, \theta_2\right)=\frac{1}{\theta_2-\theta_1}, \theta_2>\theta_1 \\
E[x]=\frac{a+b}{2} \\
\text{Var}[x]=\frac{(b-a)^2}{12} \\
f_n\left(x \mid \theta_1, \theta_2\right)=\frac{1}{\left(\theta_2-\theta_1\right)^n}
\end{gathered}$$

## Distribuição Binomial

k = número de sucessos

$$\begin{gathered}
f(x \mid \theta, k)=\left(\begin{array}{c}
n \\
k
\end{array}\right) \theta^k(1-\theta)^{n-k} \\
E[x]=p \leftrightarrow \theta \\
E\left[x^2\right]=n^2 p^2+n p(1-p) \leftrightarrow n^2 \theta^2+n \theta(1-\theta) \\
\text{Var}[x]=n p(1-p) \leftrightarrow n \theta(1-\theta) \\
f_n(x \mid \theta)=\prod_{i=1}^n\left(\begin{array}{c}
n \\
x_i
\end{array}\right) \theta^y(1-\theta)^{n-y}, y=\sum_1^n x_i
\end{gathered}$$

## Distribuição Geométrica
$k=$ fracasso

$$\begin{gathered}
f(x \mid \theta)=(1-\theta)^3 \theta \\
E[x]=\frac{1-p}{p} \leftrightarrow \frac{1-\theta}{\theta} \\
\text{Var}[x]=\frac{1-p}{p^2} \leftrightarrow \frac{1-\theta}{\theta^2}
\end{gathered}$$

## Distribuição de Bernoulli

$$\begin{gathered}
f(x \theta)-\theta^x(1-\theta)^{1-x}, x \in\{0,1\} \\
E[x]-p \leftrightarrow \theta \\
\text{Var}[x]=p(1-p) \leftrightarrow \theta(1-\theta) \\
f_n(x \mid \theta)=\theta^y(1-\theta)^{n-y}, y=\sum_1^n x_i
\end{gathered}$$

## Distribuição Exponencial

$$\begin{gathered}
f(x \mid \theta)=\theta e^{-\theta z}, \theta>0, x>0 \\
E[x]=\frac{1}{\lambda} \leftrightarrow \frac{1}{\theta} \\
V a r|x|=\frac{1}{p^2} \leftrightarrow \frac{1}{\theta^2} \\
f_n(x \mid \theta)=\theta^n e^{-\theta y}, y=\sum_1^n x_i
\end{gathered}$$

## Distribuição de Poisson

$$\begin{gathered}
f(x \theta)=\frac{e^{-\theta} \theta^x}{x !}, \theta>0 \\
E[x]-\lambda \leftrightarrow \theta \\
\text{Var}[x-\lambda \leftrightarrow \theta \\
f_n(x \mid \theta)=\frac{e^{-r \theta} \theta^y}{\prod x_{i} !}, y=\sum_1^n x_i
\end{gathered}$$

## Distribuiçăo $\text{Normal}\left(\mu, \sigma^2\right)$

$$\begin{gathered}
\int\left(x \mid \mu, \sigma^2\right)=\frac{1}{\sigma \sqrt{2 \pi}} e^{-\frac{i s-\left.\mu\right|^2}{s r^2}} \\
E[x]=\mu \\
\text{Var}(x)=\sigma^2
\end{gathered}$$

$$Z=\frac{X \quad \mu}{\sigma}$$

$Z \sim(0,1)$

$$\text{Pr}(Z \leq c)=\Phi(c)$$

### Propriedade

Seja $X_1, X_2, \ldots X_i$ i.i.d onde $X_i \sim\left(\mu, \sigma^2\right)$, entāo $X_n=\frac{1}{n} \sum_{i=1}^n X_i$ tem distribuiçäo:

$$\begin{gathered}
E\left(\frac{1}{n} \sum_{i=1}^n X_i\right)-\sum_{i=1}^n \frac{1}{n} E\left(X_i\right)=n \frac{1}{n} \mu-\mu \\
\text{Var}\left(\sum_{i=1}^n \frac{1}{n} X_i\right)=\sum_{i=1}^n\left(\frac{1}{n}\right)^2 \text{Var}\left(X_i\right)=\sum_{i=1}^n\left(\frac{1}{n}\right)^2 \sigma^2=n\left(\frac{1}{n}\right)^2 \sigma^2=\frac{\sigma^2}{n} \\
\bar{X}_n \sim\left(\mu, \frac{\sigma^2}{n}\right)
\end{gathered}$$

## Distribuição $\text{Gamma}(\alpha, \beta)$

$$\begin{gathered}
f(x \mid \alpha, \beta)=\frac{\beta^\alpha}{\Gamma(\alpha)} x^{\alpha x-1} e^{-\beta x}, x>0 \\
\xi(\theta) \propto \theta^\alpha \text { । }_e \omega \\
E x]=\text { média }=\frac{\alpha}{\beta}
\end{gathered}$$

## Distribuição Gamma-Inversa $(\alpha, \beta)$

$$f(x \mid \alpha, \beta)=\frac{\beta^\alpha}{\Gamma(\alpha)} x^{-\alpha-1} e^{-\frac{\rho}{\alpha}}$$

## Distribuição $\text{Beta}\left(\alpha_t \beta\right)$

$$\begin{gathered}
f(x \mid \alpha, \beta)-\frac{\Gamma(\alpha+\beta)}{\Gamma(\alpha) \Gamma(\beta)} x^{\alpha-1}(1-x)^{\beta-1}: 0<x<1 \\
\xi(\theta) \propto \theta^{\alpha 1}(1-\theta)^{\sigma / 1} \\
E[x]=\text { media }=\frac{\alpha}{\alpha+\beta}
\end{gathered}$$
