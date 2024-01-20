>[!Summary]+ Sommario
>L'**indice di connessione** ($\chi^2$) misura quanto le frequenze osservate in una [[tabella di contingenza]] si discostino da quelle attese in caso di [[indipendenza statistica|indipendenza]] tra due variabili. $\chi^2 = 0$ indica indipendenza completa, valori più alti suggeriscono una connessione tra le variabili. 
>L'indice **normalizzato**, può avere valori compresi tra 0 e 1, quantifica la forza della dipendenza: 0 implica indipendenza, 1 dipendenza completa.
>%% > [!formula]-
>>   $$\begin{gather} \chi^2 = \sum^m_{r=1} \sum^k_{s=1} \frac{(n_{rs}-n^*_{rs})^2}{n^*_{rs}},\ \ n^*_{rs} = \frac{n_{r+}n_{+s}}{n} \\ \chi_{\text{norm}} = \frac{\chi^2}{n \cdot min(m - 1,\ k-1)} \end{gather} $$ %%

La *distanza* fra le frequenze osservate in una [[tabella di contingenza]] e le frequenze attese nel caso di [[Indipendenza statistica|indipendenza]] è misurata dall'**indice di connessione** $\chi^2$ $$\chi^2 = \sum^m_{r=1} \sum^k_{s=1} \frac{(n_{rs}-n^*_{rs})^2}{n^*_{rs}},\ \ n^*_{rs} = \frac{n_{r+}n_{+s}}{n}$$ dove $n^*_{rs} = (n_{r+}n_{+s})/n$ è la frequenza attesa nel caso di indipendenza.

L'indice $\chi^2$ vale 0 quando tutte le frequenze osservate coincidono con quelle attese, e quindi vi è **indipendenza fra le due variabili**.

Viceversa, tanto maggiori sono i valori osservati di $\chi^2$, tanto più le due **variabili** saranno **connesse** (**[[Studio della Dipendenza|statisticamente dipendenti]]**). 
Il valore massimo dell'indice è $n \cdot \text{min}(m-1,\ k-1)$. 
I valori $m$ e $k$ indicano, rispettivamente, il numero di righe e di colonne della tabella di contingenza.

Per valutare la forza dell'eventuale dipendenza tra $X$ e $Y$ si può determinare l'**indice $\chi^2$ normalizzato**, che si ottiene dividendo l'indice assoluto per il suo massimo.
$$ \frac{\chi^2}{n \cdot min(m - 1,\ k-1)} $$
Quindi si ottiene una quantità che assume valori nell'intervallo $[0, 1]$. Se vale 0 le variabili sono statisticamente indipendenti, se vale 1 si ha dipendenza statistica piena tra $X$ e $Y$.

>[!example] **Esempio**
>*Attitudine* (continua). Con riferimento alla analisi delle attitudini musicale e pittorica, se ci fosse indipendenza tra le due, ferme restanti le distribuzioni marginali, si avrebbe la seguente tabella di contingenza
>![[Pasted image 20240117214322.png]]
>Considerando la tabella di contingenza originale:
>![[Pasted image 20240117020209.png]]
>Si può calcolare facilmente l'indice $\chi^2$ che è pari a 3.527.
> Quindi, si può dunque escludere l'indipendenza tra attitudine musicale e pittorica.
Dal momento che tale valore è lontano dal valore massimo $15 \cdot (3-1) = 30$, ed inoltre l'indice normalizzato vale 0.117, si conclude che i dati indicano una moderata connessione (dipendenza) tra le due variabili.

>[!example] **Esempio**
>*Casco*. La seguente tabella di contingenza illustra i risultati di uno studio sull'efficacia dei caschi protettivi per ciclisti nella prevenzione dei traumi cranici. Si considerano $n=793$ soggetti coinvolti in incidenti.
>![[Pasted image 20240117214733.png]]
>Se ci fosse indipendenza tra uso del casco e trauma cranico, ferme restanti marginali, si avrebbe la seguente tabella di contingenza
>![[Pasted image 20240117214824.png]]
>Confrontando le due tabelle si calcola facilmente l'indice di connessione $\chi^2$ che vale 28.26.
>
>Dal momento che il suo valore massimo è $793 \cdot (2-1) = 793$ e l'indice normalizzato è $28.26/793 = 0.036$, si conclude che esiste una lieve relazione tra le due variabili in esame.

***
Riferimenti:
[[3_Statdescr_Multiv_L3.pdf#page=20&selection=10,0,10,21|3_Statdescr_Multiv_L3, page 20]]

#statistica_descrittiva 
#statistica_descrittiva/analisi_multivariate 
#ppt-3 
#dipendenza 