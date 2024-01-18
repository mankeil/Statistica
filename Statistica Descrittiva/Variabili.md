Una variabile è una caratteristica delle unità statistiche che, al variare dell'unità, può assumere una pluralità di valori.

Le **modalità** di una variabile sono i valori che essa può assumere (e si presumono noti preliminarmente). Sono, in genere, aggettivi, valori numerici, espressioni verbali.
Le variabili si indicano con le lettere maiuscole, ad esempio $Y$ , mentre una generica modalità si indica con $y$. L'insieme $Y$ è l'insieme di tutte le possibili modalità di $Y$.  ^b79f53

Le variabili si possono classificare nel seguente modo: ^01b594
### Variabili qualitative (categoriali)
se le modalità sono espresse in forma verbale. 
In particolare, si individuano: 
* **Variabili qualitative sconnesse (nominali)**, per le quali non è possibile individuare un ordinamento naturale delle modalità (ad esempio, "Genere", "Colore degli occhi", "Religione professata");  ^ebd89e
* **Variabili qualitative ordinali**, per le quali è invece possibile individuare un ordinamento naturale delle modalità (ad esempio, "Livello di istruzione").  ^58fcd8
### Variabili quantitative (numeriche)
se le modalità sono espresse in forma numerica (da non confondere con le codifiche numeriche).
In particolare, si individuano:
*  **Variabili quantitative discrete**, se $Y$ è un insieme finito o al più numerabile (ad esempio, "Età" in a.c., "Numero di figli");  ^a1fa07
* **Variabili quantitative continue**, se $Y$ è un insieme continuo (ad esempio, "Distanza", "Altezza", "Reddito"). 
	Si noti che la continuità va intesa come potenziale continuità o come opportuno riferimento semplificativo.
Se le modalità di una variabile qualitativa sono solo due, si parla di variabile dicotomica (binaria). ^3cc28d

Una variabile quantitativa può essere con **scala di intervalli**, se non esiste uno zero naturale e non arbitrario. 
Una variabile quantitativa è con **scala di rapporti** se invece esiste uno zero con tali caratteristiche.
Ad esempio, la variabile "Temperatura", in gradi centigradi, è su scala di intervalli poiché lo zero è convenzionale. 
Quindi, non ha senso affermare che la temperatura di 30°C è due volte più calda della temperatura di 15°C. 
La variabile "Reddito" invece è su scala di rapporti. In questo caso ha senso affermare che un reddito di 20000 euro è il doppio di un reddito di 10000 euro.

### Variabili statistiche

La variabile $Y$ viene rilevata su una popolazione (campione) costituita da n unità e si ottiene una successione di modalità osservate $(y_1, . . . , y_i, . . . , y_n)$, dove $y_i, i = 1, . . . , n$, è il valore assunto da $Y$ con riferimento all'unità i-esima. 

È utile distinguere tra variabile e risultato della sua rilevazione sulla popolazione (campione). Si definisce **variabile statistica** la rilevazione $(y_1, . . . , y_i, . . . , y_n)$ di una certa variabile Y su una determinata popolazione (campione).
È una colonna della matrice dei dati. La stessa variabile rilevata su popolazioni (campioni) diverse dà luogo, in genere, a variabili statistiche differenti. 
Si usa il simbolo $Y$ per indicare anche la variabile statistica.

Nel caso di dati (campioni) $y_1, . . . , y_i, . . . , y_n$ di tipo numerico può essere utile considerare l'insieme dei dati (campione) ordinato $y(1), . . . , y(i), . . . , y(n)$, ottenuto disponendo le osservazioni in ordine non decrescente.

Il valore che occupa la posizione i-esima, $y_{(i)}$, si dice avere rango $i, i = 1, . . . , n$. Si noti che il minimo e il massimo corrispondono rispettivamente a $y_{(1)} = min(y1_, . . . , y_n)$ e $y_{(n)} = max(y_1, . . . , y_n)$. 
Non tutte le modalità potenzialmente assumibili dalla variabile $Y$ possono venire effettivamente rilevate in una popolazione (campione).

### Supporto di una variabile

Il **supporto** di una variabile statistica $Y$, indicato con $S_Y$ , è l'insieme delle modalità di $Y$ effettivamente osservate nella popolazione (campione); 
$S_Y = {y_1, . . . , y_j , . . . , y_J }$. 
Si noti che $J \le n$. 
Le modalità osservate, che concorrono a costituire $S_Y$, sono tra loro distinte, cioè vanno prese una volta sola anche se ripetute. 
Nel caso di variabili qualitative ordinali e quantitative si suppone che le modalità appartenenti al supporto vengano ordinate secondo un ordine crescente: $y_1 \lt y_2 \lt ... \lt y_J$ ^3cd569

>[!example] **Esempio**
>Con riferimento alla seguente matrice di dati:
>
| Unità | Genere | Età | Livistr | Dist |
| ---- | ---- | ---- | ---- | ---- |
| Andrea | M | 28 | 3 | 5.0 |
| Claudio | M | 17 | 2 | 7.5 |
| Lucia | F | 20 | 3 | 12.0 |
| Giuseppe | M | 32 | 4 | 3.2 |
| Mara | F | 16 | 2 | NA |
| Luca | M | 34 | 4 | 12.3 |
| Aldo | M | 18 | 3 |  25.0 |
| Arianna | F | 25 | 3 | 7.7 |
>^793ba3
>
Alla variabile $Y$ = "Età" corrisponde la variabile statistica
$Y = (28, 17, 20, 32, 16, 34, 18, 25)$ con $n=8$.
>
Con riferimento alla variabile $Y$ = "Età" il supporto è $S_Y = \{16, 17, 18, 20, 25, 28, 32, 34\}$ mentre $Y = \{0, 1, 2, ...\}$.

### Variabili Statistiche Standardizzate
Una **variabile statistica** con **[[Media Aritmetica|media]] nulla** e **[[Varianza|varianza]] unitaria** è detta **standardizzata**.

Dalle proprietà della media e della varianza si conclude
* che data una variabile $Y$ , allora $Z = (Y − \mu_Y) / \sigma_Y$ è una variabile standardizzata; 
* data una variabile $Z$ standardizzata, allora la variabile $Y = \sigma Z + \mu$ è tale che $E(Y) = \mu$ e $V(Y) = \sigma^2$. 
A volte è utile trasformare i dati $y_1, . . . , y_n$ in modo tale che i dati trasformati $z_1, . . . , z_n$ abbiamo media nulla e varianza unitaria. La trasformazione appropriata è $z_i = (y_i − μ_Y)/\sigma_Y,\ i = 1, . . . , n$. 

Con la standardizzazione dei dati possono emergere più chiaramente alcune ulteriori caratteristiche della distribuzione di frequenza, oltre la posizione e la variabilità.

La standardizzazione è utile anche per confrontare e analizzare più insiemi di dati, tenendo conto che possono avere con unità di misura e livello medio diversi.

***
Riferimenti:
[[2_Statdescr_Univ_L2.pdf#page=6&annotation=97R|2_Statdescr_Univ_L2, pagina 6]]
[[2_Statdescr_Univ_L2.pdf#page=111&selection=10,0,25,0|2_Statdescr_Univ_L2, pagina 111]]
[[OpenIntro Statistics.pdf#page=15&selection=6,0,8,18|Pagina OpenIntro Statistics]]

#statistica_descrittiva
#statistica_descrittiva/analisi_univariate
#ppt-2
#variabili 