---
tags: statistics
title: Teste não-viesado e Teste T
#published: false
sidebar:
    nav: docs-en
---

## Teste não-viesado

Suponha que desejamos testar a hipótese

$$\begin{aligned}
& H_0: \theta \in \Omega_0, \\
& H_1: \theta \in \Omega_1 
\end{aligned}$$

através do teste $\delta$. Dizemos que $\delta$ é não-viesado se (e somente se) para $\theta \in \Omega_0$ e $\theta^{\prime} \in \Omega_1$, vale

$$\pi(\theta \mid \delta) \leq \pi\left(\theta^{\prime} \mid \delta\right)$$

ou seja, se a função poder é pelo menos tão grande no espaço onde $H_0$ é falsa $\left(\Omega_1\right)$ quanto no espaço em que $H_0$ é verdadeira $\left(\Omega_0\right)$.

## Teste t

Um teste $\delta_c$ que rejeita $H_0$ se $U \geq c$ (equiv. $U \leq c$ ), com $c=T^{-1}\left(1-\alpha_0 ; n-1\right)$ é chamado um teste $t$ (unicaudal) de tamanho $\alpha_0$.

### Propriedades

Suponha que $\delta_c$ rejeita $H_0$ se $U \geq c$. Então

i) $\mu=\mu_0 \Longrightarrow \pi\left(\mu, \sigma^2 \mid \delta_c\right)=\alpha_0$ \
ii) $\mu<\mu_0 \Longrightarrow \pi\left(\mu, \sigma^2 \mid \delta_c\right)<\alpha_0$ \
iii) $\mu>\mu_0 \Longrightarrow \pi\left(\mu, \sigma^2 \mid \delta_c\right)>\alpha_0$ \
iv) $\lim _{\mu \rightarrow-\infty} \pi\left(\mu, \sigma^2 \mid \delta_c\right)=0$ \
v) $\lim _{\mu \rightarrow \infty} \pi\left(\mu, \sigma^2 \mid \delta_c\right)=1$ \
vi) $\delta_c$ é não-viesado e tem tamanho $\alpha_0$.
