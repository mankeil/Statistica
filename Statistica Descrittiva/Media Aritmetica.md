La media aritmetica, che è l'[[Statistica Descrittiva/Indici Sintetici - Introduzione#Indici di Posizione|indice di posizione]] più noto, si può calcolare per una [[Variabili#Variabili quantitative (numeriche)|variabile quantitativa]] $Y$ e si indica con $E(Y)$, con $\mu_Y$ o semplicemente con $\mu$. 

>[!example]+ **Esempio:** 
Sia $Y = (27, 30, 30)$ la [[Variabili#Variabili statistiche|variabile statistica]] che descrive i voti riportati in tre esami da uno studente. La media aritmetica dei voti è $\mu_Y = (27 + 30 + 30)/3 = 29$. Si noti che 29 non corrisponde a nessuno dei voti ottenuti.
Se $Y = (28, 30, 30)$, allora $\mu_Y = (28 + 30 + 30)/3 = 29.3$, che non corrisponde a nessuna potenziale modalità per $Y$ . 
>
In entrambi i casi la media sintetizza i valori osservati indicandone un centro. 

Se si dispone dei dati grezzi $y_1,...,y_n$ allora
$$ E(Y) = \frac{1}{n} \sum^n_{i=1}y_i$$
Se, con riferimento ad una [[Variabili#^a1fa07|variabile quantitativa discreta]] $Y$ , si dispone della tabella di [[Frequenze Assolute|frequenza assoluta]] o [[Frequenze Relative|relativa]] allora

$$E(Y) = \frac{1}{n} \sum^J_{j=1} y_j f_j = \sum^J_{j=1} y_j p_j$$

>[!example]+ **Esempio:**
Si consideri la seguente tabella di frequenza
>
>| $y_j$ | 0 | 1 | 2 | 3 | 4 | Totale |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| $f_j$ | 109 | 65 | 22 | 3 | 1 | 200 |
È immediato concludere che $E(Y) = \frac{1}{200} \sum^4_{j=1}y_j f_j = \frac{1}{200} \times 65 \times 1 + 2 \times 22 + 3 \times 3 + 4 \times 1 = 122 \div 200 = 0.61$.

Se, con riferimento ad una [[Variabili#^3cc28d|variabile quantitativa continua]] $Y$, si dispone della tabella di frequenza assoluta o relativa con [[Classi di modalità|modalità raggruppate in classi]], (ad esempio $y_{j−1} \vdash y_j,\  j = 1, . . . , J$), si calcola il punto centrale delle singole classi $$y^c_j = (y_{j−1} + y_j ) \div 2,\ j = 1, . . . , J$$ e
$$ E(Y)= \frac{1}{n} \sum^J_{j=1}y_j^c f_j = \sum^J_{j=1}y^c_j p_j$$
Se ci sono classi aperte, il punto centrale viene individuato dopo aver convenientemente "chiuso la classe". 

Questa procedura approssimata per il calcolo di $E(Y)$ è equivalente a quella che si definisce quando si dispone dei dati grezzi se viene soddisfatta una delle seguenti ipotesi:
* Le osservazioni che cadono in una classe coincidono con il punto centrale della classe;
* Le osservazioni sono distribuite in modo uniforme nella classe di appartenenza.

>[!example]+ **Esempio:**
Si consideri la seguente tabella di frequenza con modalità raggruppate in classi
>
| Classe | $0 \dashv 10$ | $10 \vdash 15$ | $15 \dashv 20$ | Totale |
| ---- | ---- | ---- | ---- | ---- |
| [[Frequenze Relative\|freq. rel.]] | 0.30 | 0.52 | 0.18 | 1 |
I valori centrali delle classi sono, rispettivamente, $y^c_1 = 5$, $y^c_2=12.5$ e $y^c_3=17.5$, da cui si conclude che $$E(Y) = \sum^3_{j=1} y^c_j p_j =$$ 
$$ 1 \cdot 5 \cdot 0.30 + 12.5 \cdot 0.52 + 17.5 \cdot 0.18 = 11.15$$

Non è detto che $E(Y)$ coincida con una delle modalità osservate o osservabili.
Può essere vista anche come il [[valore di equiripartizione]] sulle unità statistiche del totale delle osservazioni. 

La media aritmetica risente della presenza di osservazioni anomale o estreme (non è un indice robusto). Esistono altre tipologie di medie, che non vengono considerate in questa sede.

### Proprietà
La media aritmetica soddisfa le seguenti proprietà:
* **Proprietà di Cauchy**: 
  Sia $S_Y = {y_1, . . . , y_J}$, con $y_1 < · · · < y_J$ , allora $$ y_1 \le E(Y) \le y_J$$
  La media è compresa tra il più piccolo e il più grande valore osservato.
  Infatti, per ogni $j = 1,...,J$ $$y_1 \le y_j \le y_J \ \Rightarrow \ y_1p_j \lt y_jp_j \lt y_Jp_j \ \Rightarrow$$$$ \sum^J_{j=1}y_1p_j \le \sum^J_{j=1}y_jp_j \le \sum^{J}_{j=1}y_Jpj \Rightarrow $$$$ y_1 \sum^J_{j=1}p_j \le \sum^J_{j=1}y_jp_j \le y_J \sum^J_{j=1}p_j $$ da cui si ottiene la tesi, poiché $\sum^J_{j=1}p_j = 1$
* **Proprietà di baricentro**: 
  Sia $Y - E(Y)$ la variabile scarto $Y$ dalla sua media $E(Y)$, allora $$E(Y-E(Y)) = 0$$Infatti, considerando i dati grezzi e le modalità osservate $y_i - E(Y)$, $j = 1,...,J$, della variabile $Y-E(Y)$, $$ E(Y-E(Y)) = \frac{1}{n} \sum^n_{i=1}(y_i-E(Y)) = \frac{1}{n} \sum^n_{i=1}y_i - \frac{1}{n} \sum^n_{i=n}E(Y) = $$$$ = E(Y) - \frac{1}{n}nE(Y)=0$$
* **Proprietà di linearità:** 
  Sia $aY + b,\ a,\ b \in R$, una trasformata lineare della variabile $Y$ , allora $$E(aY+b) = aE(Y)+b$$Infatti, considerando i dati grezzi e le modalità osservate $ay_i + b,\ j= 1,...,J$, della variabile $aY+b$,$$ \begin{gather} E(aY+b) = \frac{1}{n}\sum^n_{i=1}(ay_i+b)=\frac{1}{n}\sum^n_{i=1} + \frac{1}{n} \sum^n_{i=1}b = \\
   = a \frac{1}{n} \sum^n_{i=1}y_i + \frac{1}{n} nb = aE(Y)+b \end{gather}$$
---
Riferimenti:
[[Lucidi & materiale/2_Statdescr_Univ_L2.pdf#page=60&selection=10,0,10,37|Lucido]]

#statistica_descrittiva 
#statistica_descrittiva/analisi_univariate
#ppt-2 
#indici_sintetici 
#indici_sintetici/indici_di_posizione