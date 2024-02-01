Il più importante indice di [[variabilità]] per variabili [[Variabili#Variabili quantitative (numeriche)|quantitative]] è la **varianza**, che si indica con $V(Y)$, con $\sigma^2_Y$ o semplicemente con $\sigma^2$.

Data una variabile statistica $Y$ con [[media aritmetica]] $E(Y)$, si ha $$ V(Y) = [E(Y-E(Y))^2] $$ La varianza è la media aritmetica della variabile scarto $Y-E(Y)$ elevata al quadrato e misura la dispersione dei dati attorno alla media. L'unità di misura è pari a quella dei dati elevata al quadrato.

Per il calcolo di $V(Y)$, si può riprendere quanto detto con riferimento alla media aritmetica.

Lo **scarto quadratico medio** di $Y$, indicato con $\sigma_Y$ o con $\sigma$, è la radice quadrata aritmetica(l'unica positiva) della varianza $$\sigma_Y = \sqrt{V(Y)}$$ è la stessa unità di misura di $Y$. ^af26fa

Se si dispone dei dati grezzi $Y = (y_1,...,y_n)$, e si è preventivamente calcolata $E(Y)$, allora la varianza corrisponde a $$V(Y) = \frac{1}{n} \sum^n_{i=1}(y_i - E(Y))^2$$Se si dispone della distribuzione di frequenza [[Frequenze Assolute|assoluta]] o [[Frequenze Relative|relativa]], $$V(Y) = \frac{1}{n} \sum^J_{j=1}(y_j-E(Y))^2f_j = \sum^J_{j=1}(y_j-E(Y))^2p_j$$ Se si dispone della **distribuzione di frequenza assoluta o relativa con** [[modalità]] **raggruppate in** [[Classi di modalità|classi]] (ad esempio $y_{j-1} \dashv y_j,\ j=1,...,J$) è necessario calcolare il *punto centrale* $y^c_j = (y_{j-1}+y_j)/2,\ j=1,...,J$, delle singole classi.
In questo caso: $$ V(Y) = \frac{1}{n} \sum^J_{j=1}(y^c_j - E(Y))^2 f_j = \sum^J_{j=1}(y^c_j - E(Y))^2 p_j $$ Questa procedura approssimata per il calcolo di $V(Y)$ è equivalente a quella che si definisce quando si dispone dei dati grezzi se le osservazioni in una classe coincidono con il punto centrale della classe.

> [!example] **Esempio**
Si consideri la seguente tabella di frequenza dalla quale si ricava che $E(Y) = 0.61$
>
| $y_j$ | 0 | 1 | 2 | 3 | 4 | Totale |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| $f_j$ | 109 | 65 | 22 | 3 | 1 | 200 |
È immediato concludere che $$ V(Y)=\frac{1}{200}[(0-0.61)^2 \cdot 109 + (1-0.61)^2 \cdot 65 + (2-0.61)^2 \cdot 22$$$$+ (3-0.61)^2 \cdot 3 + (4-0.61)^2 \cdot 1] = 0.608$$ Inoltre, $\sigma_Y = \sqrt{V(Y)} = 0.780$

>[!example] **Esempio**
Si consideri la seguente tabella di frequenza con modalità raggruppate in classi
>
| Classe | $0 \dashv 10$ | $10 \dashv 15$ | $15 \dashv 20$ | Totale |
| ---- | ---- | ---- | ---- | ---- |
| freq. rel. | 0.30 | 0.52 | 0.18 | 1 |
I valori centrali delle classi sono, rispettivamente, $y^c_1=5$, $y^c_2=12.5$ e $y^c_3=17.5$, da cui si conclude che $$ V(Y) = (5-11.15)^2 \cdot 0.30 + (12.5+11.15)^2 \cdot 0.52 $$$$+ (17.5-11.15)^2 \cdot 0.18 = 19.55$$

### Proprietà
La varianza soddisfa le seguenti proprietà.
* **Proprietà di non negatività**. $V(Y) \ge 0$, con $V(Y)=0$ se e solo se $Y$ è [[variabile statistica degenere|degenere]].
* **Formula per il calcolo**. $$V(Y) = E(Y^2) - (E(Y))^2$$ Infatti, sfruttando la [[Media Aritmetica#Proprietà|proprietà di linearità]] della media aritmetica $$ V(Y) = E\{(Y-E(Y))^2\} = E\{Y^2 + (E(Y))^2 - 2YE(Y)\}$$$$ = E(Y^2) + (E(Y))^2 - 2E(Y)E(Y) = E(Y^2)-(E(Y))^2$$ Inoltre, se $E(Y)=0$ allora $V(Y) = E(Y^2)$.
* **Proprietà di invarianza per translazioni**. $$V(Y+b) = V(Y),\ b \in \mathbb{R}$$ Infatti, sfruttando la proprietà di linearità della media aritmetica, $$V(Y+b) = E\{(Y+b-E(Y+b))^2\} = E\{(Y+b-E(Y)-b)^2\} = $$$$ = E\{(Y-E(Y))^2\} = V(Y)$$
* **Proprietà di omogeneità di secondo grado**. $$ V(aY) = a^2V(Y),\ a \in \mathbb{R}$$ Infatti, sfruttando la proprietà di linearità della media aritmetica, $$V(aY) = E\{(aY-E(aY))^2\} = E\{(aY-E(Y))^2\} = $$$$= E\{a^2(Y-E(Y))^2\} = a^2E\{(Y-E(Y))^2\} = a^2V(Y)$$
Dalle ultime due proprietà discende che $V(aY+b) = a^2V(Y)$.

>[!example] **Esempio**
Si consideri la tabella di frequenza vista in precedenza, dalla quale si è ricavato che $E(Y) = 0.61$
>
| $y_j$ | 0 | 1 | 2 | 3 | 4 | Totale |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| $f_j$ | 109 | 65 | 22 | 3 | 1 | 200 |
È immediato concludere che $$V(Y) = \frac{1}{200}[0^2 \cdot  109 + 1^2 \cdot 65 + 2^2 \cdot 22 + 3^2 \cdot 3 + 4^2 \cdot 1] = 0.98$$ Usando la formula per il calcolo, si ottiene che $$V(Y) = E(Y^2)-(E(Y))^2 = 0.98 - 0.61^2 = 0.608$$che coincide con il valore ottenuto con la definizione di varianza.

***
Riferimenti:
[[Lucidi & materiale/2_Statdescr_Univ_L2.pdf#page=101&selection=10,0,10,31|2_Statdescr_Univ_L2, pagina 101]]

#statistica_descrittiva 
#statistica_descrittiva/analisi_univariate
#ppt-2 
#indici_sintetici 
#indici_sintetici/indici_di_variabilità 