Le variabili vengono analizzate in modo **asimmetrico** perché si studia la dipendenza in media della **[[Variabili#Variabili quantitative (numeriche)|variabile quantitativa]]** $Y$ dai livelli della **[[Variabili#Variabili qualitative (categoriali)|variabile qualitativa]]** $X$.

L'indipendenza in media è una forma debole di [[Indipendenza statistica|indipendenza]] nella quale non si considera la distribuzione di frequenza di $Y$ ma solo la sua [[Media Aritmetica|media]].

Due variabili $Y$ ed $X$ si diranno **indipendenti in media** se la media condizionata di $Y$ dato $X$ è la stessa per ogni valore assunto da $X$, ovvero se $$ E(Y|X=x_r) = E(Y)$$per ogni possibile $x_r, r=1,...,m$.
Viceversa, se le varie medie condizionate sono diverse, allora le due variabili si diranno **dipendenti in media**.

Se le due variabili sono indipendenti allora sono anche indipendenti in media, mentre non è vero il viceversa.

È possibile estendere tale nozione di indipendenza considerando l'**indipendenza in distribuzione**. In questo caso, oltre al calcolo delle medie condizionate, si confrontano anche altri indici sintetici oppure i grafici (ad esempio, [[istogramma|istogrammi]] o [[boxplot]]) ottenuti per i sottogruppi definiti le varie [[modalità]] di $X$.

>[!example] **Esempio**
>*Geyser Old Faithful* (continua). Si considerano i dati riferiti alle durate delle eruzioni del geyser Old Faithful e si indica con $X$ il tipo di eruzione e $Y$ la durata della pausa.
>
| Modalità $x$ di $X$ | Media condizionata di $Y$ dato $X=x$ |
| ---- | ---- |
| Corta | 54.49 |
| Lunga | 79.99 |
Le medie condizionate sono molto diverse, quindi non si può parlare di indipendenza media tra $X$ e $Y$.
>
Se si confrontano gli istogrammi per la variabile statistica $Y$ riferita ai due gruppi, si conclude che c'è, più in generale, dipendenza in distribuzione.

***
Riferimenti:
[[3_Statdescr_Multiv_L3.pdf#page=25&selection=10,0,10,19|3_Statdescr_Multiv_L3, page 25]]

#statistica_descrittiva 
#statistica_descrittiva/analisi_multivariate 
#ppt-3 
#dipendenza 