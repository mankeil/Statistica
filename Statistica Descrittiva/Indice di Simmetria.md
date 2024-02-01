Data una variabile statistica [[Variabili#Variabili quantitative (numeriche)|quantitativa]] $Y$, con [[media aritmetica]] $E(Y)$, l'indice **indice di [[simmetria]]** più utilizzato è $$ \gamma_Y = \frac{E[(Y-E(Y))^3]}{\sigma^3_Y}$$ dove $\sigma_Y = \sqrt{V(Y)}$ è lo [[scarto quartilico medio]] di $Y$.

Se si dispone dei dati grezzi $Y = (y_1,...,y_n)$, e si sono preventivamente calcolati $E(Y)$ e $\sigma_Y$, allora l'indice di simmetria corrisponde a $$ \gamma_Y = \frac{\frac{1}{n} \sum^n_{i=1}(y_i - E(Y))^3}{\sigma^3_Y}$$ Se la distribuzione di frequenza è [[simmetria|simmetrica]], $\gamma_Y \approx 0$; se c'è **asimmetria negativa**, $\gamma_Y \lt 0$, se c'è **asimmetria positiva**, $\gamma_Y \gt 0$.

>[!example] **Esempio**
*Inquinamento* ([[Indici di Variabilità - Introduzione#^f15dac|continua]]). Con riferimento ad dati sui due dispositivi anti-inquinamento, poiché la media e [[Statistica Descrittiva/Mediana]] coincidono, si conclude che le distribuzioni di frequenza sono simmetriche; i valori dell'indice di simmetria sono pari a 0.095 e - 0.225, rispettivamente.
![[Pasted image 20240115220415.png]]
>
Dall'analisi dell'[[Istogramma]] si conferma la sostanziale simmetria.

***
Riferimenti:
[[Lucidi & materiale/2_Statdescr_Univ_L2.pdf#page=114&selection=7,1,10,19|2_Statdescr_Univ_L2, pagina 114]]

#statistica_descrittiva 
#statistica_descrittiva/analisi_univariate
#ppt-2 
#indici_sintetici 
#indici_sintetici/indici_di_variabilità 