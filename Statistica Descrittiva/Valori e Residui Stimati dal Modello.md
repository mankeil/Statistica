Una volta calcolate le stime $\hat a$ e $\hat b$ per i [[Regressione Lineare Semplice#^f821e4|coefficienti di regressione]], ad esempio attraverso il [[metodo dei minimi quadrati]], si possono determinare i **valori stimati dal modello** $$\hat y = \hat a + \hat b x_i,\ i = 1,...,n$$Cioè i valori della variabile risposta $Y$  per ogni valore osservato $x_i$.

Nel caso in cui si considerino valori per $X$ che non corrispondono ai valori osservati, si ottengono i **valori previsti dal modello**, che sono utili per fare previsioni o ricostruire di valori mancanti per $Y$.

Occorre fare molta attenzione quando si estrapola la retta di regressione stimata, cioè quando si fanno previsioni al di fuori dell'intervallo dei valori osservati per la variabile esplicativa $X$.

Infine si possono calcolare i **residui stimati** $$\hat \epsilon_i = y_i - \hat a - \hat b x_i = y_i - \hat y_i,\ i=1,...,n$$cioè la stima degli errori (residui) basata sulle osservazioni.

***
Riferimenti:
[[Lucidi & materiale/3_Statdescr_Multiv_L3.pdf#page=46&selection=10,0,10,44|3_Statdescr_Multiv_L3, page 46]]

#statistica_descrittiva 
#statistica_descrittiva/analisi_multivariate 
#ppt-3 
#regressione 