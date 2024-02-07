Il modello lineare è utile solo nel caso di relazioni sostanzialmente lineari tra $Y$ e $X$.
Con l'obiettivo di **valutare la bontà del modello** di regressione, si vuole individuare un indice in grado di valutare l'adattamento globale del modello ai dati, oltre che la sua capacità esplicativa per il fenomeno $Y$.

La [[Statistica Descrittiva/Varianza|varianza]] $V(Y)$ associata alla variabile statistica $Y$ (**varianza totale**) può essere vista come somma della quota $V(\hat Y)$ descritta dal modello (**varianza spiegata**) e dalla quota $V (\hat \epsilon)$ rimanente (**varianza residua**) $$V(Y) = V(\hat Y)+V(\hat \epsilon)$$ dove $\hat Y$ e $\hat \epsilon$ sono, rispettivamente, i valori stimati dal modello e i residui stimati.

Tanto maggiore è la varianza spiegata dal modello, tanto migliore sarà l'adattamento dei dati al modello teorico.

Un indice di bontà di adattamento del modello lineare è dato dal **coefficiente di determinazione** $R^2$, che corrisponde alla proporzione di varianza di $Y$ spiegata dal modello di regressione $$\begin{gather} R^2 = \frac{\sum_i(\hat y_i - E(\hat Y))^2 / n}{\sum_i(y_i-E(Y))^2/n} = 1 - \frac{\text{varianza spiegata}}{\text{varianza totale}} = \\ 
= \frac{\sum_i(\hat \epsilon_i - E(\hat \epsilon))^2 / n}{\sum_i(y_i-E(Y))^2/n} = 1 - \frac{\text{varianza residua}}{\text{varianza totale}} \end{gather}$$dove $E(\hat Y) = E(Y)$ è la [[Media Aritmetica|media]] dei valori stimati dal modello e $E(\hat \epsilon) = 0$ è la media dei residui stimati.

Vale che $0 \le R^2 \le 1$ e un valore per $R^2$ vicino a 1 indica un buon adattamento del modello dei dati, e viceversa un $R^2$ vicino a 0 indica un pessimo adattamento del modello ai dati.

Si dimostra inoltre che la seguente relazione con l'[[Coefficiente di Correlazione Lineare|indice di correlazione lineare]] $$R^2 = \rho^2_{XY}$$
Nel caso di modelli con $a=0$, l'indie $R^2$ va modificato opportunamente.

>[!example] **Esempio**
>*Molla* ([[Studio della Dipendenza#^7dbcdc|continua]]). Con riferimento ai dati sulla lunghezza della molla e sui pesi, dal momento che $\rho_{XY} = 0.97$, si conclude che $R^2 = 0.97^2 = 0.9409$. Quindi il modello di regressione presenta una elevata capacità esplicativa per il fenomeno in esame.

Un adattamento poco soddisfacente della retta di regressione ai dati può essere migliorato ricorrendo ad un **cambiamento di scala** della della variabile risposta e/o della variabile esplicativa.

Le trasformazione più comuni sono $log(Y), \sqrt{Y}$ e $1/Y$.

In alcuni casi, un cattivo adattamento può essere dovuto alla presenza di **valori anomali**, riconducibili a errori di misurazione o ad unità con caratteristiche particolari.

Dopo aver individuato (tipicamente per via grafica) le osservazioni potenzialmente anomale si prova a ripetere l'analisi di regressione senza tali valori.

Infine, un adattamento non ottimale può essere spiegato dal fatto che la componente d'errore del modello risulta essere elevata.

>[!example] **Esempio**
>**Velocità** ([[Diagramma di Dispersione#^cc968a|continua]]). Con riferimento ai dati sulla velocità e spazio di frenata, si ottiene $R^2 = 0.651$. È possibile migliorare l'adattemento della retta di regressione considerando $\sqrt{Y}$ come risposta.
>![[Pasted image 20240121021139.png]]
>Nel grafico di sinistra si riportano i dai osservati $(\sqrt{y_i}, x_i),\ i=1,...,n$, e la <span style="color: red">retta di regressione stimata</span> $\sqrt{y} = 1.227 + 0.332x$. L'adattemento sembra migliorato, infatti $R^2 = 0.709$.
>
>Nel grafico di destra si ha la rappresentazione sulla scala originaria (la retta di regressione diventa una parabola).

***
Riferimenti:
[[Lucidi & materiale/3_Statdescr_Multiv_L3.pdf#page=47&selection=10,0,10,28|3_Statdescr_Multiv_L3, page 47]]

#statistica_descrittiva 
#statistica_descrittiva/analisi_multivariate 
#ppt-3 
#regressione