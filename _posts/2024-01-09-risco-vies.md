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
R(\theta, \delta)=\operatorname{var}_\theta(\delta(\bar{X}))+\text { viés }_\theta(\bar{\delta}) \\
v i e ́ s(\hat{\theta})=E(\hat{\theta})-g(\theta)
\end{gathered}$$

### Estimador $\theta$ não envieasado

$$\begin{aligned}
& \text { viés }(\hat{\theta})=0 \rightarrow E(\hat{\theta})=\theta \\
& \text { viés }(\hat{\theta}) \rightarrow R(\theta, \delta)=\operatorname{var}_\theta(\delta(\bar{X}))
\end{aligned}$$

- Lembrete: Nem sempre um estimador não-viesado existe.
- Lembrete 2: Nem sempre um estimador não-viesado é um bom estimador.
