Data una variabile statistica [[Variabili#Variabili quantitative (numeriche) |quantitativa]] $Y$, con [[media aritmetica]] $E(Y)$, l'indice **indice di [[curtosi]]** più utilizzato è $$ \beta_Y = \frac{E[(Y-E(Y))^4]}{\sigma^4_Y} $$ dove $\sigma_Y = \sqrt{V(Y)}$ è lo [[scarto quartilico medio]] di $Y$.

Se si dispone dei dati grezzi $Y = (y_1,...,y_n)$, e si sono preventivamente calcolati $E(Y)$ e $\sigma_Y$, allora l'indice di curtosi corrisponde a $$ \beta_Y = \frac{\frac{1}{n} \sum^n_{i=1}(y_i-E(Y))^4}{\sigma^4_Y} $$
Se la distribuzione di frequenza é:
* **normocurtica**, $\beta_Y \approx 3$; 
* **leptocurtica**, $\beta_Y \gt 3$;
* **platicurtica**, $\beta_Y \lt 3$.

>[!example] **Esempio**
*Inquinamento* ([[Indici di Variabilità - Introduzione#^f15dac|continua]]). Con riferimento ad dati sui due dispositivi anti-inquinamento.
![[Pasted image 20240115220415.png]]
>
Dall'analisi dell'[[Istogramma]], si deduce che la secondo distribuzione che la seconda distribuzione presenta code più pesanti della prima. Infatti, i valori dell'indice di curtosi sono paria a 2.937 e 3.398, rispettivamente.

***
Riferimenti:
[[2_Statdescr_Univ_L2.pdf#page=116&selection=10,0,10,17|2_Statdescr_Univ_L2, pagina 116]]

#statistica_descrittiva 
#statistica_descrittiva/analisi_univariate
#ppt-2 
#indici_sintetici 
#indici_di_variabilità 