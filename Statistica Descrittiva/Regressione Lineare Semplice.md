Si analizzano congiuntamente di due o più [[Variabili#variabili quantitative (numeriche)]] È una generalizzazione dell'analisi di [[dipendenza in media]].

In generale, con l'analisi di regressione si studia la media condizionata di una **variabile risposta** $Y$ in funzione di una (*regressione semplice*) o più (*regressione multipla*) **variabili esplicative** $X_1,...,X_p,\ p \ge 1$.

Si considera la **regressione lineare semplice**, dove tra la variabile risposta $Y$ e l'unica variabile esplicativa $X$ si ipotizza una relazione lineare.

>[!example] **Esempio**
>*Molla*. ([[Studio della Dipendenza#^7dbcdc|continua]]). Si considerano i dati sulla lunghezza della molla $Y$ e sugli $n = 20$ diversi pesi $X$ a cui viene sottoposta.
>
>Si vuole studiare la relazione tra $X$ e $Y$ e, più precisamente, verificare se $X$ *spiega* $Y$.
>![[Pasted image 20240117005941.png]]
>In particolare, per descrivere il comportamento in media di $Y$ in funzione di $X$ si può considerare l'equazione della retta $$y_1 = a + bx_i + \text{errore},\ i = 1,...,20$$ dove $a$ indica la lunghezza attesa della molla nel caso in cui il peso sia nullo e $b$ determina il verso e l'intensità della relazione lineare tra $X$ e $Y$.
>
>Il termine di errore evidenzia il fatto che la relazione lineare non sia adatta perfettamente ai dati $(x_i, y_i),\ i=1,...,20$.
>
>L'errore racchiude cioè che la retta, e quindi $X$, non spiega del fenomeno $Y$ e l'eventuale errore di misura associato a $Y$.

ll **modello di regressione lineare semplice** (**modello lineare**) è definito dall'equazione $$ y_i = a+bx_i + \epsilon_i,\ i=1,...,n$$ dove $(x_i, y_i),\ i = 1,...,n$, sono i valori osservati per la **variabile dipendente** $Y$ e per la **variabile esplicativa** $X$.

I valori $\epsilon_i,\ i=1,...,n$, specificano gli **errori**, mentre $a$ e $b$ sono i **coefficienti di regressione**, con $a$ l'intercetta e $b$ il coefficiente angolare della **retta di regressione** $y = a + bx$. ^f821e4

L'interesse è rivolto al comportamento complessivo e non a ciò che avviene per le singole coppie di osservazioni.

Il modello si intende **lineare nei parametri**, non nella variabile esplicativa. Quindi, $$ \begin{gather} y_i = a + b \cdot \log(x_i) + \epsilon_i, \\ y^2_i = a + b \cdot \exp(x_i) + \epsilon_i, \\ y_i = a + b^2x_i + \epsilon_i\\ \end{gather}$$ sono modelli lineari per $Y$ (o per $Y^2$) nelle variabili esplicative $\log(X), \exp(X)$ e $X$, rispettivamente (una volta effettuata la riparametrizzazione $c = b^2$ ).

Invece, $$y_i = a + a^2x_i + \epsilon_i$$ non è un modello lineare in quanto il parametro $a$ compare anche elevato al quadrato.

***
Riferimenti:
[[Lucidi & materiale/3_Statdescr_Multiv_L3.pdf#page=37&selection=10,0,10,28|3_Statdescr_Multiv_L3, page 37]]

#statistica_descrittiva 
#statistica_descrittiva/analisi_multivariate 
#ppt-3 
#regressione