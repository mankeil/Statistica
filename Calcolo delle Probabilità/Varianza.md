Data una variabile casuale [[Variabili Casuali#Variabili Casuali Discrete|discreta]] o [[Variabili Casuali#Variabili Casuali Continue|continua]] $X$, con [[supporto di una variabile casuale|supporto]] $S_X$ e [[funzione di densità]] di probabilità $f_X$, si chiama **varianza** di $X$, in simboli **$V(X)$**, la quantità $$ V(X) = E((X-E(X))^2),$$se esiste finita, ovvero
se $X$ è **discreta** $$ V(X) = \sum_{x \in S_X} (x-E(X))^2 f_X(x),$$se $X$ è **continua** $$V(X) = \int^{+\infty}_{-\infty} (x-E(X))^2 f_X (x)\ dx,$$ purché la serie o l'integrale siano convergenti. ^ffc822

È l'indice di variabilità più noto. Usualmente si pone $V(X) = \sigma^2$ e si intende tacitamente che il valore atteso della definizione esista finito.

La varianza è il [[valore atteso]] della variabile casuale scarto $X - E(X)$ elevata al quadrato e misura la dispersione della [[distribuzione di probabilità]] attorno alla media.

Lo **scarto quadrico medio** di $X$, indicato con $\sigma$, è la radice quadrata aritmetica (l'unica positiva) della varianza $$\sigma = \sqrt{V(X)}$$
Valgono inoltre le seguenti proprietà, per le quali si ommettono le dimostrazioni essendo sostanzialmente analoghe a quelle viste per la [[Statistica Descrittiva/Varianza|varianza in statistica descrittiva]]: ^892494
* **Proprietà di non negatività**: $V(X) \ge 0$, con $V(X) = 0$ se e solo se $X$ è [[variabile statistica degenere|degenere]].
* **Formula per il calcolo**: $V(X) = E(X^2) - (E(X))^2$.
* **Proprietà di invarianza per translazioni**: $V(X + b) = V(X),$ $b \in \mathbb{R}$.
* **Proprietà di omogeneità di secondo grado**: $V(aX) = a^2V(X)$, $a \in \mathbb{R}$.

Dalla ultime due proprietà discende che $V(aX+b) = a^2 V(X)$, con $a,b \in \mathbb{R}$.

Inoltre data una variabile casuale $X$, con media $\mu = E(X)$ e varianza $\sigma^2 = V(X)$, la variabile casuale trasformata $$Y = \frac{X - \mu}{\sigma}$$è tale che $E(Y) = 0$ e $V(Y) = 1$ ed è detta **variabile casuale standardizzata**.

Viceversa, a partire da una variabile casuale $Y$, con $E(Y) = 0$ e $V(Y) = 1$, utilizzando la trasformata $$X = \sigma Y + \mu$$si ottiene una variabile casuale $X$ con prefissati valor medio $\mu$ e varianza $\sigma^2$.

>[!example] **Esempio**
>*Moneta* ([[Variabili Casuali#^92e4b2|continua]]).Si considera la variabile casuale $X$ che conta il numero di esiti testa in tre lanci di una moneta regolare. In questo caso, $S_X = \set{0,1,2,3}$ e $P(X=0)=P(X=3)=1/8,$ $P(X=1) = P(X=2)=3/8$ ed è facile verificare che $$ \begin{align} E(X) = 0 + 1 \frac{3}{8} + 2\frac{3}{8} + 3\frac{1}{8} = \frac{3}{2}, \\
>E(X^2) = 0 + 1 \frac{3}{8} + 4 \frac{3}{8} + 9 {1}{8} = 3.
>\end{align}
>$$Con la regola per il calcolo, si ha $V(X) = 3 - (3/2)^2 = 3/4$.

>[!example] **Esempio**
>*Variabile casuale uniforme* ([[Funzione di Densità#^b9319c|continua]]). Si consideri la variabile casuale $X \sim U(0,1)$. Poiché $E(X) = 1/2$ e $$ E(X^2) = \int^1_0 x^2 \cdot 1\ dx = \frac{1}{3}, $$si conclude che $V(X) = 1/3 - (1/2)^2 = 1/12$.

>[!example] **Esempio**
>*Variabile casuale esponenziale* ([[Funzione di Densità#^b9319c|continua]]). Si consideri la variabile casuale $X \sim \text{Esp}(\lambda)$. Poiché $E(X) = 1/\lambda$ e, integrando per parti, $$ E(X^2) = \int^{+\infty}_{0} \lambda x^2 e^{-\lambda x}\ dx = \frac{2}{\lambda} \int^{+\infty}_{0} \lambda x e^{-\lambda x}\ dx = \frac{2}{\lambda^2},$$si conclude che $V(X) = 2/\lambda^2 - (1/\lambda)^2 = 1/\lambda^2$.

>[!example] **Esempio**
>*Internet* ([[Funzione di Densità#^bca9ef|continua]]). Si considera la variabile casuale $X$ che misura la durata, in un'ora, dei collegamenti internet degli utenti di una certa compagnia telefonica. Poiché $E(X) = 1/2$ e $$E(X^2) = \int^1_0 x^2 6x(1-x)\ dx = \int^1_0 6x^3 - 6x^2\ dx = \frac{3}{10},$$si conclude che $V(X) = 3/10 - (1/2)^2 = 1/20$.

>[!example] **Esempio**
>*Costante di normalizzazione*. Si consideri la variabile casuale continua $X$ con [[funzione di densità]] di probabilità $$f_X(x) = \begin{cases} kx^2 & \text{se } x \in [0, 2] \\ 0 & \text{altrimenti}, \end{cases}$$con $k$ una opportuna costante reale. Si vuole determinare $k$ in modo che $f_X(x) \ge 0$, per ogni $x \in \mathbb{R}$, e che $$ \int^{+\infty}_{-\infty} f_X(x)\ dx = \int^2_0 k x^2\ dx = 1; $$pertanto che $k = 3/8$. La [[funzione di ripartizione]] è tale che, per $x \in [0,2]$, $$ F_X(x) = \frac{3}{8} \int^x_0 t^2\ dt = \frac{x^3}{8}, $$mentre è nulla per $x \lt 0$ e vale 1 per $x \gt 2$. Si riportano i grafici
>![[Pasted image 20240205191406.png]]
>Come si vede dal grafico di sinistra, $x_{mo} = 2$^[[[Calcolo delle Probabilità/Moda|Moda]]]. mentre il [[valore atteso]] è $$ E(X) = \frac{3}{8} \int^2_0 x^2\ dx = \frac{3}{2}.$$La [[Calcolo delle Probabilità/Mediana|mediana]] è il valore $x_{0.5} \in \mathbb{R}$ tale che $F_X(x_{0.5}) = x^3_{0.5}/8 = 1/2$, quindi $x_{0.5} = \sqrt[3]{4}$.
>Infine, utilizzando la formula per il calcolo, si ottiene la varianza $$ V(X) = E(X^2) - (E(X))^2 = \frac{3}{8} \int^2_0 x^4\ dx - \frac{9}{4} = \frac{3}{20}$$

***
Riferimenti:
[[Lucidi & materiale/5_prob_varcasual_L5.pdf#page=44&selection=12,0,12,31|5_prob_varcasual_L5, page 44]]

#probabilità 
#ppt-5 
#indici_sintetici 
#indici_sintetici/indici_di_variabilità 