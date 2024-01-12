---
tags: probability
title: Introdução à Estatística
#published: false
sidebar:
    nav: docs-en
---

## Estimador
Um estimador $\hat{\theta}$ de um parâmetro $\theta$ é uma função das observações da amostra

$$\hat{\theta}=\hat{\theta}\left(X_1, X_2, \ldots, X_n\right)$$

### Estimador não-viesado

$$E(\hat{\theta})=\theta$$

## Viés

$$\text{ Viés }(\theta)=E(\hat{\theta})-\theta$$

## Eficiência
Um estimador $\hat{\theta_1}$ é dito mais eficiente que $\hat{\theta_2}$ quando

$$\text{ Var }\left(\hat{\theta_1}\right)< \text{ Var }\left(\hat{\theta_2}\right)$$

## Consistência
Um estimador $\hat{\theta}$ é dito consistente quando, para todo $\epsilon>0$

$$\lim _{n \rightarrow \infty} text{ Pr }(|\hat{\theta}-\theta|>\epsilon)=0$$

## Erro Quadrático Médio (EQM)

$$\begin{gathered}
\text{ EQM }(T ; \theta)=E\left((T-\theta)^2\right) \\
\text{ EQM }(T ; \theta)=\text{Var}(T)+(\text{ Viés }(T))^2
\end{gathered}$$

## Estimador Consistente

Um estimador $\delta$ é dito consistente quando: $\delta_n \rightarrow \theta$, para $n \rightarrow \infty$
