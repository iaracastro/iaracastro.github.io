---
tags: statistics
title: Informação de Fisher
#published: false
sidebar:
    nav: docs-en
---

# Informação de Fisher : $I(\theta)$

$$l(x \mid \theta)=\log f(x \mid \theta)$$

$f(x \mid \theta)$ é diferenciável em $\theta$ :

$$\begin{aligned}
l^{\prime}(x \mid \theta) & =\frac{\partial l(x \mid \theta)}{\partial \theta} \\
l^{\prime \prime}(x \mid \theta) & =\frac{\partial^2 l(x \mid \theta)}{\partial \theta^2}
\end{aligned}$$

## Fórmula da informação de Fisher:

$$I_n(\theta)=E_\theta\left[l^{\prime}(x \mid \theta)^2\right]=-E_\theta\left[l^{\prime \prime}(x \mid \theta)\right]=\operatorname{Var}_\theta\left(l^{\prime}(x \mid \theta)\right)$$

- Lembrete: A informação de Fisher sempre é positiva.

Seja $X_1, X_2, \ldots, X_n$ uma amostra aleatória e seja $I_n(\theta)=-E_\theta\left[l^{\prime \prime}(x \mid \theta)\right]$, então:

$$I_n(\theta)=n I(\theta)$$

$I(\theta)$ é a informação de Fisher aplicada em apenas uma observação, então usa: $f(x \mid \theta)$. $I_n(\theta)$ é a informação de Fisher aplicada para várias observações, então usa: $f_n(x \mid \theta)$.

## Exemplos

### Bernoulli

$$\frac{1}{p(1-p)} \leftrightarrow \frac{1}{\theta(1-\theta)}$$

#### Prova

$$\begin{gathered}
f(x \mid \theta)=\theta^x(1-\theta)^{1-x}, x=1 \text { ou } x=0 \\
l(x \mid \theta)=\log f(x \mid \theta)=x \log (\theta)+(1-x) \log (1-\theta) \\
l^{\prime}(x \mid \theta)=\frac{x}{\theta}-\frac{1-x}{1-\theta} \\
l^{\prime \prime}(x \mid \theta)=-\frac{x}{\theta^2}-\frac{1-x}{(1-\theta)^2}
\end{gathered}$$

Sabemos que $E[x]=\theta$, então:

$$\begin{gathered}
I(\theta)=-E_\theta\left[\lambda^{\prime \prime}(x \mid \theta)\right]=\frac{E[x]}{\theta^2}+\frac{1-E[x]}{(1-\theta)^2} \\
I(\theta)=\frac{\theta}{\theta^2}+\frac{1-\theta}{(1-\theta)^2}=\frac{1}{\theta}+\frac{1}{1-\theta}=\frac{1-\theta+\theta}{\theta(1-\theta)}=\frac{1}{\theta(1-\theta)}
\end{gathered}$$

### Binomial

$$\frac{n}{p(1-p)} \leftrightarrow \frac{1}{\theta(1-\theta)}$$

#### Prova

$$\begin{gathered}
f_n(x \mid \theta)=\prod_{i=1}^n\left(\begin{array}{c}
n \\
x_i
\end{array}\right) \theta^y(1-\theta)^{n-y}, y=\sum_1^n x_i \\
l(x \mid \theta)=\log f(x \mid \theta)=\sum_{i=1}^n \log \left(\left(\begin{array}{c}
n \\
x_i
\end{array}\right)\right)+y \log (\theta)+(n-\theta) \log (1-\theta) \\
l^{\prime}(x \mid \theta)=\frac{y}{\theta}-(n-y) \frac{1}{1-\theta} \\
l^{\prime \prime}(x \mid \theta)=-\frac{y}{\theta^2}-\frac{n-y}{(1-\theta)^2} \\
I_n(\theta)=-E_\theta\left[\lambda^{\prime \prime}(x \mid \theta)\right]=\frac{E[y]}{\theta^2}+\frac{1}{(1-\theta)^2} E[n-y] \\
I_n(\theta)=\frac{n \theta}{\theta^2}+\frac{n-n \theta}{(1-\theta)^2}=\frac{n \theta(1-\theta)^2+(n-n \theta) \theta^2}{\theta^2(1-\theta)^2} \\
I_n(\theta)=\frac{n \theta-2 \theta^2+\not \not \theta^\zeta+n \theta^2-\not n \theta^5}{\theta^2(1-\theta)^2}=\frac{n \not \theta^{\prime}(1-\theta)}{\theta^{\prime \prime}(1-\theta)^{\not \prime}} \\
I_n(\theta)=\frac{n}{\theta(1-\theta)} \leftrightarrow I(\theta)=\frac{1}{\theta(1-\theta)}
\end{gathered}$$

### Exponencial

$$\frac{1}{\lambda^2} \leftrightarrow \frac{1}{\theta^2}$$

Prova:

$$\begin{gathered}
f(x \mid \theta)=\theta e^{-\theta x}, \theta>0, x>0 \\
l(x \mid \theta)=\log f(x \mid \theta)=\log (\theta)-\theta x \\
l^{\prime}(x \mid \theta)=\frac{1}{\theta}-x \\
l^{\prime \prime}(x \mid \theta)=-\frac{1}{\theta^2}
\end{gathered}$$

Sabemos que $E[x]=\frac{1}{\theta}$, mas a função já independe de $\mathrm{x}$ então:

$$I(\theta)=-E_\theta\left[\lambda^{\prime \prime}(x \mid \theta)\right]=-\left(-\frac{1}{\theta^2}\right)=\frac{1}{\theta^2}$$

### Poisson

$$\frac{1}{\lambda} \leftrightarrow \frac{1}{\theta}$$

#### Prova

$$\begin{gathered}
f_n(\bar{x} \mid \theta)=\frac{e^{-n \theta} \theta^y}{\prod x_{i} !}, y=\sum_1^n x_i,, \theta>0 \\
l(x \mid \theta)=\log f_n(x \mid \theta)=y \log (\theta)-n \theta-\log \left(\prod x_{i} !\right) \\
l^{\prime}(x \mid \theta)=-n+\frac{y}{\theta} \\
l^{\prime \prime}(x \mid \theta)=\frac{-y}{\theta^2}
\end{gathered}$$

$$I_n(\theta)=-E_\theta\left[\lambda^{\prime \prime}(x \mid \theta)\right]=\frac{1}{\theta^2} E\left[\sum_1^n x_i\right]$$

Sabemos que $E[x]=\theta$, então:

$$I_n(\theta)=\frac{1}{\theta^2} n \theta=\frac{n}{\theta} \leftrightarrow I(\theta)=\frac{1}{\theta}$$

### Normal
$\mu$ desconhecido e $\sigma^2$ é dado

$$I(\mu)=E\left[I^{\prime \prime}(x \mid \mu)\right]=\frac{1}{\sigma^2}$$

#### Prova

$$\begin{gathered}
l(x \mid \mu)=\log f(x \mid \theta)=-\frac{1}{2} \log \left(2 \pi \sigma^2\right)-\frac{(x-\mu)^2}{2 \sigma^2} \\
l^{\prime}(x \mid \mu)=\frac{x-\mu}{\sigma^2} \\
l^{\prime \prime}(x \mid \mu)=-\frac{1}{\sigma^2}
\end{gathered}$$

Sabemos que $E[x]=\mu$, mas já é idependente de $\mu$ então basta trocar o sinal:

$$I(\theta)=-E_\theta\left[\lambda^{\prime \prime}(x \mid \theta)\right]=\frac{1}{\sigma^2}$$
