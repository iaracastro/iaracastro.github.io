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

$$\operatorname{Viés}(\theta)=E(\hat{\theta})-\theta$$

## Eficiência
Um estimador $\hat{\theta_1}$ é dito mais eficiente que $\hat{\theta_2}$ quando

$$\operatorname{Var}\left(\hat{\theta_1}\right)<\operatorname{Var}\left(\hat{\theta_2}\right)$$

## Consistência
Um estimador $\hat{\theta}$ é dito consistente quando, para todo $\epsilon>0$

$$\lim _{n \rightarrow \infty} \operatorname{Pr}(|\hat{\theta}-\theta|>\epsilon)=0$$

##Erro Quadrático Médio (EQM)

$$\begin{gathered}
\operatorname{EQM}(T ; \theta)=E\left((T-\theta)^2\right) \\
\operatorname{EQM}(T ; \theta)=\operatorname{Var}(T)+(\operatorname{Viés}(T))^2
\end{gathered}$$
