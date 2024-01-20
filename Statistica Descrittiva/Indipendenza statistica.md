Si nota che la [[Distribuzioni di Frequenza#^d8cbd3|distribuzione condizionata]] di $Y$ varia al variare di $X$, e viceversa. Ad esempio, se l'attitudine musica è sufficiente, l'attitudine pittorica non può essere ottima.

Quindi si può concludere che esiste una qualche forma di dipendenza fra le due variabili.

Si parla di **indipendenza statistica** quando tutte le distribuzioni condizionate di $Y$ dato $X = x_r,\ r=1,...,m$, sono uguali e quindi uguali alla [[Distribuzioni di Frequenza#^3f36a4|distribuzione marginale]] di $Y$.

Analoghe considerazioni si possono fare per le distribuzioni condizionate di $X$ dato $Y = y_s,\ s=1,...,k$, e per la [[Distribuzioni di Frequenza#^08c8ee|distribuzione marginale]] di $X$.

In tal caso, il valore assunti da una variabile non influenza il valore assunto dall'altra.

Dall'uguaglianza delle [[Distribuzioni di Frequenza#^3f15a9|distribuzioni di frequenza relativa]] condizionata di $X$ dato $Y=y_s, s=1,...,k$ alla distribuzione marginale di $X$ (o viceversa), si ha che $$ \frac{n_{rs}}{n_{+s}} = \frac{n_{r+}}{n},\ r=1,...,m,\ s=1,...,k$$ ovvero $$ n_{rs} = \frac{n_{r+}n_{+s}}{n},\ r=1,...,m,\ s=1,...,k $$ che corrisponde alla definizione di variabili $X$ e $Y$ **statisticamente indipendenti**.

Se due variabili sono indipendenti l'[[indice di connessione]] $\chi^2$ sarà uguale a 0.

Dividendo per $n$ si ottiene la seguente specificazione alternativa basata sulle [[frequenze relative]] $$\frac{n_{rs}}{n} = \frac{n_{r+}}{n} \frac{n_{+s}}{n},\ r=1,...,m,\ s=1,...,k$$
Inoltre, l'indipendenza statistica implica l'[[Coefficiente di Correlazione Lineare#^4f77fa|incorrelazione]].

***
Riferimenti:
[[3_Statdescr_Multiv_L3.pdf#page=18&selection=10,0,10,23|3_Statdescr_Multiv_L3, page 18]]

#statistica_descrittiva 
#statistica_descrittiva/analisi_multivariate 
#ppt-3 
#dipendenza 