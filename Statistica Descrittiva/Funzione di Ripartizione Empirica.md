Un'ulteriore rappresentazione grafica per **dati [[Variabili#Variabili quantitative (numeriche)|quantitativi]]**, e che risulta in molti casi particolarmente efficace, è fornita dalla **funzione di ripartizione empirica**.

La funzione di ripartizione empirica è una funzione il cui valore nel punto $y \in \mathbb{R}$ corrisponde al rapporto tra il numero di osservazioni minori o uguali a $y$ e il numero totale di osservazioni $$ F_n(y) = \frac{\text{no. oss.} \le y}{\text{no. totale oss.}},\ y \in \mathbb{R}$$ Al variare di $y$, fornisce la proporzione cumulata di unità statistiche che presentano [[modalità]] minori o uguali a $y$ ed è quindi una funzione a gradini.

La nozione di ripartizione empirica è utile per una rappresentazione grafica delle [[frequenze relative]] [[Frequenze Cumulate|cumulate]], in particolare per variabili quantitative discrete.

>[!example] **Esempio**
Si consideri la seguente tabella delle frequenze relative e relative cumulate riferita ad una variabile quantitativa discreta. Di seguito viene rappresentata la corrispondente funzione di ripartizione empirica.
>
| $Y$ | 0 | 1 | 2 | 3 | 4 | 5 | 7 | Tot. |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| freq. rel. | 0.04 | 0.06 | 0.22 | 0.26 | 0.30 | 0.10 | 0.02 | 1 |
| freq. rel. cum. | 0.04 | 0.10 | 0.32 | 0.58 | 0.88 | 0.98 | 1.00 |  |
![[Pasted image 20240116141113.png]]

>[!example] **Esempio**
*Geyser Old Faithful*. Si dispone di dati riferiti alle durate delle pause (in minuti) e alla tipologia delle eruzioni che precedono le pause (lunga o corta), con riferimento al geyser Old Faithful che si trova nel parco nazionale di Yellowstone, Wyoming, USA.
>
Su hanno le seguenti $n = 272$ osservazioni
>
| Pausa | Eruzione |
| ---- | ---- |
| 79 | Lunga |
| 54 | Corta |
| 74 | Lunga |
| 62 | Corta |
| 85 | Lunga |
| 55 | Corta |
| $$\vdots$$ | $$ \vdots $$ |
| 90 | Lunga |
| 46 | Corta |
| 73 | Lunga |
Considerando tutti i dati disponibili si può calcolare il seguente [[istogramma]]. Si individuano [[Classi di modalità|classi]] di ampiezza costante pari a 5 minuti.
![[Pasted image 20240116141553.png]]
La forma dell'istogramma è dovuta al fatto che si sono considerati congiuntamente i dati sulla durata delle pause, senza distinguere tra durata corta o lunga dell'eruzione precedente.
>
Se si considerano le durate delle pause, raggruppando i dati in base alla tipologia dell'eruzione precedente, si ottengono i seguenti istogrammi 
![[Pasted image 20240116141718.png]]
Le pause successive ad un'eruzione corta tendo ad essere più corte di quelle che seguono un'eruzione lunga.
>
Considerando i due insiemi di dati distinti, si possono determinare le associate funzioni di ripartizione empiriche (<span style="color:red">rosso</span> = eruzione corta, **nero** = eruzione lunga), che confermano questa affermazione.
![[Pasted image 20240116141937.png]]

^1df9ab

***
Riferimenti:
[[Lucidi & materiale/2_Statdescr_Univ_L2.pdf#page=49&selection=10,0,10,33|2_Statdescr_Univ_L2, pagina 49]]

#statistica_descrittiva 
#statistica_descrittiva/analisi_univariate
#ppt-2 
#grafici