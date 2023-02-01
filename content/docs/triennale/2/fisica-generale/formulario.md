# Formulario

{{<katex>}}{{</katex>}}

## Generale

### Derivata di un vettore di modulo costante

> 📖 Un vettore di modulo costante è sempre perpendicolare alla sua derivata (rispetto al tempo)
>
> $$
> \vec{a} \perp \frac{d\vec{a}}{dt}
> $$

## Cinematica

### Problema diretto della dinamica

Sia noto il **vettore posizione** **\\(\vec{r}\\)**, troviamo il vettore **velocità** e il vettore **accelerazione**:

{{<katex display>}}
\vec{v} = \frac{d\vec{r}{dt}
{{</katex>}}}

{{<katex display>}}
\vec{a} = \frac{d\vec{v}}{dt} = \frac{d^2\vec{r}}{dt^2}
{{</katex>}}

### Problema inverso della dinamica

Sia noto il vettore accelerazione, troviamo velocità e posizione rispetto al tempo:

{{<katex display>}}
\vec{v}(t) = \vec{v}_0 + \int_{t_0}^{t} {\vec{a}(s)ds} \\
\vec{r}(t) = \vec{r}_0 + \int_{t_0}^{t} {\vec{v}(s)ds}
{{</katex>}}

## Rappr cartesiana → Rappr. intrinseca

Siano note le variabili cinematiche in rappr. cartesiana:

{{<katex display>}}
\vec{r} = x\hat{i} + y\hat{j} + z\hat{k} \\

\vec{v} = v_x\hat{i} + v_y\hat{j} + v_z\hat{k} \\

\vec{a} = a_x\hat{i} + a_y\hat{j} + a_z\hat{k}
{{</katex>}}

1. Troviamo il modulo della velocità lungo lo spostamento

   {{<katex display>}}
   \dot{s} = |\vec{v}| = \sqrt{v^2} = \sqrt{v_x^2 + v_y^2 + v_z^2}
   {{</katex>}}

2. Troviamo il versore tangente

$$
\hat{u}_t = \frac{\vec{v}}{|\vec{v}|}
$$

1. Troviamo la componente (il modulo) dell’accelerazione tangente allo spostamento

<p>
$$
   a_t =\ddot{s} =  \vec{a} \cdot \hat{u}_t \\
   \vec{a}_t = a_t \hat{u}_t
$$
</p>


2. Troviamo la componente normale dell’accelerazione normale allo spostamento

   $$
   \vec{a}_n = \vec{a}-\vec{a}_t \\
   a_n = |\vec{a}_n| = \sqrt{a^2 - a_t^2}
   $$

3. Troviamo il vettore normale

   $$
   \hat{u}_n = \frac{\vec{a}_n}{|\vec{a}_n|}
   $$

4. Troviamo il raggio di curvatura

   $$
   \rho = \frac{\dot{s}^2}{a_n}
   $$

5. **L’accelerazione totale** è

   $$
   \vec{a}=\ddot{s}\hat{u}_t + \frac{\dot{s}^2}{\rho}\hat{u}_n
   $$

## Coordinate polari piane

{{<katex display>}}
\begin{cases}
   x = r \cos{\phi} \\
   y = r \sin{\phi}
\end{cases}
\quad
\longrightarrow
\quad

\begin{cases}
 r = \sqrt{x^2 + y^2} \\
 \phi = \arctan{\frac{y}{x}}
\end{cases}
{{</katex>}}

## Moto circolare

$$
S(t) = R\cdot\phi(t)
$$

Con S arco di circonferenza {{<katex>}}[0\le S \le 2\pi R]{{</katex>}} e {{<katex>}}R=\vec{|r|}{{</katex>}} il raggio della circonferenza.

$$
\vec{r}(s)=R\cos\left(\frac{S}{R}\right) \hat{i} \ + \ R\sin\left(\frac{S}{R}\right)\hat{j}
$$

La posizione dipende solo dall’angolo {{<katex>}}\phi{{</katex>}}.

| Angolo:                 | {{<katex>}}\phi = \frac{S}{R}{{</katex>}}           |
| ----------------------- | --------------------------------------------------- |
| Velocità angolare:      | {{<katex>}}\omega = \dot{\phi}=\frac{\dot{S}}{R}=\frac{v}{R}{{</katex>}} |
| Accelerazione angolare: | {{<katex>}}\alpha=\dot{\omega} = \frac{\ddot{S}}{R}{{</katex>}}          |

{{<katex display>}}
\vec{v} = R\omega{\hat{u}_\phi}=\dot{S}{\hat{u}_\phi}\\
\vec{a}=R\alpha{\hat{u}_\phi}+R\omega^2({-\hat{u}_r})=\ddot{S}{\hat{u}_\phi}+ \frac{\dot{S}^2}{R}{-\hat{u}_r}
{{</katex>}}

## Moto periodico

Soluzione generale

$$
f(x)= A \cos{(\omega t+\phi_0)}
$$

Con

