---
tags: statistics
title: Teste de Hipóteses
#published: false
sidebar:
    nav: docs-en
---

## Definição 

O teste de hipóteses uma metodologia estatística que nos auxilia a tomar decisões sobre uma ou mais populações baseado na informação obtida da amostra.

Nos permite verificar se os dados amostrais trazem evidência que apoiem ou não uma hipótese estatística formulada.

Ao tentarmos tomar decisões, é conveniente a formulação de suposições ou de conjeturas sobre as populações de interesse, que, em geral, consistem em considerações sobre parâmetros ($\mu$, $\sigma^2$, $p$) das mesmas.

Essas suposições, que podem ser ou não verdadeiras, são denominadas de Hipóteses Estatísticas.

Em muitas situações práticas o interesse do pesquisador é verificar a veracidade sobre um ou mais parâmetros populacionais ($\mu$, $\sigma^2$, $p$) ou sobre a distribuição de uma variável aleatória.

## Hipótese Nula e Alternativa

Vimos que no teste de hipóteses estatísticas, identificamos partições do espaço de parâmetros que codificam as hipóteses de interesse.
Agora, considere o espaço de parâmetros $\Omega$ e defina $\Omega_0, \Omega_1 \subset \Omega$ de modo que $\Omega_0 \cup \Omega_1=\Omega$ e $\Omega_0 \cap \Omega_1=\emptyset$. Definimos

$$\begin{aligned}
& H_0:=\theta \in \Omega_0, \\
& H_1:=\theta \in \Omega_1 .
\end{aligned}$$

Dizemos que $H_0$ é a hipótese nula e $H_1$ é a hipótese alternativa.
Se $\theta \in \Omega_1$, dizemos que rejeitamos a hipótese nula. Por outro lado, se $\theta \in \Omega_0$ dizemos que não rejeitamos ou falhamos em rejeitar $\mathrm{H}_0$.

### Exemplo

Suponha que Palmirinha recebeu uma carta da Associação Nacional da Pamonha Gourmet (ANPG), dizendo que a pamonha deve ter, no mínimo, $7 \mathrm{mg} / \mathrm{L} \mathrm{de}$ concentração de amido. Supondo que a concentração de amido tenha distribuição Normal com parâmetros $\mu$ (desconhecido) e $\sigma^2$ (conhecido), Palmirinha rabisca num papel:

$$\begin{aligned}
& H_0: \mu \in[7, \infty), \\
& H_1: \mu \in(0,7) .
\end{aligned}$$

## Hipóteses Simples e Compostas

Dizemos que uma hipótese $H_i$, é simples, se $\Omega_i=\left\{\theta_i\right\}$, isto é, se a partição correspondente é um ponto. Uma hipótese é dita composta se não é simples.

### Hipótese simples sobre a média

Suponha que estamos estudando o efeito de uma droga na redução da pressão arterial. Modelamos esta redução como uma variável aleatória $X$ com esperança $E[X]=: \theta$. É costumaz testar a hipótese $H_0: \theta=0$, que chamamos, especificamente nesse caso, de "hipótese de efeito nulo".

### Hipótese unilateral e bilateral

Uma hipótese da forma $H_0: \theta \leq \theta_0$ ou $H_0: \theta \geq \theta_0$ é dita unilateral ("one-sided"), enquanto hipóteses da forma $H_0: \theta \neq \theta_0$ são ditas bilaterais ("two-sided").

- Se $H_0$ é simples, a hipótese alternativa $H_1$ será, em geral, bilateral.
