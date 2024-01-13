>[!Summary]+ Sommario
>Il numero di volte che una specifica [[modalità]] o [[Classi di modalità|classe di modalità]] appare in un insieme di dati.
>Si indicano con $f_j$​, dove $j$ rappresenta la modalità.
I dati grezzi (la variabile statistica), pur rappresentando pienamente il contenuto dell'osservazione, usualmente non permettono di cogliere in modo chiaro le caratteristiche del fenomeno in esame. 

È utile passare dai dati in forma grezza ad una tabella di frequenza che fornisca una sintesi dei dati in un formato facile da capire.

Esempio. _Colesterolo_. Si è misurato il livello di colesterolo sierico a n soggetti maschi, discriminando i pazienti in due classi di età: 25-34 anni e 55-64 anni. Ci si chiede se il livello di colesterolo sia maggiore negli adulti piuttosto che nei giovani.

I dati rilevati sono troppi per cercare di ricavare informazioni utili solamente guardandoli.
È necessario operare una sintesi. Definire una tabella dove si considerano le frequenze con cui le diverse modalità, o classi di modalità, sono state osservate.

Se $y_j \in S_Y, j = 1, ..., J$, è una delle modalità osservate di $Y$, si dice **frequenza assoluta** di $y_j$ il numero di volte che $y_j$ risulta osservata.
Si indica con $f_j$. 
Evidentemente, $f_j \gt 0, j=1,...,J$[^1], e $\sum^J_{j=1} f_j=n$[^2] 

La lista delle modalità osservate accompagnate dalle rispettive frequenze assolute è detta distribuzione di frequenza assoluta e si rappresenta con una tabella di frequenza del tipo

| Modalità | $y_1 \cdots y_j \cdots y_J$ | Totale |
| ---- | ---- | ---- |
| Frequenza | $f_1 \cdots f_j \cdots f_J$ | $\sum^J_{j=1}f_j$ |

>[!example] **Esempio:**
facendo rifermento alla [[Variabili#^793ba3|matrice vista in precedenza]]:
>
| Liv. di istruz. | frequenza |
| ---- | ---- |
| Scuola obbligo | 2 |
| Diploma superiore | 4 |
| Laurea o superiore | 2 |
| Totale | 8 |
Una tabella di frequenza riferita ad una variabile statistica qualitativa è detta **serie statistica**.
%%Footnotes:%%

[^1]: La sintassi: $j = 1,...,J$ significa che $j$ può assumere qualsiasi valore da 1 a $J$.
[^2]: In parole più semplici, significa che si somma tutte le frequenze assolute per ogni modalità della variabile $Y$, si otterrà il totale delle osservazioni $n$.

Riferimenti:
[[2_Statdescr_Univ_L2.pdf#page=17&selection=6,4,10,18|Lucido]]

#statistica_descrittiva 
#analisi_univariate
#ppt-2 
#frequenze 