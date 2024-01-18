Vale la **diseguaglianza di Cauchy-Schwarz**: $$ -\sigma_X \sigma_Y \le \sigma_{XY} \le \sigma_X \sigma_Y$$ Una misura normalizzata della [[Studio della Dipendenza|dipendenza lineare]] è il coefficiente di correlazione lineare definito da $$\rho_{XY} = Cor(X, Y) = \frac{\sigma{XY}}{\sigma{X}\sigma{Y}}$$ Dalla diseguaglianza di Cauchy-Schwarz si ha che $-1 \le \rho_{XY} \le 1$.

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
![[Pasted image 20240118023122.png]]e di correlazione negativa ![[Pasted image 20240118023240.png]] Nel grafico seguente si rappresentano punti $(x_i, y_i),\ i=1,...,n$, tali che $y_i = x^2_i$.

Tra $X$ e $Y$ c'è un *legame quadratico* perfetto, che il coefficiente di correlazione lineare, che vale 0.12, non misura.
![[Pasted image 20240118023438.png]] Il coefficiente di correlazione lineare è influenzato dalla presenza di valori anomali.

[todo]

***
Riferimenti:
[[3_Statdescr_Multiv_L3.pdf#page=29&selection=10,0,10,34|3_Statdescr_Multiv_L3, page 29]]

#statistica_descrittiva 
#statistica_descrittiva/analisi_multivariate 
#ppt-3 
#correlazione 