Gli **istogrammi** si utilizzano per rappresentare **distribuzioni di [[Frequenze Assolute|frequenza assoluta]] o [[Frequenze Relative|relativa]]** con [[modalità]] raggruppate in [[Classi di modalità|classi]], riferite usualmente a dati [[Variabili#^3cc28d|quantitativi continui]]. 

L'istogramma è un insieme di rettangoli adiacenti, ognuno rappresentativo di una classe, posti su un piano cartesiano. 

Il rettangolo corrispondente alla classe $j-esima$ $y_{j−1} \vdash y_j,\ j = 1, . . . , J$, ha come base l'intervallo $[y_{j−1}, y_j]$ e
* altezza (e quindi area) proporzionale a, oppure pari a, $f_j / (y_j − y_{j−1})$: **istogramma delle frequenze assolute**;
* altezza (e quindi area) proporzionale a, oppure pari a, $p_j /(y_j − y_{j−1})$: **istogramma delle frequenze relative**. 
Se i rettangoli hanno la stessa base, allora l'altezza è proporzionale a $f_j$ o a $p_j$.

Se le classi sono estreme sono aperte, ad esempio, $-y_1$ e $y_{J-1}-$, vanno chiuse scegliendo opportunamente gli estremi $y_0$ e $y_J$.

Se si considerano altezze pari a $p_j/(y_j - y_{j-1})$, la somma delle aree dei rettangoli è pari a **1**.

L'istogramma può essere utilizzato anche per descrivere distribuzioni di frequenza associate a **[[Variabili#^a1fa07|variabili quantitative discrete]]**, quando si hanno molte modalità osservate distinte.

>[!example] **Esempio**
>*Reddito*. Si consideri la seguente seriazione riferita alla variabile reddito (lordo mensile in migliaia di euro)
>
| Reddito | $1.5 \dashv 2.5$ | $2.5 \dashv 3.5$ | $3.5 \dashv 4.5$ | $4.5 \dashv 6.5$ | Tot. |
| ---- | ---- | ---- | ---- | ---- | ---- |
| freq. rel. | 0.2 | 0.3 | 0.4 | 0.1 | 1 |
L'associato istogramma delle frequenze relative corrisponde a ![[Pasted image 20240116015639.png]]

^11a7f6

>[!example] **Esempio**
>*Colesterolo*([[Frequenze Assolute#^0d78d1|continua]]). Considerando i dati sul livello di colesterolo sierico, si ottengono i seguenti istogrammi riferiti, rispettivamente, ai pazienti di età 25-34 anni e di età 55-64 anni.
>![[Pasted image 20240116020050.png]]
>I grafici sono basati sulle **frequenze relative** e suggeriscono le stesse conclusioni fatte sulla base delle tabelle di frequenza. La distribuzione di frequenza relativa dei pazienti più anziani è spostata più a destra rispetto a quella dei pazienti giovani.

***
Riferimenti:
[[2_Statdescr_Univ_L2.pdf#page=41&selection=10,0,10,10|2_Statdescr_Univ_L2, pagina 41]]

#statistica_descrittiva 
#statistica_descrittiva/analisi_univariate
#ppt-2 
#grafici