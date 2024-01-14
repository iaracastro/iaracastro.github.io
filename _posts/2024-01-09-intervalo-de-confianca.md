---
tags: statistics
title: Intervalo de Confiança
#published: false
sidebar:
    nav: docs-en
---

## Definição

De acordo com a interpretação frequentista, um intervalo de confiança para um determinado parâmetro da população mostra um intervalo de valores do verdadeiro parâmetro da população compatíveis com os dados da amostra, com um certo nível de confiança, seja o parãmetro a média de uma determinada distribuição, o risco relativo, a razão de chances, a variância, etc. O cálculo do intervalo de confiança é um dos principais resultados de uma análise estatística.

Seja $X=\left\{X_1, X_2, \ldots, X_n\right\}$ uma amostra aleatória, cada variável aleatória com p.d.f. $f(x \mid \theta)$, e considere uma função real $g(\theta)$. Sejam $A(X)$ e $B(X)$ duas estatísticas de modo que valha
$$\text{Pr}\{A(X)<g(\theta)<B(X)\} \geq \gamma$$

Dizemos que $I(X)=(A(X), B(X))$ é um intervalo de confiança de $100 \gamma \%$ para $g(\theta)$. Se a desigualdade for uma igualdade para todo $\theta \in \Omega$, dizemos que o intervalo é exato.

### Intervalo de confiança para a média no caso Normal

Lembremos que
$$U=\frac{\sqrt{n}\left(\bar{X}_n-\mu\right)}{\sqrt{\frac{\Delta^2}{n-1}}} \sim T(n-1) .$$

Para $c>0$, podemos computar $text{Pr}(-c<U<c)=\gamma$ :
$$\begin{aligned}
& text{Pr}\left(-c<\frac{\sqrt{n}\left(\bar{X}_n-\mu\right)}{\sqrt{\frac{\Delta^2}{n-1}}}<c\right)=\gamma, \\
& text{Pr}\left(\bar{X}_n-\frac{c \hat{\sigma}^{\prime}}{\sqrt{n}}<\mu<\bar{X}_n+\frac{c \hat{\sigma}^{\prime}}{\sqrt{n}}\right)=\gamma, \\
& T_{n-1}(c)-T_{n-1}(-c)=2 T_{n-1}(c)-1=\gamma .
\end{aligned}$$

Concluímos que $c=F_T^{-1}\left(\frac{1+\gamma}{2} ; n-1\right)$.

No caso do intervalo de confiança para o parâmetro de média, temos

$$text{Pr}\{A(\boldsymbol{X})<g(\mu)<B(\boldsymbol{X})\} \geq \gamma,$$
$text{com} g(\mu)=\mu \mathrm{e}$
$$\begin{aligned}
& A(\boldsymbol{X})=\bar{X}_n-\frac{c \hat{\sigma}^{\prime}}{\sqrt{n}}=\bar{X}_n-\frac{c \sqrt{\sum_{i=1}^n\left(X_i-\bar{X}_n\right)^2}}{\sqrt{n(n-1)}}, \\
& B(\boldsymbol{X})=\bar{X}_n+\frac{c \hat{\sigma}^{\prime}}{\sqrt{n}}=\bar{X}_n+\frac{c \sqrt{\sum_{i=1}^n\left(X_i-\bar{X}_n\right)^2}}{\sqrt{n(n-1)}} .
\end{aligned}$$

### Mapeando uma distribuição normal genérica $\sim(\mu, \sigma)$ para uma distribuição normal padrão $\sim(0,1)$

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
$$H_0: g(\theta)=g_0$$
$$H_1: g(\theta) \neq g_0$$
de modo que existe um teste $\delta_{g_0}$ com nível $\alpha_0$ destas hipóteses. Para cada $\boldsymbol{X}=\boldsymbol{x}$, defina
$$w(\boldsymbol{x})=\{g_0: \delta_{g_0} \text { não rejeita } H_0 \text { dado que } \boldsymbol{X}=\boldsymbol{x}\} .$$
Fazendo o nível de confiança do intervalo $\gamma=1-\alpha_0$, temos
$$\text{Pr}\left(g\left(\theta_0\right) \in w(\boldsymbol{X}) \mid \theta=\theta_0\right) \geq \gamma, \forall \theta_0 \in \Omega$$ |

### Interpretação do Gráfico

Suponha que $z_p$ significa o valor da variável aleatória $\mathbf{Z}$ que segue a distribuição normal padrão, $N(0,1)$, para o qual $P\left(z \leq z_p \right)=p$, ou seja, a área sob a curva normal padrão à esquerda de $z_p$ é igual a $p$. Assim, para $p=0,01(1 \%), z_{0,01}=-2,33$. 

<div style="float:middle; margin:2em;">
    <img src="https://raw.githubusercontent.com/iaracastro/iaracastro.github.io/master/images/distribuicao-normal-padrao.png"/>
</div>

Para uma população com uma distribuição normal padrão, dado um valor $\alpha(0 \leq \alpha \leq 1)$, podemos obter ० intervalo $\left(z_{\alpha / 2}, z_{1-\alpha / 2}\right)$ que conterá com probabilidade $(1-\alpha)$ o valor de um elemento extraído aleatoriamente dessa população. Para a distribuição normal padrão, $z_{\alpha / 2}=-z_{1-\alpha / 2}$.

## Interpretação do Intervalo de Confiança

O intervalo de confiança $(100-\alpha) \%$ para um parâmetro consiste em um intervalo aleatório que possui a propriedade de conter o valor real desse parâmetro com uma probabilidade de $(100-\alpha) \%$. O termo aleatório nessa interpretação indica que, antes de realizarmos a amostragem e calcularmos o intervalo de confiança de acordo com o procedimento apropriado, haverá uma probabilidade de $(100-\alpha) \%$ de o intervalo vir a conter o real valor do parâmetro de interesse.

### Observações 

- Um intervalo de confiança não é uma afirmação sobre o(s) parâmetro(s)!
A afirmação probabilística da forma $\text{Pr} \{ A(X) < g(\theta) < B(X) \} = \gamma$ diz respeito à distribuição conjunta das variáveis aleatórias $A(X)$ e $B(X)$ para um valor fixo de $\theta$ - e, portanto, de $g(\theta)$.

- Intervalos de confiança são procedimentos

Como de costume na teoria ortodoxa (frequentista), o foco da construção de um intervalo confiança está em dar garantias probabilísticas com relação à distribuição dos dados. Dizer que $\text{Pr}\{A(X) < g(\theta) < B(X)\}=\gamma$ é dizer que, se eu gerasse $M$ grande amostras aleatórias $X^{(1)}, X^{(2)}, \ldots, X^{(M)}$ de tamanho $n$ e construisse $M$ intervalos $I\left(X^{(1)}\right), I\left(X^{(2)}\right), \ldots, I\left(X^{(M)}\right)$, eu esperaria encontrar:

$$\frac{1}{M} \sum_{i=1}^M \mathbb{I}\left(g(\theta) \in I\left(X^{(i)}\right)\right) \approx \gamma$$
