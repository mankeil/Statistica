Si considerano due variabili $X$ e $Y$. La loro osservazione su $n$ unità statistiche fornisce i dati grezzi $(x_i, y_i),\ i=1,...,n$.

A partire dai dati grezzi si possono determinare le distribuzioni di [[Frequenze Assolute|frequenza assoluta]] e [[Frequenze Relative|relativa]] che si possono distinguere in:
* **distribuzione congiunta**, se si considerano le frequenze delle unità che presentano congiuntamente la [[modalità]] $x_r,\ r=1,...,m$ della prima variabile e la modalità $y_s,\ s=1,...,k$, della seconda.
* **distribuzione marginale**, se si considera la distribuzione di frequenza relativa ad una singola variabile.
* **distribuzione condizionata**, se si considera la distribuzione di frequenza relativa ad una singola variabile considerando soltanto le unità statistiche che assumono una determinata modalità dell'altra.

Si può operare allo stesso modo anche se si hanno modalità [[Classi di modalità|raggruppate in classi]].

Una tabella di frequenza è di fatto una distribuzione doppia di frequenza.
Inoltre, risulta utile per indagare le relazioni esistenti tra le modalità delle due variabili.

Dalla [[Tabella di Contingenza]] si ricavano le seguenti **distribuzioni di frequenza assoluta**
* **congiunta**: $(x_r,y_s),\ n_{rs},\ r=1,...,m,\ s=1,...,k;$
* **marginale di** $X$: $x_r, n_{r+}, r=1,...,m;$
* **marginale di** $Y$: $y_s, n_{+s},\ s=1,...,k$;
* **condizionata di** $X$ **dato** $Y = y_s$: $x_r,\ n_{rs},\ r = 1,...,k$
* **condizionata di** $Y$ **dato** $X = x_r$: $y_s, n_{rs}, s = 1,...,m$.
Le frequenze marginali di $X$ e di $Y$ corrispondono, rispettivamente, ai totali di riga e colonna.

Le frequenze condizionate di $X$ e di $Y$ corrispondono, rispettivamente, ai valori di colonna e di riga individuati dalle condizioni $Y = y_s$ e $X=x_r$.

Le **distribuzioni di frequenza relativa** si ottengono dividendo per i corrispondenti totali. In particolare, le distribuzioni congiunta e marginali si dividono per $n$, le distribuzioni condizionate per i totali di riga o colonna corrispondenti alla condizione. ^3f15a9

>[!example] **Esempio**
>*Attitudine*([[Studio della Dipendenza#^752de4|continua]]). Con riferimento alla analisi delle attitudini musicale e pittorica, si ottengono le seguenti distribuzioni di frequenza marginale assoluta e relativa
>![[Pasted image 20240117022315.png]]
>e le seguenti distribuzioni di frequenza condizionata, assoluta e relativa, di $Y$ dato $X = x_r$
>![[Pasted image 20240117022457.png]]
>In modo analogo si ottengono le distribuzioni di frequenza condizionata e relativa, di $X$ dato $Y=y_s$.

## Rappresentazioni Grafiche

Oltre all'analisi delle distribuzioni di frequenza, risultano molto utili le **rappresentazioni grafiche**. 

Tenendo conto della tipologia della variabili, dei dati a disposizione e degli obiettivi dell'analisi, si possono utilizzare i [[Rappresentazioni grafiche - Introduzione|diagrammi]] visti in precedenza o loro opportune estensioni tridimensionali.

Se si dispone dei **dati grezzi**, riferiti a due [[Variabili#Variabili quantitative (numeriche)|variabili quantitative]], si può disegnare un **[[Diagramma di Dispersione|grafico di dispersione]]** (**scatterplot**), dove le coppie $(x_i, y_i), i = 1, . . . , n$, sono rappresentate come punti del piano, i cui assi corrispondono alle due variabili.

Per rappresentare una **distribuzione di frequenza congiunta** di due variabili quantitative si possono utilizzare **[[Istogramma|istogrammi]] o [[Diagramma a Bastoncini|diagrammi a bastoncini]]**, disegnati **in uno spazio tridimensionale**.

Per rappresentare una distribuzione di **frequenza marginale o condizionata** si possono utilizzare tutte le rappresentazioni grafiche viste per il caso univariato: istogrammi, [[boxplot]], diagrammi a bastoncini, [[Diagramma a Barre|a rettangoli]], [[Diagramma Circolare|a torta]], etc.
***
Riferimenti:
[[3_Statdescr_Multiv_L3.pdf#page=5&selection=10,0,10,26|3_Statdescr_Multiv_L3, page 5]]
[[3_Statdescr_Multiv_L3.pdf#page=15&selection=10,0,10,26|3_Statdescr_Multiv_L3, page 15]]

#statistica_descrittiva 
#statistica_descrittiva/analisi_multivariate 
#ppt-3 
#frequenze 