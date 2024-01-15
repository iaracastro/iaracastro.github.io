---
tags: statistics
title: Função Poder, Tipos de Erro e Tamanho do Teste
#published: false
sidebar:
    nav: docs-en
---

## Função Poder

Nossa capacidade de rejeitar $H_0$ depende do valor de $\theta \in \Omega$. Esta dependência é capturada pela função poder.

Seja $\delta$ um procedimento de aceitação/rejeição como visto anteriormente. A função poder é definida como
$$\pi(\theta \mid \delta):=\text{Pr}\left(\boldsymbol{X} \in S_1 \mid \theta\right)=\text{Pr}(T \in R \mid \theta), \theta \in \Omega$$

Idealmente, queremos $\pi(\theta \mid \delta)=1$ para $\theta \in \Omega_1$.

### Função Poder para a média da Normal

Considere a situação em que $X_1, X_2, \ldots, X_n$ vêm de uma Normal com média $\mu$, desconhecida, e variância $\sigma^2$, conhecida.

- $\sigma^2$ conhecida

Lembrando que $T= |\bar{X}_n-\mu_0 |$, e tomando $\delta$ como o procedimento descrito acima, escrevemos

$$\begin{aligned}
\pi(\mu \mid \delta) & =\text{Pr}(T \in R \mid \mu) \\
& =\text{Pr}\left(\bar{X}_n \geq \mu_0+c \mid \mu\right)+\text{Pr}\left(\bar{X}_n \leq \mu_0-c \mid \mu\right) \\
& =\left\{1-\Phi\left(\sqrt{n} \frac{\mu_0+c-\mu}{\sigma}\right)\right\}+\Phi\left(\sqrt{n} \frac{\mu_0-c-\mu}{\sigma}\right) .
\end{aligned}$$

## Tipos de Erro

Quando testamos uma hipótese, nunca estamos livres de cometer um erro. É conveniente classificar os possíveis erros em duas categorias.

| Nome | Erro cometido |
| --- | --- |
| Erro tipo I | Rejeitar $H_0$ quando ela é verdadeira. |
| Erro tipo II | Falhar em rejeitar $H_0$ quando ela é falsa. |


Isto nos leva a concluir que

| Situação | Quantidade | Interpretação |
| --- | --- | --- |
| $\theta \in \Omega_0$ | $\pi(\theta \mid \delta)$ | $\text{Pr}($ Erro tipo I) |
| $\theta \in \Omega_1$ | $1-\pi(\theta \mid \delta)$ | $\text{Pr}($ Erro tipo II $)$ |

- Diminuir o erro do Tipo I implica em aumentar o erro do tipo II

Para haver um equilíbrio, tome $0<\alpha_0 < 1 $. E construa o procedimento $\delta^*$ de modo que

  $$\pi\left(\theta \mid \delta^*\right) \leq \alpha_0, \forall \theta \in \Omega$$

Buscamos o teste que tenha $\pi\left(\theta \mid \delta^*\right)$ máxima em $\theta \in \Omega_1$.

## Tamanho do Teste

Dizemos que um teste, $\delta$, tem tamanho ou nível de significância $\alpha(\delta)$, com

$$alpha(\delta):=\sup _{\theta \in \Omega_0} \pi(\theta \mid \delta)$$

### Tamanho de um teste com $H_0$ simples
  
Se $H_0$ é simples, então $\alpha(\delta)=\pi\left(\theta_0 \mid \delta\right)$

### Construindo um teste de tamanho $\alpha_0$
Se $T=r(X)$ é uma estatística, podemos quase sempre encontrar c tal que valha

$$\sup _{\theta \in \Omega_0} \text{Pr}(T \geq c \mid \theta) \leq \alpha_0$$

ou seja, encontrar c tal que $\delta$ tenha tamanho (ou nível de significância) $\alpha_0$.

