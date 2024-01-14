---
tags: statistics
title: Intervalo de Confiança
#published: false
sidebar:
    nav: docs-en
---

## Definição

De acordo com a interpretação frequentista, um intervalo de confiança para um determinado parâmetro da população mostra um intervalo de valores do verdadeiro parâmetro da população compatíveis com os dados da amostra, com um certo nível de confiança, seja o parãmetro a média de uma determinada distribuição, o risco relativo, a razão de chances, a variância, etc. O cálculo do intervalo de confiança é um dos principais resultados de uma análise estatística

Suponha que $z_p$ significa o valor da variável aleatória $\mathbf{Z}$ que segue a distribuição normal padrão, $N(0,1)$, para o qual $P\left(z \leq z_p \right)=p$, ou seja, a área sob a curva normal padrão à esquerda de $z_p$ é igual a $p$. Assim, para $p=0,01(1 \%), z_{0,01}=-2,33$. 

<div style="float:middle; margin:2em;">
    <img src="https://raw.githubusercontent.com/iaracastro/iaracastro.github.io/master/images/distribuicao-normal-padrao.png"/>
</div>

Para uma população com uma distribuição normal padrão, dado um valor $\alpha(0 \leq \alpha \leq 1)$, podemos obter ० intervalo $\left(z_{\alpha / 2}, z_{1-\alpha / 2}\right)$ que conterá com probabilidade $(1-\alpha)$ o valor de um elemento extraído aleatoriamente dessa população. Para a distribuição normal padrão, $z_{\alpha / 2}=-z_{1-\alpha / 2}$.

### Uma distribuição normal genérica $\sim(\mu, \sigma)$

Podemos mapear áreas sob o gráfico de uma distribuição normal genérica com média $\mu$ e desvio padrão $\sigma$ para áreas sob o gráfico da distribuição normal padrão por meio da expressão:
$$Z=\frac{X-\mu}{\sigma}$$

Assim o intervalo $z_{\alpha / 2} \leq Z \leq z_{1-\alpha / 2}$ irá ser mapeado para o intervalo
$$\begin{gathered}
z_{\alpha / 2} \leq \frac{X-\mu}{\sigma} \leq z_{1-\alpha / 2} \\
\mu+z_{\alpha / 2} \sigma \leq X \leq \mu+z_{1-\alpha / 2} \sigma \Rightarrow \mu-z_{1-\alpha / 2} \sigma \leq X \leq \mu+z_{1-\alpha / 2} \sigma
\end{gathered}$$

Portanto a probabilidade de extrairmos um elemento da população com distribuição $N\left(\mu, \sigma^2\right)$ e o valor desse elemento pertencer ao intervalo $\left[\mu-z_{1-\alpha / 2} \sigma, \mu+z_{1-\alpha / 2} \sigma\right]$ é $(1-\alpha) \%$.

## Intervalos de Confiança em Testes de Hipótese

| Definição |
| --- |
| Suponha que dispomos de dados $\boldsymbol{X}=\{X_1, X_2, \ldots, X_n\}$ com f.d.p. comum $f(x \mid \theta)$, e estamos interessados em testar as hipóteses:
$$\begin{aligned}
& H_0: g(\theta)=g_0, \\
& H_1: g(\theta) \neq g_0,
\end{aligned}$$
de modo que existe um teste $\delta_{g_0}$ com nível $\alpha_0$ destas hipóteses. Para cada $\boldsymbol{X}=\boldsymbol{x}$, defina
$$w(\boldsymbol{x})=\left\{g_0: \delta_{g_0} \text { não rejeita } H_0 \text { dado que } \boldsymbol{X}=\boldsymbol{x}\right\} .$$
Fazendo o nível de confiança do intervalo $\gamma=1-\alpha_0$, temos
$$\operatorname{Pr}\left(g\left(\theta_0\right) \in w(\boldsymbol{X}) \mid \theta=\theta_0\right) \geq \gamma, \forall \theta_0 \in \Omega$$ |

## Interpretação do Intervalo de Confiança

O intervalo de confiança $(100-\alpha) \%$ para um parâmetro consiste em um intervalo aleatório que possui a propriedade de conter o valor real desse parâmetro com uma probabilidade de $(100-\alpha) \%$. O termo aleatório nessa interpretação indica que, antes de realizarmos a amostragem e calcularmos o intervalo de confiança de acordo com o procedimento apropriado, haverá uma probabilidade de $(100-\alpha) \%$ de o intervalo vir a conter o real valor do parâmetro de interesse.

### Observações 

- Um intervalo de confiança não é uma afirmação sobre o(s) parâmetro(s)!
A afirmação probabilística da forma $\operatorname{Pr}\{A(\boldsymbol{X})<g(\theta)<B(\boldsymbol{X})\}=\gamma$ diz respeito à distribuição conjunta das variáveis aleatórias $A(\boldsymbol{X})$ e $B(\boldsymbol{X})$ para um valor fixo de $\theta$ - e, portanto, de $g(\theta)$.

- Intervalos de confiança são procedimentos

Como de costume na teoria ortodoxa (frequentista), o foco da construção de um intervalo confiança está em dar garantias probabilísticas com relação à distribuição dos dados. Dizer que $\operatorname{Pr}\{A(\boldsymbol{X})<g(\theta)<B(\boldsymbol{X})\}=\gamma$ é dizer que, se eu gerasse $M$ grande amostras aleatórias $\boldsymbol{X}^{(1)}, \boldsymbol{X}^{(2)}, \ldots, \boldsymbol{X}^{(M)}$ de tamanho $n$ e construisse $M$ intervalos $I\left(\boldsymbol{X}^{(1)}\right), I\left(\boldsymbol{X}^{(2)}\right), \ldots, I\left(\boldsymbol{X}^{(M)}\right)$, eu esperaria encontrar:

$$\frac{1}{M} \sum_{i=1}^M \mathbb{I}\left(g(\theta) \in I\left(\boldsymbol{X}^{(i)}\right)\right) \approx \gamma$$
