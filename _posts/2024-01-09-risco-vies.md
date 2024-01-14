---
tags: statistics
title: Risco e Viés
#published: false
sidebar:
    nav: docs-en
---

## Risco

$$R(\theta, \delta)=E_\theta\left[(\delta(\bar{X})-\theta)^2\right]$$

Um estimador bom, terá um risco baixo.

### Viés

$$\begin{gathered}
R(\theta, \delta)= \text{ var }_{\theta}(\delta(\bar{X})) + \text{viés}_{\theta}(\bar{\delta}) \\
\text{ viés }(\hat{\theta})=E(\hat{\theta})-g(\theta)
\end{gathered}$$

### Estimador $\theta$ não envieasado

$$\begin{aligned}
& \text { viés }(\hat{\theta})=0 \rightarrow E(\hat{\theta})=\theta \\
& \text { viés }(\hat{\theta}) \rightarrow R(\theta, \delta)=\text{ var }_\theta(\delta(\bar{X}))
\end{aligned}$$

- Lembrete: Nem sempre um estimador não-viesado existe.
- Lembrete 2: Nem sempre um estimador não-viesado é um bom estimador.

### Estimador não-viesado da variância

Seja $\boldsymbol{X}= \{X_1, X_2, \ldots, X_n \}$ uma amostra aleatória, com $E\left[X_1\right]=m e$ $\text{Var}\left(X_1\right)=v<\infty$. Então

$$\delta_1(\boldsymbol{X})=\frac{1}{n-1} \sum_{i=1}^n \left(X_i-\bar{X}_n \right )^2$$

é um estimador não-viesado de $v$.