- {{<katex>}}T{{</katex>}} periodo
- {{<katex>}}\omega{{</katex>}} pulsazione, ovvero n. di giri compiuti nell’unità di tempo,
- {{<katex>}}\nu = \frac{1}{T}{{</katex>}} frequenza, ovvero n. di T contenuti nell’unità di tempo

### Moto oscillatorio armonico

$$
x(t) = l \cos{(\omega t + \phi_0)}
$$

con

| {{<katex>}}l{{</katex>}}                 | ampiezza      |
| ------------------- | ------------- |
| {{<katex>}}\omega t + \phi_0{{</katex>}} | fase          |
| {{<katex>}}\phi_0{{</katex>}}            | fase iniziale |

## Statica

### Momento di un vettore

↪️ **Momento** di un vettore applicato {{<katex>}}F{{</katex>}} rispetto al polo {{<katex>}}\Omega{{</katex>}}:

{{<katex display>}}
\begin{cases}
 \vec{M}_\Omega = \vec{r} \wedge \vec{F} \\

 M_\Omega = |\vec{r}| |\vec{F}| \sin{\theta}
\end{cases}
{{</katex>}}


### Statica del corpo esteso

Un corpo esteso risulta in condizione di equilibrio quando:

$\left\{\begin{aligned}
& \vec{R} \ = \sum{\vec{F}_i}=0 \\
& \vec{M}_\Omega = \sum {\vec{M}_i} = 0
\end{aligned}\right.$

## Dinamica

<aside>
↪️ **Principio di relatività galileiano**

Tutte le leggi della fisica si scrivono nello stesso modo in ogni sistema di riferimento inerziale.

</aside>

### Secondo principio della dinamica

<aside>
↪️ *In un sistema di riferimento inerziale, la forza complessiva che agisce su un corpo materiale è proporzionale all’accellerazione di quel corpo attraverso una costante di proporzionalità della **massa inerziale**.*

$$
\vec{F} = m\vec{a}
$$

</aside>

### Piano inclinato liscio

$$
t = \sqrt{\frac{2L}{g \sin \alpha}} = \sqrt{\frac{2h}{g \sin^2 \alpha}}
$$

- {{<katex>}}h{{</katex>}} → altezza del corpo rispetto alla {{<katex>}}h=0{{</katex>}}
- {{<katex>}}g{{</katex>}} → accelerazione di gravità

### Forza elastica / legge di Hooke

$$
\vec{F} = -kx \hat{i}
$$

### Pendolo semplice

$$
\theta(t) = \alpha \sin(\omega t),
\quad \alpha = \frac{v_0}{\sqrt{gl}},
\quad \omega = \sqrt{\frac{g}{l}}
$$

$$
\frac{d\theta}{dt} = \alpha \omega \cos{\theta}
$$

Reazione vincolare:

$$
R_v = ml \dot\theta + mg \cos{\theta}
$$

### Forza di attrito statico

$$
F_{AS} = \mu_S F_{\perp}
$$

con {{<katex>}}\mu_S{{</katex>}} coefficiente di attrito statico.

### Forza di attrito dinamico

{{<katex display>}}
\vec{F}_{AD} = \mu_D F_{\perp} (-\hat{u}_t)
{{</katex>}}

## Lavoro ed energia

### Lavoro infinitesimo e lavoro

Lavoro infinitesimo compito da {{<katex>}}\vec{F}{{</katex>}} durante uno spostamento infinitesimo {{<katex>}}d\vec{l}{{</katex>}}

$$
\delta\mathscr{L} = \vec{F} \cdot d\vec{l}, \quad \mathscr{L} = \int \delta\mathscr{L}
$$

In coordinate cartesiane:

{{<katex display>}}
\begin{align}
\mathscr{L} &= \underset{\ell}{\int_{A}^{B}} \vec{F}(x,y,z)\cdot d\vec{l} \\
            &= \underset{\ell}{\int_{A}^{B}} \left[F_{x}(x,y,z)dx + F_{y}(x,y,z)dy + F_{z}(x,y,z)dz \right]
\end{align}
{{</katex>}}

#### Lavoro di una forza elastica

{{<katex display>}}
\mathscr{L}_{1,2}
=\int_\ell -k \Delta x
=
-\frac{k}{2}
\left(x^2_2-x^2_1 \right)
{{</katex>}}

### Potenza di una forza

$$
P=\frac{\delta\mathscr{L}}{dt} = \vec{F}\cdot\vec{v}
$$

### Teorema delle forze vive

Per un punto materiale…

$$
T = \frac{1}{2}mv^2 \\
\text{La variazione di energia cinetica corrisponde al lavoro svolto}\\
\delta\mathscr{L} = dT
$$

### Forze conservative

Forze **posizionali** in cui il lavoro non dipende mai dal percorso, ma solo dal punto di partenza e dal punto di arrivo.

#### Prima proprietà - Circuitazione nulla

$$
\mathscr{L} = \oint{\vec{F}} \cdot dl = 0
$$

La circuitazione di un campo conservativo è nulla.

#### Seconda proprietà - Energia potenziale

$$
\mathscr{L}_{A,B}=U(A)-U(B) = \phi(B)-\phi(A)
$$

Esiste una funzione scalare, detta **energia potenziale** (o semplicemente **potenziale**), tale che _il lavoro per spostarsi dalla configurazione A alla configurazione B è dato dalla differenza tra l'energia potenziale in A e in B_.

#### Terza proprietà - Gradiente del campo

Esiste una funzione scalare {{<katex>}}U(P) = -\phi(P){{</katex>}}, detta energia potenziale, tale che..

$$
\vec{F} = -\vec\nabla U
$$

Il campo può essere scritto come gradiente di una funzione.

#### Quarta proprietà - Campo irrotazionale

$$
\vec\nabla \wedge \vec F = 0 \iff \text{campo conservativo}
$$

Il campo è conservativo se e solo se è irrotazionale.

### Conservazione dell’energia meccanica

In presenza di forze **tutte conservative**

<aside>
🪢 L’energia meccanica si conserva

$$
E = T + U = \text{costante}
$$

</aside>

### Potenziali notevoli

| Potenziale forza peso     | {{<katex>}}U(P)= mgz{{</katex>}}            |
| ------------------------- | ---------------------- | -------- | ----- |
| Potenziale elastico       | {{<katex>}}U(P) = k\frac{        | \vec r^2 | }{2}{{</katex>}} |
| Potenziale forza costante | {{<katex>}}U(P)=-f_xx-f_yy-f_zz{{</katex>}} |

# Terzo principio della dinamica

### Quantità di moto

$$
\vec q = m \vec v
$$

A massa costante, possiamo dire che

$$
\vec F = \frac {d\vec q} {dt}
$$

**La forza rappresenta quindi la variazione della quantità di moto nel tempo**.

## Urti

### Forze impulsive

Nell’istante in cui agiscono si può considerare il sistema come **\*\***\*\***\*\***isolato**\*\***\*\***\*\***

$$
\int_{t_1}^{t_2}{\vec F dt} = \vec q(t_2) - \vec q(t_1) = \Delta \vec q
$$

### Forza media

$$
\left<\vec F\right> = \frac 1 {\Delta t} \int_{t_1}^{t_2} {\vec F dt} = \frac{\vec q(t_2) - \vec q(t_1)}{\Delta t} = \frac{\Delta \vec q}{\Delta t}
$$

Con {{<katex>}}\left<F\right>{{</katex>}} forza media

### Urti collineari elastici

Si conservano sia la **\*\***\*\***\*\***\*\*\*\***\*\***\*\***\*\***quantità di moto**\*\***\*\***\*\***\*\*\*\***\*\***\*\***\*\*** che l’\***\*\*\*\*\*\*\***\*\*\***\*\*\*\*\*\*\***energia cinetica\***\*\*\*\*\*\*\***\*\*\***\*\*\*\*\*\*\***.

$$
Q_{\text{in}} = Q_{\text{fin}} \\
T_{\text{in}} = T_{\text{fin}}
$$

### Urti collineari totalmente anelastici

Si conserva solo la **\*\***\*\***\*\***\*\*\*\***\*\***\*\***\*\***quantità di moto**\*\***\*\***\*\***\*\*\*\***\*\***\*\***\*\***.

$$
Q_{\text{in}} = Q_{\text{fin}} \\

m_1 \vec v_{1} + m_2  \vec v_{2} = (m_1 + m_2) \vec v_{fin}
$$

# Elettrostatica

<aside>
<img src="https://www.notion.so/icons/mathematics_gray.svg" alt="https://www.notion.so/icons/mathematics_gray.svg" width="40px" /> Legge di Coulomb:

$$
\vec{F}_{12} = \frac{q_1q_2}{4\pi\epsilon_0}\frac{\vec{r}_2-\vec{r}_1}{\lvert\vec{r}_2-\vec{r}_1\rvert^3}
$$

</aside>

<aside>
<img src="https://www.notion.so/icons/mathematics_gray.svg" alt="https://www.notion.so/icons/mathematics_gray.svg" width="40px" /> Campo elettrostatico **carica puntiforme**:

$$
\vec{E}(\vec r) = \frac{1}{4\pi\epsilon_0}\frac{Q}{r^2}\hat{u}_r
$$

</aside>

<aside>
<img src="https://www.notion.so/icons/mathematics_gray.svg" alt="https://www.notion.so/icons/mathematics_gray.svg" width="40px" /> Forza elettrostatica sapendo il potenziale:

$$
\vec{F}(\vec{r}) = q\vec{E}(\vec{r})
$$

</aside>

<aside>
<img src="https://www.notion.so/icons/light-bulb_gray.svg" alt="https://www.notion.so/icons/light-bulb_gray.svg" width="40px" /> Il campo elettrico **è conservativo:**

$$
\oint_\Gamma \vec{E}\cdot d\vec{l} = 0
$$

$$
\vec{\nabla}\wedge\vec{E} = \vec{0}
$$

$$
\vec{E} = -\vec{\nabla}V
$$

$$
V(A)-V(B)=\int_A^B\vec{E}\cdot d\vec{l}
$$

{{<katex>}}V(x, y, z){{</katex>}} è detto **potenziale elettrostatico.**

</aside>

<aside>
<img src="https://www.notion.so/icons/mathematics_gray.svg" alt="https://www.notion.so/icons/mathematics_gray.svg" width="40px" /> Potenziale elettrostatico di una carica puntiforme:

$$
V(\vec{r}) = \frac{1}{4\pi\epsilon_0}\frac{Q}{r}
$$

</aside>

<aside>
<img src="https://www.notion.so/icons/mathematics_gray.svg" alt="https://www.notion.so/icons/mathematics_gray.svg" width="40px" /> Principio di sovrapposizione:

$$
\vec{F} = \sum_{i=1}^N\frac{1}{4\pi\epsilon_0}\frac{qq_i}{r_i^3}\vec{r}_i
$$

$$
\vec{E} = \sum_{i=1}^N\frac{1}{4\pi\epsilon_0}\frac{q_i}{r_i^3}\vec{r}_i
$$

$$
V(x, y, z) = \sum_{i=1}^N\frac{1}{4\pi\epsilon_0}\frac{q_i}{r_i}
$$

</aside>

### Densità volumetrica di carica:

$$
\rho = \frac{dq}{d\tau}
$$

$$
q_\tau = \iiint_\tau\rho d\tau
$$

### Densità superficiale di carica

Sia {{<katex>}}S{{</katex>}} una superficie

$$
\sigma= \frac{dq}{dS}
$$

$$
q_\tau = \iint_S\sigma dS
$$

### Densità lineare di carica

Sia {{<katex>}}l{{</katex>}} una curva

$$
\lambda = \frac{dq}{dl}
$$

$$
q_\tau = \int_l \lambda dl
$$

---

<aside>
<img src="https://www.notion.so/icons/mathematics_gray.svg" alt="https://www.notion.so/icons/mathematics_gray.svg" width="40px" /> Campo elettrostatico su distribuzioni continue:

$$
\vec{E}(\vec{r}) = \frac{1}{4\pi\epsilon_0}\iiint_\tau\frac{\rho(\vec{r}')(\vec{r}-\vec{r}')}{\lvert\vec{r}-\vec{r}'\rvert^3}d\tau
$$

$$
\vec{E}(\vec{r}) = \frac{1}{4\pi\epsilon_0}\iint_S\frac{\sigma(\vec{r}')(\vec{r}-\vec{r}')}{\lvert\vec{r}-\vec{r}'\rvert^3}dS
$$

$$
\vec{E}(\vec{r}) = \frac{1}{4\pi\epsilon_0}\int_l\frac{\lambda(\vec{r}')(\vec{r}-\vec{r}')}{\lvert\vec{r}-\vec{r}'\rvert^3}dl
$$

</aside>

---

<aside>
<img src="https://www.notion.so/icons/mathematics_gray.svg" alt="https://www.notion.so/icons/mathematics_gray.svg" width="40px" /> Potenziale elettrostatico su distribuzioni continue:

$$
V(\vec{r}) = \frac{1}{4\pi\epsilon_0}\iiint_\tau\frac{\rho(\vec{r}')}{\lvert\vec{r}-\vec{r}'\rvert}d\tau
$$

$$
V(\vec{r}) = \frac{1}{4\pi\epsilon_0}\iint_S\frac{\sigma(\vec{r}')}{\lvert\vec{r}-\vec{r}'\rvert}dS
$$

$$
V(\vec{r}) = \frac{1}{4\pi\epsilon_0}\int_l\frac{\lambda(\vec{r}')}{\lvert\vec{r}-\vec{r}'\rvert}dl
$$

</aside>

---

<aside>
<img src="https://www.notion.so/icons/mathematics_gray.svg" alt="https://www.notion.so/icons/mathematics_gray.svg" width="40px" /> **Lavoro** della forza elettrostatica:

$$
\mathcal{L}_{el}=\int_A^B\vec{F}_{el}\cdot d\vec{l} = q \Delta V_{AB}
$$

</aside>

---

<aside>
<img src="https://www.notion.so/icons/light-bulb_gray.svg" alt="https://www.notion.so/icons/light-bulb_gray.svg" width="40px" /> **Energia potenziale elettrostatica**:

$$
U_E = q\cdot V \\
U_E = \int F dl = q\int Edl = q\cdot V
$$

L’energia potenziale elettrostatica **si conserva** poiché è generata da una **forza conservativa**.

</aside>

---

<aside>
<img src="https://www.notion.so/icons/mathematics_gray.svg" alt="https://www.notion.so/icons/mathematics_gray.svg" width="40px" /> Il **flusso** del campo elettrico:

$$
d\Phi_S(\vec{E}) = \vec{E}\cdot \hat{n}dS
$$

</aside>

---

<aside>
<img src="https://www.notion.so/icons/mathematics_gray.svg" alt="https://www.notion.so/icons/mathematics_gray.svg" width="40px" /> Legge di Gauss

Il flusso del campo elettrico attraverso una **superficie chiusa** è pari alla **somma delle cariche interne** **alla superficie** diviso la costante dielettrica nel vuoto.

$$
\Phi_S(\vec{E}) = \oiint_S\vec{E}\cdot \hat{n}dS = \frac{Q_S}{\epsilon_0}
$$

</aside>

<aside>
<img src="https://www.notion.so/icons/light-bulb_gray.svg" alt="https://www.notion.so/icons/light-bulb_gray.svg" width="40px" /> Il **flusso** generatob attraverso una superficie da **cariche esterne alla superficie è nullo**.

</aside>

<aside>
<img src="https://www.notion.so/icons/light-bulb_gray.svg" alt="https://www.notion.so/icons/light-bulb_gray.svg" width="40px" /> Legge di Gauss in forma locale:

$$
div\vec{E} =
\vec{\nabla}\cdot \vec{E} = \frac{\rho}{\epsilon_0}
$$

</aside>

<aside>
<img src="https://www.notion.so/icons/light-bulb_gray.svg" alt="https://www.notion.so/icons/light-bulb_gray.svg" width="40px" /> Equazione di **Poisson**

$$
\nabla^2 V= -\frac{\rho}{\epsilon_0}
$$

</aside>

## Elettrostatica dei conduttori

### Campo elettrico all’interno dei conduttori

<aside>
<img src="https://www.notion.so/icons/light-bulb_gray.svg" alt="https://www.notion.so/icons/light-bulb_gray.svg" width="40px" /> Il campo elettrico interno ai conduttori è nullo in condizioni di equilibrio.

</aside>

### Campo elettrico in prossimità della superficie dei conduttori

Il campo in prossimità della superficie dei conduttori è perpendicolare alla superficie e di modulo:

$$
E = \frac{\sigma}{\epsilon_0}
$$

con {{<katex>}}\sigma{{</katex>}} densità superficiale di carica

### Conduttore sferico:

$$
\vec E =
\begin{cases}
0 & \text{se } r < R \\
\frac{1}{4\pi\epsilon_0}\frac{Q}{r^2}\hat{u}_r & \text{se } r > R
\end{cases}
$$

$$
V = \begin{cases}
\frac{Q}{4\pi\epsilon_0}\frac{1}{R} & \text{se } r < R \\
\frac{Q}{4\pi\epsilon_0}\frac{1}{r} & \text{se } r > R
\end{cases}
$$

---

### Conduttori collegati

Se due conduttori carichi vengono collegati, si forma un unico conduttore **equipotenziale** dunque il potenziale è il medesimo su entrambi gli oggetti.

**Esempio:**
Due sfere cariche collegate hanno potenziale:

- {{<katex>}}V_1 = \frac{1}{4\pi\epsilon_0}\frac{Q_1}{R_1}{{</katex>}}
- {{<katex>}}V_2 = \frac{1}{4\pi\epsilon_0}\frac{Q_2}{R_2}{{</katex>}}

Se esse vengono connesse: {{<katex>}}V_1 = V_2{{</katex>}}

Ne consegue:

$$
\frac{Q_1}{R_1} = \frac{Q_2}{R_2} \implies
Q_1R_2 = Q_2R_1
$$

Da cui si ricava:

$$
\left\{\begin{aligned}
Q_{1_f} = \frac{R_1}{R_1+R_2}(Q_{1_i} + Q_{2_i}) \\
Q_{2_f} = \frac{R_2}{R_1+R_2}(Q_{1_i} + Q_{2_i})
\end{aligned}
\right.
$$


---

### Capacità

$$
C = \frac{Q}{V}
$$

Con {{<katex>}}Q{{</katex>}} quantità di carica e {{<katex>}}V{{</katex>}} voltaggio tra le due armature.

<aside>
<img src="https://www.notion.so/icons/light-bulb_gray.svg" alt="https://www.notion.so/icons/light-bulb_gray.svg" width="40px" /> Capacità di un **conduttore** sferico:

$$
C=4\pi\epsilon_0R
$$

</aside>

<aside>
<img src="https://www.notion.so/icons/light-bulb_gray.svg" alt="https://www.notion.so/icons/light-bulb_gray.svg" width="40px" /> Capacità di un condensatore piano:

$$
C = \frac{\epsilon_0 S}{d}
$$

</aside>

<aside>
<img src="https://www.notion.so/icons/light-bulb_gray.svg" alt="https://www.notion.so/icons/light-bulb_gray.svg" width="40px" /> Capacità condensatore sferico:

$$
C = 4\pi\epsilon_0 \left(\frac{R_1R_2}{R_2-R_1}\right)
$$

</aside>

---

<aside>
<img src="https://www.notion.so/icons/mathematics_gray.svg" alt="https://www.notion.so/icons/mathematics_gray.svg" width="40px" /> Condensatori in **parallelo**:

$$
C_{\text{TOT}} = \sum C_i
$$

</aside>

<aside>
📖 Condensatori in **serie**:

$$
\frac 1 {C_{\text{TOT}}} =
\sum \frac 1 {C_i}
$$

</aside>

---

## Energia potenziale sistemi di cariche

<aside>
<img src="https://www.notion.so/icons/mathematics_gray.svg" alt="https://www.notion.so/icons/mathematics_gray.svg" width="40px" /> Energia potenziale tra due cariche:

$$
U_{12} = U_{21} = \frac{q_1q_2}{4\pi \epsilon_0r_{12}}
$$

Energia potenziale elettrostatica di un sistema di cariche:

$$
U_E = \sum_{i=1}^N\sum_{j>i}^N\frac{q_iq_j}{4\pi\epsilon_0r_{ij}}
$$

</aside>

---

<aside>
<img src="https://www.notion.so/icons/mathematics_gray.svg" alt="https://www.notion.so/icons/mathematics_gray.svg" width="40px" /> Energia immagazzinata in un condensatore:

$$
U_e
= \frac{Q^2}{2C}
= \frac 1 2 (\Delta V)^2 \ C
= \frac 1 2 \Delta V Q
$$

</aside>

---

#### Densità volumetrica di energia:

$$
u_E = \frac{1}{2}\epsilon_0E^2 = \frac{dU_E}{d\tau}
$$

$$
U_E = \int_\tau u_E d\tau
$$

---

### Condensatori con dielettrici

$$
\left\{
\begin{aligned}
&\vec{E} = \frac{1}{\epsilon_r}\vec{E}_0\\
&\Delta V = \frac{1}{\epsilon_r}\Delta V_0 \\
& C = \epsilon_rC_0 = \epsilon_r\epsilon_0\frac{S}{d}
\end{aligned}
\right.
$$

# Correnti

<aside>
<img src="https://www.notion.so/icons/mathematics_gray.svg" alt="https://www.notion.so/icons/mathematics_gray.svg" width="40px" /> Intensità di corrente: [Ampere]

$$
i = \frac{dq}{dt}
$$

</aside>

---

<aside>
<img src="https://www.notion.so/icons/mathematics_gray.svg" alt="https://www.notion.so/icons/mathematics_gray.svg" width="40px" /> Densità di corrente:

- {{<katex>}}n = \frac{N}{d\tau}{{</katex>}}
- {{<katex>}}dq = Ne^+= nq_e^+d\tau{{</katex>}}
- {{<katex>}}d\tau = [(\vec{v}_d\cdot \hat{n})dt]dS{{</katex>}}

$$
\vec{j} = nq_e\vec{v}_d, \qquad
i = \frac{dq}{dt} = \iint_S \vec{j}\cdot \hat{n}dS
$$

</aside>

---

<aside>
<img src="https://www.notion.so/icons/mathematics_gray.svg" alt="https://www.notion.so/icons/mathematics_gray.svg" width="40px" /> Equazione di continuità:

$$
\vec{\nabla}\cdot \vec{j} = -\frac{\partial \rho}{\partial t}
$$

**La divergenza del vettore intensità bilancia la variazione di carica**, una varazione di cariche corrisponde ad un moto di cariche **non solenoidale**.

</aside>

<aside>
<img src="https://www.notion.so/icons/attachment_gray.svg" alt="https://www.notion.so/icons/attachment_gray.svg" width="40px" /> In condizioni stazionarie la carica entrante in una superficie è pari alla carica uscente dalla stessa:

$$
\Delta q = q_{out}-q_{in} = 0\\
i_{uscente} = 0
$$

Il **flusso** della densità di corrente è **nullo**:

$$
\Phi_S(\vec{J}) = \oiint_S\vec{J}\cdot \hat{n}dS = 0
$$

E il **campo densità di corrente** è **solenoidale** (linee di campo sempre chiuse):

$$
\vec{\nabla}\cdot\vec{J} = 0
$$

</aside>

---

### Modello di Drude - Lorentz

<aside>
<img src="https://www.notion.so/icons/mathematics_gray.svg" alt="https://www.notion.so/icons/mathematics_gray.svg" width="40px" /> Velocità media (o di deriva):

$$
\vec{v}_d = \langle\vec{v}_e\rangle = \frac{q_e}{m_e}\vec{E}\langle t\rangle
$$

Dove {{<katex>}}\langle t \rangle{{</katex>}} è il tempo medio che intercorre tra due urti.

</aside>

---

<aside>
<img src="https://www.notion.so/icons/mathematics_gray.svg" alt="https://www.notion.so/icons/mathematics_gray.svg" width="40px" /> Conducibilità elettrica:

$$
\sigma_C = \frac{mq_e^2}{m_e}\langle t\rangle\\
\vec{J} = \sigma_C\vec{E}
$$

</aside>

<aside>
<img src="https://www.notion.so/icons/mathematics_gray.svg" alt="https://www.notion.so/icons/mathematics_gray.svg" width="40px" /> Resistività elettrica:

$$
\rho_R = \frac{1}{\sigma_C}\\
\vec{E} = \rho_R\vec{J}
$$

</aside>

---

<aside>
<img src="https://www.notion.so/icons/mathematics_gray.svg" alt="https://www.notion.so/icons/mathematics_gray.svg" width="40px" /> Prima legge di Ohm:

$$
\Delta V = Ri
$$

</aside>

<aside>
<img src="https://www.notion.so/icons/attachment_gray.svg" alt="https://www.notion.so/icons/attachment_gray.svg" width="40px" /> Legge di Ohm generalizzata:

$$
\Delta V + \sum_k \mathcal{E}_k = R_{\text{TOT}} \ i
$$

</aside>

<aside>
<img src="https://www.notion.so/icons/mathematics_gray.svg" alt="https://www.notion.so/icons/mathematics_gray.svg" width="40px" /> Seconda legge di Ohm:

$$
R = \rho_R \ \frac l S
$$

</aside>

---

<aside>
<img src="https://www.notion.so/icons/mathematics_gray.svg" alt="https://www.notion.so/icons/mathematics_gray.svg" width="40px" /> Resistenze in serie:

$$
R_{TOT} = \sum_i R_i
$$

Resistenze in parallelo:

$$
\frac{1}{R_{TOT}} = \sum_i\frac{1}{R_i}
$$

</aside>

---

<aside>
<img src="https://www.notion.so/icons/mathematics_gray.svg" alt="https://www.notion.so/icons/mathematics_gray.svg" width="40px" /> Effetto Joule

$$
P = R \cdot i^2 = \Delta V \cdot i = \frac{\Delta V^2}{R}
$$

</aside>

---

<aside>
<img src="https://www.notion.so/icons/mathematics_gray.svg" alt="https://www.notion.so/icons/mathematics_gray.svg" width="40px" /> Prima legge di Kirchhoff (legge delle maglie)

$$
\sum_k\mathcal{E}_k = R_{TOT}i
$$

Su qualunque magli di un circuito la caduta di potenziale è uguale alla somma delle tensioni erogate dai generatori

</aside>

<aside>
<img src="https://www.notion.so/icons/mathematics_gray.svg" alt="https://www.notion.so/icons/mathematics_gray.svg" width="40px" /> Seconda legge di Kirchhoff (legge dei nodi)

$$
\sum_{nodo}i_k = \sum_{entranti}i_k-\sum_{uscenti}i_k = 0
$$

In qualunque nodo di un circuito la corrente totale entrante è uguale alla corrente uscente.

</aside>

### Corrente di spostamento (Condensatore)

$$
i_s = \epsilon_0 \frac{d\Phi (\vec{E})}{dt}
$$

# Magnetostatica

<aside>
<img src="https://www.notion.so/icons/light-bulb_gray.svg" alt="https://www.notion.so/icons/light-bulb_gray.svg" width="40px" /> Il campo magnetico è **solenoidale**

$$
\vec{\nabla}\cdot \vec{B} = 0
$$

Di conseguenza il **flusso è nullo su una qualsiasi superficie chiusa**:

$$
\Phi_S(B) = \oiint_S\vec{B}\cdot \hat{n}dS = 0
$$

La ciruitazione è **non nulla**:

$$
\oint_\Gamma \vec{B}\cdot d\vec{l} \ne 0
$$

E il rotore **non è nullo**:

$$
\vec{\nabla}\wedge \vec{B}\ne 0
$$

Il campo magnetico **non è conservativo**

</aside>

## Campo magnetico generato da un solenoide

Campo interno generato da un solenoide con

| Numero di spire      | {{<katex>}}N{{</katex>}} |
| -------------------- | --- |
| Lunghezza            | {{<katex>}}L{{</katex>}} |
| Corrente stazionaria | {{<katex>}}i{{</katex>}} |

$$
\vec B = \mu_0 ni\hat k = \mu_0 \frac N L i \hat k
$$

Esternamente il campo è nullo.

## Seconda legge di Laplace

$$
d\vec{F} = id\vec{l}\wedge\vec{B}
$$

$$
\vec{F} = \int_{filo}\vec{j}\wedge \vec{B}d\tau
$$

è la forza su un filo di lunghezza {{<katex>}}l{{</katex>}} e volume {{<katex>}}\tau{{</katex>}} immerso in un campo magnetico.

## Forza di Lorentz

$$
\vec{F} = q\vec{v}\wedge \vec{B}
$$

con {{<katex>}}\vec v{{</katex>}} velocità della particella carica in movimento e {{<katex>}}\vec B{{</katex>}} campo magnetico in cui è immersa.

Generalizzando, **una particella carica immersa in un campo elettromagnetico subisce una forza:**

$$
\vec{F} = q\vec{E} +q\vec{v}\wedge \vec{B}
$$

<aside>
<img src="https://www.notion.so/icons/attachment_gray.svg" alt="https://www.notion.so/icons/attachment_gray.svg" width="40px" /> Uguagliando la forza di Lorentz alla forza centripeta si ottiene:

- Raggio di curvatura → {{<katex>}}R = \frac{mv}{qB}{{</katex>}}
- Periodo di rotazione → {{<katex>}}T = 2\pi \frac{m}{qB}{{</katex>}}
- Velocità angolare → {{<katex>}}\omega = \frac{qB}{m}{{</katex>}}
</aside>

---

<aside>
<img src="https://www.notion.so/icons/mathematics_gray.svg" alt="https://www.notion.so/icons/mathematics_gray.svg" width="40px" /> Momento magnetico di una spira

$$
\vec{M} = iS\hat{n}\wedge\vec{B}
$$

$$
\vec{M} = \vec{m}\wedge \vec{B}
$$

con {{<katex>}}\vec{m} = iS\hat{n}{{</katex>}}

</aside>

---

<aside>
<img src="https://www.notion.so/icons/mathematics_gray.svg" alt="https://www.notion.so/icons/mathematics_gray.svg" width="40px" /> **Prima legge di Laplace** - campo magnetico generato da un filo infinitesimo percorso da corrente:

---

$$
d\vec{B} = \frac{\mu_0i}{4\pi}\frac{d\vec{l}\wedge \vec{r}}{r^3}\\
\lvert d\vec{B}\rvert = \frac{\mu_0 i}{4\pi}\frac{dl\sin(\theta)}{r^2}
$$

</aside>

---

<aside>
<img src="https://www.notion.so/icons/mathematics_gray.svg" alt="https://www.notion.so/icons/mathematics_gray.svg" width="40px" /> **Legge di Biot-Savart** - campo magnetico generato da un filo rettilineo di lunghezza indefinita:

$$
\vec{B}  = \frac{\mu_0i}{2\pi r}
$$

</aside>

---

<aside>
<img src="https://www.notion.so/icons/mathematics_gray.svg" alt="https://www.notion.so/icons/mathematics_gray.svg" width="40px" /> Forza tra due fili percorsi da corrente:

$$
dF_{12} = \frac{\mu_0}{2\pi}\frac{i_1i_2}{d}dl_2
$$

La forza è attrattiva se i due fili sono percorsi nello stesso verso, repulsiva altrimenti.

</aside>

## Legge di Ampere

$$
\oint_\Gamma \vec{B}\cdot d\vec{l} = \mu_o\sum_k^{conc}i_k
$$

La **circuitazione** di un campo magnetico è **proporzionale** alla somma delle **correnti concatenate**.

$$
\sum_k^{conc}i_k = \iint_S \vec{J}_c \cdot \hat{n}dS
$$

Dove {{<katex>}}S{{</katex>}} è una generica superficie orientata che ha per bordo {{<katex>}}\Gamma{{</katex>}} e {{<katex>}}J_c{{</katex>}} è la densità di corrente concatenata.

**In forma locale otteniamo:**

$$
\vec{\nabla}\wedge \vec{B} = \mu_0\vec{J}
$$

In ogni punto dello spazio, il **rotore** del campo magnetico è **proporzionale** alla **densità di corrente** in quel punto.


## Elettromagnetismo

### Leggi di Maxwell

#### Flusso del campo elettrico

$$
\vec \nabla \cdot \vec E = \frac \rho {\epsilon_0},
\qquad
\oiint_S {\vec E \cdot \hat n dS = \frac{Q_s}{\epsilon_0}}
$$

Con {{<katex>}}\vec E{{</katex>}} campo elettrico, {{<katex>}}\rho{{</katex>}} densità di carica.

Il flusso del campo elettrico attraverso una superficie chiusa {{<katex>}}S{{</katex>}} è uguale al rapporto tra la carica totale presente all’interno della superficie e la costante dielettrica nel vuoto.

#### Flusso del campo magnetico

$$
\vec \nabla \cdot \vec B = 0,
\qquad \oiint_S {\vec B \cdot \hat n dS} = 0
$$

Con {{<katex>}}\vec B{{</katex>}} campo magnetico.

Il flusso del campo magnetico attraverso una superficie chiusa {{<katex>}}S{{</katex>}} è sempre nullo.

#### Circuitazione del campo elettrico (f.e.m.)

$$
\vec \nabla \wedge \vec E = - \frac {\partial \vec B}{\partial t}, \qquad \oint_\Gamma{\vec E \cdot d\vec l} = -\frac{d}{dt} \iint_S{\vec B \cdot \hat n dS}
$$

La circuitazione del campo elettrico (ovvero la differenza di potenziale = f.e.m.) su una linea chiusa {{<katex>}}\Gamma{{</katex>}} è uguale all’opposto della variazione nel tempo del flusso del campo magnetico attraverso la superificie chiusa {{<katex>}}S{{</katex>}} che “si appoggia” su {{<katex>}}\Gamma{{</katex>}}.

#### Circuitazione del campo magnetico

$$
\vec\nabla\wedge \vec B = \mu_0\vec j+\mu_0\epsilon_0 \frac{\partial\vec E}{\partial t}
,\qquad
\oint_\Gamma{ \vec B \cdot d\vec l} = \mu_0 \sum_k^{conc}{(i_c+i_s)}
$$

La circuitazione del campo magnetico su una linea chiusa {{<katex>}}\Gamma{{</katex>}} è proporzionale (con costante di proporzionalità {{<katex>}}\mu_0{{</katex>}}) alla somma delle correnti concatenate (che bucano la superficie) di spostamento e di conduzione.
