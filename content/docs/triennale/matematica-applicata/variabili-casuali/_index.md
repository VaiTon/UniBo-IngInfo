---
title: Variabili casuali
tocLevels: 5
---

# Schema riassuntivo dei modelli di variabile casuale


## Modelli di variabili discrete

{{<katex display>}}
p(a):= \text{probabilità che la variabile casuale assuma il valore } a
{{</katex>}}

#### Funzione di ripartizione di probabilità

{{<katex display>}}
F(b)=\displaystyle\sum_{a=-\infty}^{b}p(a)
{{</katex>}}

#### Valore medio

{{<katex display>}}
E[X] = \displaystyle\sum_{k=1}^{n} x_k \cdot p(x_k) \quad X \in \{x_1, x_2, \dots, x_n\}
{{</katex>}}

---

### Bernoulli

{{<katex>}}
\begin{aligned}
X \sim Be(p), \qquad
&p:= \text{rappresenta la probabilità che si verifichi l'evento} \\
&\quad p \in (0,1) \\
&q := 1-p
\\ \\
&X = \begin{cases}
1 & \text{se l'evento si verifica} \\
0 & \text{se l'evento non si verifica}
\end{cases}

\end{aligned}
{{</katex>}}

{{<columns>}}
#### Funzione di massa di probabilità

{{<katex>}}
p(a) = \begin{cases}
p & \text{se } a=1 \\
1-p & \text{se } a=0
\end{cases}
{{</katex>}}

<--->

#### Funzione di ripartizione di probabilità

{{<katex>}}
F(b) = \begin{cases}
0 & \text{se } b<0 \\
p & \text{se } 0 \le b < 1 \\
1 & \text{se } b \ge 1
\end{cases}
{{</katex>}}

{{</columns>}}

{{<columns>}}

#### Valore medio

{{<katex>}}
E[X] = p
{{</katex>}}

<--->
#### Varianza

{{<katex>}}
Var(X) = p \cdot q
{{</katex>}}

{{</columns>}}

#### Funzione generatrice dei momenti

{{<katex>}}
\phi(t) = q + pe^{t}
{{</katex>}}

---

### Binomiale

{{<katex display>}}
\begin{aligned}
X \sim B(n,p) \qquad
&n:= \text{numero di volte che è stato ripetuto un esperimento} \\
&p:= \text{probabilità che l'evento si verifichi}
\end{aligned}
{{</katex>}}

{{<katex>}}
X= \displaystyle\sum^n _{j=1}Y_j \quad
\text{con} \ Y_1 ,..., Y_n \sim Be(p) \text{ indipendenti}
{{</katex>}}

{{<katex>}}X \in \{0,1,...,n\} :={{</katex>}} numero di prove in cui si verifica l'evento

{{<columns>}}

#### Funzione di massa di probabilità

{{<katex>}}
p(k) = \displaystyle \binom{n}{k}p^k(1-p)^{n-k}
{{</katex>}}

<--->

#### Valore medio

{{<katex>}}
E[X] = np
{{</katex>}}

{{</columns>}}

{{<columns>}}

#### Varianza

{{<katex>}}
Var(X) = npq
{{</katex>}}

<--->
#### Funzione generatrice dei momenti

{{<katex>}}
\phi(t) = (q + pe^{t})^n
{{</katex>}}

{{</columns>}}

#### Riproducibilità della binomiale

{{<katex display>}}
\left.\begin{aligned}
    X \sim B(n,p)\\
    Y \sim B(m,p)
\end{aligned}\right\}

\text{indipendenti} \Rightarrow X+Y \sim B(n+m,p)
{{</katex>}}

---

### Poisson

{{<katex display>}}
X \sim Po(\lambda ) \qquad \text{con} \  \lambda \in \mathbb{R}^+
{{</katex>}}

Una variabile casuale di Poisson rappresenta il numero di eventi che si osservano in un intervallo temporale/spaziale a patto che il singolo evento abbia una bassa probabilità di verificarsi

{{<columns>}}

#### Funzione di massa di probabilità

{{<katex>}}
p(k) = \displaystyle \frac{\lambda^k}{k!}e^{-\lambda}
{{</katex>}}

<--->

#### Valore medio

{{<katex>}}
E[X] = \lambda
{{</katex>}}

{{</columns>}}

{{<columns>}}

#### Momento secondo

{{<katex>}}
E[X^2] = \lambda + \lambda^2
{{</katex>}}

<--->
#### Varianza

{{<katex>}}
Var(X) = \lambda
{{</katex>}}

{{</columns>}}

#### Funzione generatrice dei momenti

{{<katex>}}
\displaystyle \phi(t) = e^{\lambda(e^t-1)}
{{</katex>}}

#### Riproducibilità della Poissoniana

{{<katex display>}}
\left.\begin{aligned}
    X \sim Po(\lambda) \\
    Y \sim Po(\mu )
\end{aligned}\right\}
\text{indipendenti} \ \Rightarrow X+Y \sim Po(\lambda +\mu)
{{</katex>}}

---

### Geometrica

Si ripete un esperimento finchè non si verifica un evento. Si conta il numero di volte che l'esperimento è stato ripetuto prima che l'evento si sia verificato.

{{<katex>}}
\begin{aligned}
X \sim G(p), \qquad &p:= \text{rappresenta la probabilità che si verifichi l'evento} \\
&p \in (0,1)
&q := 1-p
\end{aligned}
{{</katex>}}

#### Funzione di massa di probabilità

{{<katex display>}}
p(k) = (1-p)^{k-1} \cdot p
{{</katex>}}


## Modelli di variabili continue

{{<katex display>}}
f(a):= \text{densità di probabilità}
{{</katex>}}
<br>

**Proprietà:**
<br>
- {{<katex>}}
\displaystyle\int_{-\infty}^{\infty} f(a) da = 1
{{</katex>}}

{{<columns>}}

#### Funzione di ripartizione di probabilità

{{<katex display>}}
F(b)=\displaystyle\int_{-\infty}^{b}f(a) da
{{</katex>}}

<--->

#### Valore medio

{{<katex display>}}
E[X] = \displaystyle\int_{-\infty}^{+\infty} x \cdot f(x) dx
{{</katex>}}

{{</columns>}}

---

### Uniforme

{{<katex>}}
X \sim U(\alpha,\beta), \qquad \alpha < \beta
{{</katex>}}

<br>

{{<columns>}}

#### Funzione di densità di probabilità

{{<katex>}}
f(x) = \begin{cases}
k = \frac{1}{\beta-\alpha} & \text{se } \alpha \le x \le \beta \\
0 & \text{altrimenti}
\end{cases}
{{</katex>}}

<--->

#### Funzione di ripartizione di probabilità

{{<katex display>}}
F(a) = \begin{cases}
0 & \text{se } a < \alpha \\
\frac{a-\alpha}{\beta-\alpha} & \text{se } \alpha \le a \le \beta \\
1 & \text{se } a > \beta
\end{cases}
{{</katex>}}

{{</columns>}}
{{<columns>}}

#### Valore medio

{{<katex display>}}
E[X] = \displaystyle\frac{\alpha+\beta}{2}
{{</katex>}}

<--->

#### Varianza

{{<katex display>}}
Var(X) = \displaystyle\frac{(\beta-\alpha)^2}{12}
{{</katex>}}

{{</columns>}}

#### Coppie di variabili casuali uniformi

Siano

{{<katex display>}}
\left.\begin{aligned}
&X \sim U(\alpha,\beta) \\
&Y \sim U(\gamma,\delta)
\end{aligned} \right\} \text{indipendenti}
{{</katex>}}

##### Funzione di densità di probabilità congiunta

{{<katex display>}}
\underbrace{f(x,y) =f_X(x) \cdot f_Y(y)}_{\text{per l'indip.}}
= \begin{cases}
k = \frac{1}{(\beta-\alpha)(\delta-\gamma)} & \text{se }
x \in [\alpha, \beta], \ y \in [\gamma, \delta] \\
0 & \text{altrimenti}
\end{cases}
{{</katex>}}

##### Probabilità che {{<katex>}}(X,Y) \in \mathcal B{{</katex>}}

Sia {{<katex>}}R = \{(x,y) \in \mathbb R^2 \mid x \in [\alpha, \beta], \ y \in [\gamma, \delta]\}{{</katex>}}
il rettangolo di definizione di {{<katex>}}(X,Y){{</katex>}}.

{{<katex display>}}
\begin{aligned}
P((X,Y) \in \mathcal B) = \displaystyle\frac{\text{Area}(\mathcal B)}{\text{Area}(R)}
\end{aligned}
{{</katex>}}

---

### Esponenziale

{{<katex display>}}
X \sim E(\lambda), \qquad \lambda \in \mathbb R^+
{{</katex>}}

{{<hint danger>}}
N.B. Le variabili esponenziali **NON** sono riproducibili.
{{</hint>}}

{{<columns>}}

#### Funzione di densità di probabilità

{{<katex display>}}
f(x) = \begin{cases}
\lambda e^{-\lambda x} & \text{se } x \ge 0 \\
0 & \text{altrimenti}
\end{cases}
{{</katex>}}

<--->

#### Funzione di ripartizione di probabilità

{{<katex display>}}
F(a) = \begin{cases}
0 & \text{se } a < 0 \\
1-e^{-\lambda a} & \text{se } a \ge 0
\end{cases}
{{</katex>}}

{{</columns>}}

{{<columns>}}

#### Valore medio

{{<katex display>}}
E[X] = \displaystyle\frac{1}{\lambda}
{{</katex>}}

<--->

#### Varianza

{{<katex display>}}
Var(X) = \displaystyle\frac{1}{\lambda^2}
{{</katex>}}

{{</columns>}}

#### Funzione generatrice dei momenti

{{<katex display>}}
\phi(t) = \begin{cases}
\text{non esiste} & \text{se } t \ge \lambda \\
\displaystyle \frac{\lambda}{\lambda-t} & \text{se } t < \lambda
\end{cases}
{{</katex>}}


### Variabile casuale **NORMALE** (o Gaussiana)

{{<katex display>}}
X \sim N(\mu,\sigma^2)
\qquad \mu \in \mathbb R,
\ \sigma^2 \in \mathbb R^+
{{</katex>}}

{{<columns>}}

#### Funzione di densità di probabilità

{{<hint warning>}}
⚠️ **DA SAPERE A MEMORIA**
{{</hint>}}

{{<katex display>}}

f(x) = \frac{1}{\sqrt{2\pi\sigma^2}}
e^{\displaystyle -\frac{(x-\mu)^2}{2\sigma^2}}

{{</katex>}}

<--->

#### Funzione di ripartizione di probabilità

{{<katex display>}}
\begin{aligned}
F(a) &= \int_{-\infty}^a f(x) dx = \\
&= \int_{-\infty}^a \frac{1}{\sigma^2\sqrt{2\pi}}e^{-\frac{(x-\mu)^2}{2\sigma^2}} dx
\end{aligned}
{{</katex>}}
{{</columns>}}

{{<columns>}}

#### Massima probabilità

{{<katex display>}}
f(\mu) = \frac{1}{\sigma \sqrt{2\pi}}, \qquad \text{con } \mu = E[X]
{{</katex>}}

<--->

#### Funzione generatrice dei momenti

{{<katex display>}}
\phi(t) = e^{\mu t + \frac{t^2}{2} \sigma^2}
{{</katex>}}

{{</columns>}}
