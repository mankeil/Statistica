I *coefficienti di regressione* sono noti; sono parametri da *stimare sulla base dei dati osservarti*, in modo che la retta di regressione si adatti bene alle osservazioni.

Avendo osservato $n$ coppie di valori $(y_i, x_i),\ i=1,...,n$, si hanno $n$ valori osservati anche per l'errore di regressione $$ \epsilon_i = y_i - (a + bx_i),\ i = 1,...,n $$ I valori $\epsilon_i,\ 1,...,n$, detti **residui di regressione**, rappresentano gli scostamenti fra le osservazioni e il modello teorico.

Per stimare i coefficienti di regressione può essere ragionevole cercare i valori per $a$ e $b$ che minimizzano (non è l'unica possibilità) la **somma dei quadrati dei residui** $$ Q(a,b) = \sum^n_{i=1} \epsilon^2_i = \sum^n_{i=1} (y_i - a - bx_i)^2 $$ Il metodo presentato è detto **metodo dei minimi quadrati** e le stime ottenute, indicate con $$\hat a = E(Y) - \hat b E(X),\ \hat b = \frac{Cov(X,Y)}{V(X)} $$
dove $E(Y)$ è la [[media aritmetica]] di $Y$, e $V(X)$ la [[varianza]] di $X$.

La retta $y = \hat a + \hat bx$ è detta **regressione stimata** (**retta dei minimi quadrati**).

>[!example] **Esempio**
>*Molla* ([[Studio della Dipendenza#^7dbcdc|continua]]). Con riferimento ai dati sulla lunghezza della molla e sui diversi pesi a cui viene sottoposta, si ottengono le seguenti stime per i coefficienti di regressione $$ \hat b = 0.27215/1.33 = 0.2046,\ \hat a = 5.3885 - 0.2046 \cdot 1.9 = 4.9997 $$ Nel grafico seguente si riposta, oltre ai dati osservati, la retta di <span style="color: red">retta di regressione stimata</span> $y=4.9997 + 0.2046x$ e i <span style="color: dodgerblue"> residui stimati </span> $\epsilon_i,\ i=1,...,20$.
>![[Pasted image 20240119003402.png]]
>Dall'analisi della retta di regressione stimata si conclude che:
>* con un peso di 2.5 Kg, si potrebbe prevedere un allungamento della molla pari a $4.9997 - 0.2046 \cdot 2.5 = 5.51$;
>* con un peso di 7.5 Kg, si potrebbe prevedere (facendo un'estrapolazione) un allungamento della molla pari a $4.9997 - 0.2046 \cdot 7.5 = 6.53$ (che forse è non è un valore realistico)

>[!example] **Esempio**
>*Velocità* ([[Diagramma di Dispersione#^cc968a|continua]]). Con riferimento ai dati sulla velocità e spazio di frenata, si ottengono le seguenti stime per i coefficienti di regressione $\hat a = -17.579,\ \hat b = 3.932.$
>![[Pasted image 20240119004104.png]]
>Nel grafico si riportano i dati osservati e la <span  style="color:red">retta di regressione stimata</span> $y = −17.579 + 3.932 x$. 

Tra l'**analisi di regressione** e l'**analisi di correlazione** ci sono differenze e punti di contatto.
* Nella correlazione, c'è **[[simmetria]]** tra le due variabili, mentre nella regressione c'è **asimmetria**: si suppone di fissare i valori $x_i$ per vedere come variano i valori $y_i,\ i = 1,...,n$.
* Nella regressione si opera come se i valori $x_i,\ i=1,...,n$, fossero fissati a priori e ottenuti senza errore (anche se nella pratica a volte i valori di $X$ e $Y$ sono generati simultaneamente).
* Il coefficiente angolare stimato della retta di regressione $\hat b$ è direttamente proporzionale al coefficiente di correlazione lineare $\rho_{XY}$. Infatti, $$ \hat b \frac{Cov(X,Y)}{V(X)} = \rho_{XY} \frac{\sigma_Y}{\sigma_X} $$ dove $\sigma_X$ è lo [[scarto quartilico medio]] di $X$.

***
Riferimenti:
[[Lucidi & materiale/3_Statdescr_Multiv_L3.pdf#page=41&selection=10,0,10,26|3_Statdescr_Multiv_L3, page 41]]

#statistica_descrittiva 
#statistica_descrittiva/analisi_multivariate 
#ppt-3 
#correlazione 