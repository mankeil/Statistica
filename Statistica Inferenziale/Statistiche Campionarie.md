Ogni analisi statistica inferenziale è caratterizzata da una componente di incertezza, poiché i dati campionari $x$ sono interpretati come realizzazione di un vettore casuale $X$.

Se si ripete l'esperimento, nelle medesime condizioni, si ottengono dei dati $x^′$, tipicamente diversi da $x$.

Ogni inferenza sulla popolazione (sul parametro di interesse) va accompagnata da una valutazione, in termini di probabilità, sul suo grado di affidabilità/incertezza.

Nell'effettuare una analisi statistica, i dati campionari $x$ non vengono considerati così come sono ma vengono opportunamente sintetizzati.

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

esempi


***
Riferimenti:
#statistica_inferenziale 
#statisiche_campionarie