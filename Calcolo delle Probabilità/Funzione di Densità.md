>[!premise]- Ripasso %% Rimuovere? definizione forse superflua, presente nei lucidi %%
![[Variabili Casuali#^de955f]]

La funzione $f_x$ è chiamata **funzione di densità** ed è tale che:
* $f_X(x) \gt 0$, per ogni $x \in \mathbb{R}$;
* $\int^{+\infty}_{-\infty} f_X(x)dx=1$;
* $f_X(x) = \frac{d}{dx}F_X(x)$, per ogni $x \in R$ in cui $f_X(x)$ continua.
Quindi dalla conoscenza di $f_X$ si ottiene $F_X$ e viceversa; $f_X$ caratterizza la [[Variabili Casuali|variabile casuale]] $X$.
Dove $F_X$ è la [[funzione di ripartizione]].

Il [[supporto di una variabile casuale|supporto]] $S_X$ è un insieme continuo, ad esempio $\mathbb{R}$ o un intervallo o semiretta di $\mathbb{R}$.

Invece che assegnare probabilità a valori puntuali (si ricordi che, essendo $F_X$ continua, $P(X = x)=0$), per ogni $x \in \mathbb{R}$, si assegna probabilità agli intervalli, semirette, etc. di $\mathbb{R}$.

Gli eventi $(X \lt a)$ e $(x \le a)$, $a \in \mathbb{R}$, hanno la stessa probabilità.

Il valore della [[funzione di ripartizione]] in $x = 1,\ F_X(1)$, (grafico di sinistra) corrisponde all'area sottesa dalla funzione di densità con riferimento a $(-\infty, 1]$ (grafico di destra).
![[Pasted image 20240126010258.png]]
Inoltre, come conseguenza dei risultati di probabilità elementare, $$ P(X \gt a) = 1 - P(X \le a) = 1 - F_X(a),\ \text{per ogni}\ a \in \mathbb{R} $$ Vale il seguente risultato: per ogni $a,b \in \mathbb{R}, a \lt b$, $$ P(a \lt X \le b) = F_X(b) - F_X(a) = \int^b_a f_X(x)dx,$$ che corrisponde all'area sottesa dalla funzione di densità con riferimento all'intervallo $[a, b]$. Graficamente, se $[a, b] = [1, 2]$,
![[Pasted image 20240126022128.png]]
In generale, la probabilità associata all'evento $X \in B$ corrisponde a $$ P(X \in B) = \int_B f_X(x)dx $$[^formula1]
Si noti che *$f_X$ non definisce la probabilità associata all'evento $X = x$, che risulta essere nulla[^nota1]*, ma è direttamente proporzionale alla probabilità che $X$ assuma valori in un intorno di x;

>[!example] **Esempio**
>*Internet*. Una compagnia telefonica ha riscontrato che la durata, in un'ora, dei collegamenti internet dei propri utenti è descritta da una variabile casuale continua $X$ con funzione di densità $f_X(x)=6x(1-x)$, se $x \in [0,1]$, e nulla altrove
>![[Pasted image 20240126022501.png]]
>Si verifica facilmente che $\int^{+\infty}_{-\infty} f_X (x) dx = 1$ e che $f_X$ è non negativa.
>La funzione di ripartizione è tale che per $x \in [0,1],\ F_X(x) = 3x^2 - 2x^3$, mentre, se $x \lt 0,\ F_X(x)=0$ e, se $x \gt 1,\ F_X(x)=1$.
>
>La probabilità che $X$ assuma valori in $[0.5,0.7]$ è $$ 
>P(0.5 \le X \le 0.7) = F_X(0.7) - F_X(0.5) = \int^{0.7}_{0.5} 6x(1-x)dx=0.284 $$e corrisponde all'area evidenziata nel grafico sottostante
>![[Pasted image 20240126022948.png]]

^bca9ef

>[!example] **Esempio**
>*Variabile casuale esponenziale*. Una **variabile casuale** $X$ è **esponenziale**, in simboli $X \sim \text{Esp}(\lambda)$, con $\lambda \gt 0$, se $S_X = [0,\ +\infty)$ e $$ f_X(x) = \begin{cases}
>\lambda e^{-\lambda x} & \text{se}\ x \in S_X \\
>0 & \text{altrimenti}
>\end{cases} $$La [[funzione di ripartizione]] è $$F_X(x) = \int^x_{-\infty} \lambda e^{-\lambda t} dt = \int^x_0 \lambda e^{-\lambda t} dt = 1 - e^{-\lambda x}\ ,$$se $x \in S_X$, mentre $F_X(x) = 0$, se $x \notin S_X$.
>Si calcolano le probabilità $$\begin{gather}
>P(X \gt 1) = 1-F_X(1)=e^{-\lambda}, \\
>P(1 \le X \le 3) = F_X(3) - F_X(1) = e^{-\lambda}-e^{-3\lambda},
>\end{gather}
>$$ che, se $\lambda = 1$, corrispondono rispettivamente a $e^{-1}$ e $e^{-1}-e^{-3}$.
>La variabile casuale esponenziale viene utilizzata soprattutto per rappresentare durate e tempi di vita o funzionamento, nel caso in cui si ipotizza assenza di memoria o di usura.
>
>Si presentano, rispettivamente, i grafici della funzione di ripartizione e della funzione di densità nel caso $\lambda = 1$.
>![[Pasted image 20240127003058.png]]

^b9319c

>[!example] **Esempio**
>*Variabile casuale uniforme*. Una **variabile casuale continua** $X$ è **uniforme** in $[0, 1]$, in simboli $X \sim U(0,1)$, se $S_X=[0,1]$ e $$ f_X(x) = \begin{cases}
>1 & \text{se}\ x \in S_X \\
>0 & \text{altrimenti}
>\end{cases}$$ La funzione di ripartizione è $$ F_X(x) = \begin{cases} 
>0 & \text{se}\ x \lt 0 \\
>x & \text{se}\ 0 \le x \lt 1 \\
>1 & \text{se}\ x \ge 1 \end{cases} $$Si noti che, se gli intervalli $[a, b]$ e $[c, d]$ del support, con $a \lt b$ e $c \lt d$, hanno uguale ampiezza $h$, allora $$P(a \le X \le b) = P(c \le X \le d) = h \cdot 1 = h$$Dunque, tutti gli intervalli del supporto di uguale lunghezza hanno la stessa probabilità di contenere un valore di $X$.
>
>La variabile casuale uniforme continua viene utilizzata per esperimenti aleatori che possono essere rappresentati come un'estrazione casuale di un numero da un certo intervallo di $\mathbb{R}$.
>
>È un modello che descrive l'equiprobabilità nel continuo.
>
>Si presentano, rispettivamente, i grafici della funzione di ripartizione e della funzione di densità.
>![[Pasted image 20240127004214.png]]

^774c2e

***
Riferimenti:
[[Lucidi & materiale/5_prob_varcasual_L5.pdf#page=19&selection=12,0,12,19|5_prob_varcasual_L5, page 19]]

Risorse Esterne:
[Wikipedia - Funzione di Densità di Probabilità](https://it.wikipedia.org/wiki/Funzione_di_densit%C3%A0_di_probabilit%C3%A0?useskin=vector)

[^formula1]:Integrale su tutto $B$, $B$ può essere anche "disgiunto"

[^nota1]:Poiché la variabile casuale è continua

#variabili_casuali 
#ppt-4 