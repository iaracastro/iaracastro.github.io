---
tags: statistics
title: Cramer-Ráo e Eficiência de um estimador
#published: false
sidebar:
    nav: docs-en
---

## Cramer-Ráo e Eficiência

O limite de Cramér-Rao afirma que o inverso da informação de Fisher é um limite inferior na variância de qualquer estimador não enviesado de $\theta$. $(\hat{\theta})$

### Information Inequality

$$\text{Var}_\theta(\delta) \geq \frac{\left[m^{\prime}(\theta)\right]^2}{n I(\theta)}$$

$$m(\theta)=E_\theta[\hat{\theta}]$$

Definição: Um estimador é dito eficiente se ele atinge a cota de Cramer-Ráo.

$$\text{Var}_\theta(\delta)=\frac{\left[m^{\prime}(\theta)\right]^2}{n I(\theta)}$$

Exemplo: Seja $X_1, X_2, \ldots, X_n$ uma amostra aleatória de uma distribuição de Poisson, $\overline{x_n}$ é um estimador eficiente de $\theta$.

- Se $\hat{\theta}$ é um estimador não-viesado, então $m(\theta)=\theta \leftrightarrow m^{\prime}(\theta)=1$

$$\text{Var}_\theta(\delta) \geq \frac{1}{n I(\theta)}$$

## Distribuição Assintótica

Propriedades assintóticas são aquelas válidas apenas para grandes amostras, ou para amostras com tamanho $n \rightarrow \infty$. A distribuição amostral de um estimador é diferente para tamanhos de amostras diferentes. A distribuição da média amostral para amostras de qualquer população é definida pelo Teorema do Limite Central (TCL).

O Teorema nos garante que quando o tamanho da amostra cresce, a distribuição assintótica será aproximadamente normal. Então, para qualquer que seja a distribuição que tenha gerado os dados amostrais, sabemos que o estimador convergirá para a distribuição normal, sendo esta a distribuição assintótica do estimador.

Definição: $\hat{\theta}$ é um estimador assintoticamente não viesado de $\theta$ se $\lim _{n \rightarrow \infty} E(\hat{\theta})=\theta$.
