Ogni analisi statistica inferenziale è caratterizzata da una componente di incertezza, poiché i [[campionamento|dati campionari]] $x$ sono interpretati come realizzazione di un vettore casuale $X$.

Se si ripete l'esperimento, nelle medesime condizioni, si ottengono dei dati $x^′$, tipicamente diversi da $x$.

Ogni inferenza sulla popolazione (sul parametro di interesse) va accompagnata da una valutazione, in termini di probabilità, sul suo grado di affidabilità/incertezza.

Nell'effettuare un analisi statistica, i dati campionari $x$ non vengono considerati così come sono ma vengono opportunamente sintetizzati.

Si chiama **statistica** (**campionaria**) ogni trasformata $T = t(X_1, . . . , X_n)$ che *sintetizza* opportunamente *il campione casuale* $X_1, . . . , X_n$.

La scelta della statistica riassuntiva $T$ deve essere fatta tenendo conto del modello statistico e dell'obiettivo dell'inferenza.

Il **valore osservato** $t = t(x_1, . . . , x_n)$ di $T$ è un'opportuna *sintesi dei dati campionari osservati* $x_1, . . . , x_n$, utile per l'inferenza su $θ$.

Se si ripete l'esperimento, nelle medesime condizioni, si ottengono dei dati $x^′$ e, tipicamente, si ha che $t^′ = t(x^′) \ne t = t(x)$.

$T$ è una variabile casuale con una determinata distribuzione di probabilità, chiamata **distribuzione campionaria**.

La bontà di $T$ , come statistica riassuntiva per fare inferenza su $θ$, si può valutare analizzando la sua distribuzione campionaria.

La distribuzione di probabilità di $T$, che è una funzione di $X = (X_1, . . . , X_n)$, dipende dal parametro ignoto $θ$. Quindi, va intesa **sotto** $θ$, cioè nell'ipotesi che $θ$ sia il vero valore del parametro, *qualunque esso sia*.

Dato un campione casuale $_X1, . . . , X_n$, sono esempi di statistiche campionarie: 
* la **somma campionaria** $S_n = \sum^n_{i=1} X_i$, la **media campionaria** $\bar X_n = n^{−1}S_n$, la **varianza campionaria** $S^2 = n^{−1} P_n \sum_{i=1}^n (X_i − \bar X_n)^2$ e la sua versione corretta $S^2_c$;
* le **statistiche ordinate** $X(1) \ge · · · \ge X_{(n)}$, dove $X_{(i)}$ è la variabile casuale che occupa l'i-esima posizione nel campione; 
* la **variabile casuale minimo** $X(1) = min{X_1, . . . , X_n}$ e la **variabile casuale massimo** $X(n) = max{X_1, . . . , X_n}$;
* la **mediana campionaria**, definita da $X_{((n+1)/2)}$, se $n$ è dispari, e da $(X_{(n/2)} + X_{((n/2)+1)})/2$, se $n$ è pari;
* i **momenti campionari**, centrati e non centrati, $n^{−1} \sum^n_{i=1} (X_i − \bar X_n)^r,\ n^{−1} \sum^n_{i=1} X^r_i,\ r \in \mathbb{N}^+$.
Nel seguito, oltre che definire le sintesi campionarie $S_n,\ \bar X_n,\ S^2$ e $S^2_c$, si presenteranno le loro proprietà, considerando opportuni risultati di calcolo delle probabilità.

>[!example] **Esempio**
>*Campioni gaussiani*. Sia $X_1, . . . , X_n$ un campione casuale semplice tratto da una popolazione normale, cioè $X_i \sim N (μ, σ^2),\ i = 1, . . . , n$. Si è interessati al parametro $θ = μ$ (*media della popolazione*) ed è ragionevole considerare, come sintesi del campione, la media campionaria $\bar X_n = (1/n) \sim^n_{i=1} X_i$ (*media del campione*). 
>
>Si ripete per due volte l'esperimento e si osservano i vettori: $$ \begin{gather} 
>x = (−0.89, −0.66, 0.93, 2.42, −2.29, −1.39, −0.86, 0.20, 1.96, −0.59, −1.36, −0.11, 0.52, 1.17, 0.13), \\ 
>x^′ = (−0.19, −1.52, 2.80, −0.17, −0.30, −0.02, 0.07, 1.69, −1.53, −2.74, −1.03, −0.88, 0.21, 0.18, −1.17).
\end{gather}$$ I due campioni osservati $x$ e $x^′$ sono diversi e danno origine a due realizzazioni diverse per la media campionaria: rispettivamente, $\sum^{15}_{i=1} x_i/15 = −0.05$ e $\sum^{15}_{i=1} x^{'}_i/15 = −0.31$.
>
Si determinano gli istogrammi delle frequenze relative riferiti ai campioni osservati $x$ e $x^′$.
![[Pasted image 20240211021804.png]]
Dalla analisi degli istogrammi si può ragionevolmente confermare che $x$ e $x^′$ provengono dalla medesima popolazione.
>
Quindi, nei due casi, l'inferenza su $μ$ porterà a conclusioni simili, anche se non uguali per effetto della variabilità campionaria.

***
Riferimenti:
#statistica_inferenziale 
#statisiche_campionarie