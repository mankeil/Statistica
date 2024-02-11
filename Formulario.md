In ordine alfabetico.
# I:
## Indice di Connessione
$$\chi^2 = \sum^m_{r=1} \sum^k_{s=1} \frac{(n_{rs}-n^*_{rs})^2}{n^*_{rs}},\ \ n^*_{rs} = \frac{n_{r+}n_{+s}}{n}$$dove:
* $m$ e $k$ indicano, rispettivamente, il numero di righe e di colonne della [[tabella di contingenza]].
* $n_{r+},\ n_{+s}$ sono le frequenze assolute marginali, di riga e di colonna rispettivamente. Vedasi: [[Distribuzioni di Frequenza]]  
* $n^*_{rs} = (n_{r+}n_{+s})/n$ è la frequenza attesa nel caso di indipendenza.
### Indice di connessione normalizzato
$$ \frac{\chi^2}{n \cdot min(m - 1,\ k-1)} $$dove $n \cdot min(m-1, k-1)$ è il valore massimo di $\chi^2$.
# M:
## Moltiplicazione di Probabilità (Formula)

$$ P(B\cap A) = P(A) \times P(B) = P(A) P(B|A) $$
Dove $P(B|A)$ è la [[Probabilità condizionata]] [[#Probabilità condizionata|formula]].

# P:
## Probabilità Condizionata
La [[probabilità]] che $B$ si realizzi una volta che $A$ si è realizzato: $$ P(B|A) = \frac{P(B \cap A)}{P(A)}$$
# T:
## Test chi quadrato di Pearson
Vedasi: [[#Indice di Connessione]]
# V:
## Varianza

### Variabili statistiche 

Dato $Y = (y_1,...,y_n)$, $$ \sigma^2 = V(Y) = \frac{1}{n} \sum^J_{j=1}(y_j-E(Y))^2f_j = \sum^J_{j=1}(y_j-E(Y))^2p_j = \frac{1}{n} \sum^n_{i=1}(y_i - E(Y))^2$$Dove:
* **$n$** è il numero di osservazioni.
* **$J$** è la dimensione del [[supporto di una variabile statistica|supporto]] $S_X$.
* **$f_j$** è la [[Frequenze Assolute|frequenza assoluta]]
* **$p_j$** è la [[Frequenze Relative|frequenza relativa]]

Nel caso in cui le [[modalità]] siano [[Classi di modalità|distribuite in classi]]:
$$ V(Y) = \frac{1}{n} \sum^J_{j=1}(y^c_j - E(Y))^2 f_j = \sum^J_{j=1}(y^c_j - E(Y))^2 p_j $$
Dove, inoltre, **$y^c_j$** è il *punto centrale* della classe $y^c_j = (y_{j-1}+y_j)/2,\ j=1,...,J$.

### Variabili casuali
Data una variabile casuale $X$:
se $X$ è **[[Variabili Casuali#Variabili Casuali Discrete|discreta]]** $$ V(X) = \sum_{x \in S_X} (x-E(X))^2 f_X(x),$$se $X$ è **[[Variabili Casuali#Variabili Casuali Continue|continua]]** $$V(X) = \int^{+\infty}_{-\infty} (x-E(X))^2 f_X (x)\ dx,$$purché la serie o l'integrale siano convergenti.
Dove $f_X$ è la [[funzione di densità]].