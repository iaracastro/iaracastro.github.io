---
tags: statistics
title: Teste da razão da verossimilhança e Teorema de Wilks
#published: false
sidebar:
    nav: docs-en
---

## Teste da razão da verossimilhança

Considere testar

$$\begin{aligned}
& H_0: \theta \in \Omega_0, \\
& H_1: \theta \in \Omega_1 
\end{aligned}$$

Em certas situações, podemos utilizar a função de verossimilhança para quantificar a evidência em favor de $H_0$.

### Definição

A estatística

$$\Lambda(x)=\frac{\sup _{\theta \in \Omega_0} f_n(x \mid \theta)}{\sup _{\theta \in \Omega} f_n(x \mid \theta)}$$

é chamada uma estatística de razão de verossimilhanças. Um um teste de razão de verossimilhanças, $\delta_k$ é um teste que rejeita $H_0$ se $\Lambda(x) \leq k$ para uma constante $k$.

## Teorema de Wilks

O teorema de Wilks afirma que a razão log-verossimilhança é assintoticamente normal. Isto pode ser usado para produzir intervalos de confiança para estimativas de máxima verossimilhança ou como uma estatística de teste para realizar o teste de razão de verossimilhança.

Suponha que temos um espaço de parâmetros com $k$ coordenadas, $\theta=\left(\theta_1, \theta_2, \ldots, \theta_k\right)$ e desejamos testar a hipótese (simples) da forma

$$\begin{aligned}
& H_0: \theta_j=\theta_0^j, \; j=1,2, \ldots, k, \\
& H_1: \theta_j \neq \theta_0^j, \;  j=1,2, \ldots, k .
\end{aligned}$$

Então, sob condições de regularidade, temos que, à medida que $n \rightarrow \infty$,

$$-2 \log \Lambda(x) \stackrel{d}{\rightarrow} \chi^2(k)$$
