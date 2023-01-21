---
title: Coppie di variabili casuali
---

{{<katex>}}{{</katex>}}

# Coppie di variabili casuali discrete

## Funzione di massa di probabilità congiunta

\\(
\begin{aligned}
&p: \mathbb{R}^2 \to [0,1] \\\
 &p(a,b) = P(X=a, Y=b)
\end{aligned}
\\)

### Proprietà

1. \\(p(a,b) \in [0,1]\\)
2. {{<katex>}}\sum_{k=1}^n \sum_{j=1}^m p(a_k,b_j) = 1{{</katex>}}

## Funzioni di massa di probabilità marginali

\\(
\begin{aligned}
p_X(a) &= P(X=a) \\\ &= P(X=a, Y \text{qualsiasi}) \\\ &= \sum_{j=1}^m p(a,b_j)
\end{aligned}
\\)

---

\\(
\begin{aligned}
p_Y(b) &= P(Y=b) \\\ &= P(X \text{qualsias}, Y=b) \\\ &= \sum_{k=1}^n p(a_k,b)
\end{aligned}
\\)

### Esempio

{{<hint info>}}
Scatola di 12 palline. 3 rosse, 4 nere, 5 blu. Estrazione senza reimmissione di 3 palline.
Calcolare la funzione di massa congiunta e le funzioni di massa marginali.
{{</hint>}}

\\(X=\text{numero di palline rosse estratte}\\)

\\(Y=\text{numero di palline nere estratte}\\)

| Y \ X     | 0                      | 1                       | 2                      | 3                     | \\(p_y\\)               |
| --------- | ---------------------- | ----------------------- | ---------------------- | --------------------- | ----------------------- |
| 0         | \\( \frac{10}{220} \\) | \\( \frac{30}{220} \\)  | \\( \frac{15}{220} \\) | \\( \frac{1}{220} \\) | \\( \frac{56}{220} \\)  |
| 1         | \\( \frac{40}{220} \\) | \\( \frac{60}{220} \\)  | \\( \frac{12}{220} \\) | \\( 0 \\)             | \\( \frac{112}{220} \\) |
| 2         | \\( \frac{30}{220} \\) | \\( \frac{18}{220} \\)  | \\( 0 \\)              | \\( 0 \\)             | \\( \frac{48}{220} \\)  |
| 3         | \\( \frac{4}{220} \\)  | \\( 0 \\)               | \\( 0 \\)              | \\( 0 \\)             | \\( \frac{4}{220} \\)   |
| \\(p_x\\) | \\( \frac{84}{220} \\) | \\( \frac{108}{220} \\) | \\( \frac{27}{220} \\) | \\( \frac{1}{220} \\) |                         |


