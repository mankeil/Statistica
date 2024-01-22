L'individuazione del centro di un insieme di dati, tramite opportuni [[Indici Sintetici - Introduzione#Indici di Posizione|indici di posizione]], può non essere sufficiente per descrivere in modo completo la associata [[distribuzione|distribuzione di frequenza]].

>[!example]+ **Esempio**
>
*Inquinamento*. Per confrontare l'efficacia di due diversi dispositivi per contenere l'inquinamento atmosferico si sono analizzati i fumi prodotti da una certa industria. 
>
Si sono considerati 360 campioni di fumo e si è misurata la quantità di pulviscolo inquinante in g/min. In 180 si è utilizzato il dispositivo anti-inquinante A, mentre sui campioni rimanenti si è utilizzato il dispositivo anti-inquinante B. Si hanno i seguenti dati:
>
Dispositivo A: $14.98654, 15.14828, 15.15741, . . . , 14.92036, 14.93270$
Dispositivo B: $14.62067, 15.26097, 14.87602, . . . , 14.74481, 15.13047$
>
Si calcolano alcuni valori di sintesi
>
| Dispositivo | $y_{(1)}$ | $y_{0.25}$ | $y_{0.5}$ | $\mu$ | $y_{0.75}$ | $y_{(n)}$ |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| A | 14.44 | 14.87 | 15.00 | 15.00 | 15.14 | 15.64 |
| B | 13.83 | 14.83 | 15.02 | 15.02 | 15.22 | 15.80 |
>
$y_{0.25}$ : [[Quantili|quantile]] con $\alpha = 0.25$, inoltre il quantile $y_{0.5}$ corrisponde alla [[mediana]]
$\mu$  : [[Media Aritmetica|media aritmetica]]
>
Entrambi i dispositivi sembrano tarati allo stesso modo, poiché forniscono valori centrati sul valore di 15 g/min.
![[Pasted image 20240115010058.png]]
![[Pasted image 20240115010155.png]]
>
Dalla analisi dei grafici si nota che gli scostamenti dal valore centrale sembrano essere più elevati per il dispositivo B.
>
I dati riferiti a B sono più dispersi attorno al valore centrale, cioè mostrano una variabilità più accentuata.

^f15dac

Si presentano i seguenti **indici di variabilità** utili per [[Variabili#Variabili quantitative (numeriche)|variabili quantitative]]:
* [[Campo di Variazione]]
* [[Scarto Interquartilico]]
* [[Varianza]] (e **scarto quadratico medio**)
* [[Coefficiente di Variazione]]

Non si considerano gli indici di variabilità per [[Variabili#Variabili qualitative (categoriali)|variabili qualitative]], detti anche **indici di mutabilità**.

La variabilità di una variabile statistica si traduce nella diversificazione delle [[modalità]] osservate. Se $Y$ è quantitativa, tale diversificazione si intende sia come **diversità** di valori osservati sia come distanza fra essi. ^2f6152

>[!example] **Esempio**
>Se Y è una [[variabile statistica degenere]] ($S_Y = {y_1}$) la sua variabilità è nulla. 
>Se $Y_1 = (1, 1, 1, 2, 2)$ e $Y_2 = (1, 1, 1, 10, 10)$, i due [[Variabili#Supporto di una variabile|supporti]] corrispondenti contengono due modalità, ma la variabilità di $Y_2$ è più accentuata di quella di $Y_1$.

***
Riferimenti:
[[Lucidi & materiale/2_Statdescr_Univ_L2.pdf#page=94&selection=10,0,10,21|Lucido]]

#statistica_descrittiva 
#statistica_descrittiva/analisi_univariate
#ppt-2 
#indici_sintetici 
#indici_di_variabilità