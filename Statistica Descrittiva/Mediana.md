La mediana si può calcolare per una variabile [[Variabili#^58fcd8|qualitativa ordinale]] o [[Variabili#Variabili quantitative (numeriche)|quantitativa]] $Y$ e si indica con $y_{0.5}$. È quel valore che, rispetto all'ordinamento non decrescente delle osservazioni, le divide in due parti uguali. È il valore centrale.

La mediana corrisponde a ogni valore $y_{0.5}$ tale che:
* almeno il 50% delle unità statistiche presenta [[modalità]] inferiori o pari a $y_{0.5}$;
* almeno il 50% delle unità statistiche presenta modalità superiori o pari a $y_{0.5}$

Se si dispone dei dati grezzi $y_1, ..., y_n$ ordinati secondo un ordinamento non decrescente, allora la mediana di $y_{0.5}$ corrisponde
* alla modalità che si trova nella ==posizione $(n+1)/2$ se $n$ è **dispari**==, cioè $y_{0.5} = y_{(n+1)/2}$
* alle modalità che si trovano nelle ==posizioni $n/2$ e $\frac{n}{2}+1$ se, se $n$ è **pari**==, cioè $y_{0.5} = y_{n/2}$ e $y_{0.5} = y_{n/2+1}$

![[Pasted image 20240113233018.png]]

Se $y_{n/2}$ e $y_{n/2+1}$ non coincidono, la mediana può non essere unica.

Nel caso di variabili quantitative con $n$ pari, si può avere anche un intervallo di valori $[y_{n/2},\ y_{(n/2+1)}]$ che soddisfano la definizione di mediana. In questo caso di può prendere il punto di mezzo come **mediana convenzionale**.

>[!example] **Esempio**
>*Voti.* Si consideri la variabile statistica qualitativa ordinale Y che descrive il voto di $n = 5$ studenti, $$Y = (\text{sufficiente, sufficiente, buono, buono, ottimo})$$ Poiché $n$ è dispari, $y_{0.5} = y_{(n+1)/2} = y_3 = \text{buono}$
>Se invece $$Y = (\text{sufficiente, sufficiente, sufficiente, buono, buono, ottimo})$$ $n$ è pari, quindi $y_{0.5} = y_{n/2} = y_3 = \text{sufficiente}$ e $y_{0.5} = y_{(n/2)+1} = y_4 = \text{buono}$.
>Infine, se $$Y = (\text{sufficiente, sufficiente, buono, buono, ottimo, ottimo})$$ $n$ è pari, ma $y_{0.5} = y_{n/2} = y_3 = \text{buono}$ e $y_0.5 = y_{n/2+1} = y_4 = \text{buono}$, quindi "buono" è l'unica mediana. 
 
Se si dispone soltanto della distribuzione di [[Frequenze Relative|frequenza relativa]] o [[Frequenze Assolute|assoluta]], si può operare nel seguente modo.

Si suppone che le modalità del supporto $S_Y = \{y_1, . . . , y_J\}$ siano ordinate in senso crescente.

Se sono note le **frequenze assolute** $f_j,\ j = 1, . . . , J$, e quindi la dimensione $n$ della popolazione, la mediana corrisponde:
* se $n$ è **dispari**, alla modalità $y_j$ che presenta la [[Frequenze Cumulate|frequenza assoluta cumulata]] $F_j$ più piccola tale che $F_j \ge (n + 1)/2$;
* se n è **pari**, alla modalità $y_j$ che presenta la frequenza assoluta cumulata $F_j$ più piccola tale che $F_j ≥ n/2$ e alla modalità $y_j$ che presenta la frequenza assoluta cumulata $F_j$ più piccola tale che $F_j \ge (n/2) + 1$.

Nel caso con $n$ pari si possono avere due valori mediani distinti o più di due, se si considerano variabili quantitative.

Se sono note solo le **frequenze relative** $p_j,\ j = 1, . . . , J$, e quindi la dimensione $n$ della popolazione non risulta nota, allora la mediana corrisponde alla modalità $y_j$ che presenta frequenza relativa cumulata più piccola tale che $P_j \ge 0.5$.

Se esiste una modalità $y_j$ tale che $P_j = 0.5$, allora sia $y_j$ che $y_j+1$ soddisfano la definizione di mediana.

Per l'individuazione della mediana è utile, in questo contesto, l'analisi della funzione di ripartizione empirica, con particolare riferimento al livello 0.5.

La mediana è un indice di posizione robusto rispetto a valori anomali dei dati.

Se si dispone soltanto della **distribuzione di frequenza relativa o assoluta con modalità raggruppate in classi**, si può operare allo stesso modo. 

Quindi, si individuerà una **classe mediana**.

>[!example] **Esempio**
Sia $Y$ la variabile quantitativa discreta che descrive il numero di componenti delle famiglie residenti in Liguria alla data del Censimento 1981. Si riporta la associata tabella di frequenza.
>
| No. componenti | $f$ | $F$ | $p$ | $P$ |
| ---- | ---- | ---- | ---- | ---- |
| 1 | 197906 | 197906 | 0.272 | 0.272 |
| 2 | 203709 | 401615 | 0.281 | 0.553 |
| 3 | 168536 | 570151 | 0.232 | 0.785 |
| 4 | 117509 | 687660 | 0.162 | 0.947 |
| 5 | 29727 | 717387 | 0.041 | 0.988 |
| 6 | 6577 | 723964 | 0.009 | 0.997 |
| 7 | 1707 | 725671 | 0.002 | 0.999 |
| 8 o più | 906 | 726577 | 0.001 | 1 |
| **Totale** | 726577 |  | 1 |  |
Poiché $n = 726577$ è dispari, la mediana è unica e corrisponde alla modalità della famiglia che si trova nella posizione $(n + 1)/2 = 363289$, dopo avere ordinato le famiglie secondo il numero crescente di componenti. Quindi $y_{0.5} = 2$.
>
Si noti che a 2 corrisponde la frequenza assoluta cumulata più piccola che risulta maggiore o uguale a $(n+1)/2=363289$.
>
Se si prendono in esame le frequenze relative cumulate, $y_{0.5} = 2$ è la modalità che presenta frequenza relativa cumulata più piccola tale che $P_j \ge 0.5$
>
Si consideri la tabella di frequenza riferita alla regione Campania
>
| No. componenti | $f$ | $F$ | $p$ | $P$ |
| ---- | ---- | ---- | ---- | ---- |
| 1 | 225641 | 225641 | 0.144 | 0.144 |
| 2 | 304325 | 529966 | 0.194 | 0.338 |
| 3 | 278879 | 808845 | 0.178 | 0.516 |
| 4 | 355488 | 1164333 | 0.226 | 0.742 |
| 5 | 228494 | 1392827 | 0.146 | 0.888 |
| 6 | 98924 | 1491751 | 0.063 | 0.951 |
| 7 | 42894 | 1534645 | 0.027 | 0.978 |
| 8 o più | 34999 | 1569644 | 0.022 | 1 |
| **Totale** | 1569644 |  | 1 |  |
Poiché $n=1569644$ è pari, la mediana corrisponde alla modalità della famiglia che si trova nella posizione $n/2 = 784822$ e alla modalità della famiglia che si trova nella posizione $(n/2)+1 = 784823$, dopo avere ordinato le famiglie secondo il numero crescente di componenti.
>
Tali famiglie presentano la stessa modalità 3, quindi $y_{0.5} = 3$.
>
Si noti che a 3 corrisponde la frequenza assoluta cumulata più piccola che risulta maggiore o uguale sia a $n/2 = 784822$ che a $(n/2)+1 = 784823$.
>
Se si considerano le frequenze relative cumulate, $y_{0.5}=3$ è la modalità che presenta frequenza relativa cumulata più piccola tale che $P_j \ge 0.5$

***
[[2_Statdescr_Univ_L2.pdf#page=70&selection=4,6,10,28|Lucido]]

#statistica_descrittiva 
#analisi_univariate
#ppt-2 
#indici_sintetici 
#indici_di_posizione