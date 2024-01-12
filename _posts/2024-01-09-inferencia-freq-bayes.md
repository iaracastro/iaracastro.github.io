---
tags: probability
title: Inferência Frequentista e Bayesiana
#published: false
sidebar:
    nav: docs-en
---

## Inferência Frequentista

Em uma abordagem frequencista à inferência, parâmetros desconhecidos são frequentemente, mas nem sempre tratados como se tivessem valores fixos, mas desconhecidos que não podem ser tratados como variados aleatórios em qualquer sentido e assim não há como associar probabilidades a eles. O modo frequentista de encarar a inferência faz uso apenas das informações presentes na amostra para inferir as características da população de interesse. Deste modo, os estimadores construídos sob esse modelo utilizam apenas as informações observadas na amostra, sem utilizar informações anteriores ao experimento.

## Inferência Bayesiana

A inferência bayesiana é um ramo muito recente da estatística inferencial, e tem suas ideias baseadas no teorema proposto por Thomas Bayes (1702 – 1761), onde considera uma inserção de um conhecimento à priori, ou seja, um conhecimento anterior à pesquisa. Trata tudo como variável aleatória:

$$\xi(\theta \mid \bar{x})=\frac{\xi(\theta) f_n(\bar{x} \mid \theta)}{f(\bar{x})}=\frac{\xi(\theta) \prod_{i=1}^n f\left(x_i \mid \theta\right)}{\int \xi(\theta) \prod_{i=1}^n f\left(x_i \mid \theta\right) d \theta}, \bar{x}\left(x_1, x_2, \ldots, x_n\right)$$

Com variáveis discretas:

$$\xi(\theta \mid \bar{x})=\frac{\xi(\theta) f_n(\bar{x} \mid \theta)}{\sum_\theta \xi(\theta) \prod_i f_n(\bar{x} \mid \theta)}$$
