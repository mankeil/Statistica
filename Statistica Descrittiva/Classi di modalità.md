> [!Summary]+ Sommario
> Una classe di modalità è un raggruppamento di valori o modalità in un intervallo specifico. Ogni classe, quindi. rappresenta un intervallo di valori.
> In genere, le classi sono definite in modo da essere disgiunte, coprire tutte le possibili modalità e garantire un'organizzazione chiara dei dati.
> Una regola comune per avere classi di uguale ampiezza è individuare $\sqrt{n}$ classi.

Se la variabile statistica è [[Variabili#^3cc28d|quantitativa continua]], si osservano, a meno di effetti di arrotondamento(approssimazioni etc...), tante modalità distinte quante sono le unità statistiche:
$S_Y$ corrisponde all'insieme dei dati grezzi e $f_j = 1, j = 1, . . . , J$.
Questo può accadere, in alcuni casi, anche con [[Variabili#^a1fa07|variabili statistiche quantitative discrete]].

È conveniente definire classi di modalità contigue e contare le unità che appartengono a ciascuna classe. 
Le classi vanno definite di modo che: non siano né troppe né troppo poche; siano disgiunte; comprendano tutte le modalità osservate.

La regola di individuare un numero di classi (di uguale ampiezza) pari a $\sqrt{n}$ in molti casi va bene. Talvolta è necessario fare qualche aggiustamento o utilizzare regole più sofisticate.

Le classi non hanno necessariamente un'ampiezza costante.

Si ottiene una tabella (distribuzione) di frequenza assoluta con modalità raggruppate in classi

| Classi | $y_0 \vdash y_1 \cdots y_{j-1} \vdash y_j \cdots y_{J-1} \vdash y_J$ | Totale |
| ---- | ---- | ---- |
| Frequenza | $f_1 \cdots f_j \cdots f_J$ | $\sum^J_{j=1}f_j$ |
dove $f_j$ è la frequenza assoluta associata alla classe $y_{j−1} \dashv y_j$ , che corrisponde all'intervallo $(y_{j−1}, y_j]$.[^1] 
Analogamente, $y_{j−1} \vdash y_j$ corrisponde all'intervallo $[y_{j−1}, y_j )$ e $y_J -$ indica $(y_J , +\infty)$.
Una tabella di frequenza così ottenuta è detta seriazione statistica. 

>[!example] **Esempio:** 
Con riferimento alla [[Variabili#^793ba3|matrice vista in precedenza]], si ricava la seguente seriazione statistica associata alla variabile "Distanza":
>
| Dist | frequenza |
| ---- | ---- |
| $0 \vdash 5$ | 2 |
| $5 \vdash 15$ | 4 |
| $15-$ | 1 |
| **Totale** | 7 |
[^1]: [ ] si pone quando l'estremo dell'intervallo accanto ad essa è compreso nell'intervallo, mentre la ( ) quando l'estremo non è compreso.

#statistica_descrittiva 
#analisi_univariate
#ppt-2 
#frequenze 
#variabili