Vale la **diseguaglianza di Cauchy-Schwarz**: $$ -\sigma_X \sigma_Y \le \sigma_{XY} \le \sigma_X \sigma_Y$$ Una misura normalizzata della [[Studio della Dipendenza|dipendenza lineare]] è il coefficiente di correlazione lineare definito da $$\rho_{XY} = Cor(X, Y) = \frac{\sigma_{XY}}{\sigma_{X}\sigma_{Y}}$$dove $\sigma_{XY}$ è la [[covarianza]] tra $X$ e $Y$, e $\sigma_X$ il rispettivo [[scarto quartilico medio]].
Dalla diseguaglianza di Cauchy-Schwarz si ha che $-1 \le \rho_{XY} \le 1$.

Se $\rho_{XY} \gt 0$ c'è una **relazione lineare crescente** fra $X$ e $Y$;
	Nel caso in cui $\rho_{XY} = 1$ i punti $(x_i, y_i)$ sono allineati su una retta di pendenza positiva.
Se $\rho_{XY} \lt 0$ c'è una **relazione lineare decrescente** fra $X$ e $Y$;
	Nel caso in cui $\rho_{XY} = -1$ i punti $(x_i, y_i)$ sono allineati su una retta di pendenza negativa.
Se $\rho_{XY} = 0$, c'è assenza di legame lineare tra $X$ e $Y$, che sono dette **incorrelate** (ma non necessariamente indipendenti).

Il valore assoluto $|\rho_{XY}|$ indica la *forza* del legame lineare.

L'incorrelazione è una forma di indipendenza è una forma più debole dell'[[indipendenza statistica]]: la seconda implica la prima, ma non vale necessariamente il viceversa. ^4f77fa

>[!example] **Esempio**
>*Velocità* ([[Diagramma di Dispersione#^cc968a|continua]]). Si considerano i dati sulla velocità $X$ e sullo spazio di frenata $Y$ di automobili degli anni 20.
>![[Pasted image 20240116142355.png]]
>Si ha $\rho_{XY} = 0.81$, che indica un significativo legame lineare positivo.

Si considerano alcuni esempi di correlazione positiva
![[Pasted image 20240118023122.png]]e di correlazione negativa ![[Pasted image 20240118023240.png]]

Nel grafico seguente si rappresentano punti $(x_i, y_i),\ i=1,...,n$, tali che $y_i = x^2_i$.

Tra $X$ e $Y$ c'è un *legame quadratico* perfetto, che il coefficiente di correlazione lineare, che vale 0.12, non misura.
![[Pasted image 20240118023438.png]] Il coefficiente di correlazione lineare è influenzato dalla presenza di valori anomali.

>[!example] **Esempio**
>*Molla* ([[Studio della Dipendenza#^7dbcdc|continua]]). Si considerano i dati sulla lunghezza della molla $Y$ e sugli $n = 20$ pesi $X$ a cui viene sottoposta.
>Dai dati riportati nella tabella rappresentata in precedenza si ha che $$ \begin{gathered} E(X) = 1.9,\ E(Y)=5.388,\ V(X)=1.33, \\ V(Y) = 0.059,\ Cov(X,Y)=0.272 \end{gathered} $$ Da cui si ottiene che $$ \rho_{XY} = 0.272 \sqrt{1.33 \cdot 0.059} = 0.97 $$ valore che indica una correlazione positiva molto forte tra $X$ e $Y$.
>Se al posto dell'osservazione $(x_{19}, y_{19}) = (3.6, 5.68)$, si avesse il valore anomalo (outlier) $(x_{19}, y_{19}) = (3.6, 5.01)$, il coefficiente di correlazione lineare, che risente della presenza di valori anomali, risulterebbe pari a 0.76.


### Indice di correlazione di Spearman

Anche per **[[Variabili#^58fcd8|variabili qualitative ordinali]]** $X$ e $Y$ è possibile definire un indice che misura l'intensità (come l'[[indice di connessione|indice]] $χ^2$) e il verso dell'associazione.

Dati i valori osservati $(x_i, y_i),\ i=1,...,n$, si considerano i **[[rango|ranghi]]**, calcolati separatamente per ciascuna delle due variabili.

Si definisce **indice di correlazione tra i ranghi di Spearman** $\rho^S_{XY}$, il coefficiente di correlazione lineare calcolato sui ranghi invece che sulle osservazioni (e se ci sono osservazioni uguali, si considera come rango il valore medio delle loro posizioni).

Poiché si ha un indice di correlazione, $-1 \le \rho^S_{XY} \le 1$ e
* $\rho^S_{XY} = 1\ (\rho^S_{XY} = -1)$ indica una perfetta concordanza (discordanza) tra i ranghi di $X$ e di $Y$;
* $\rho^S_{XY} = 0$ indica che i ranghi di $X$ e di $Y$ non mostrano alcuna associazione.

Il coefficiente $\rho^S_{XY}$ si può utilizzare anche per **[[Variabili#Variabili quantitative (numeriche)|variabili quantitative]]**, come alternativa *robusta* a $\rho_{XY}$. Un ulteriore alternativa è rappresentata dall'**indice di correlazione di Kendall**.

***
Riferimenti:
[[3_Statdescr_Multiv_L3.pdf#page=29&selection=10,0,10,34|3_Statdescr_Multiv_L3, page 29]]

#statistica_descrittiva 
#statistica_descrittiva/analisi_multivariate 
#ppt-3 
#correlazione 