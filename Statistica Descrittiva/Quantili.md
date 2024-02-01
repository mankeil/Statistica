La [[Statistica Descrittiva/Mediana]] può venire interpretata come un particolare quantile di livello $\alpha$, con $\alpha \in (0, 1)$, indicato con la scrittura $y_{\alpha}$.

Data una [[Variabili#^58fcd8|variabile qualitativa ordinale]] o [[Variabili#Variabili quantitative (numeriche)|quantitativa]] $Y$, $y_{\alpha}$ è quel valore che, rispetto all'ordinamento non decrescente delle osservazioni, risulta preceduto da $\alpha 100\%$[^1] delle osservazioni e seguito ad $(1-\alpha)100\%$ osservazioni, a meno degli effetti di discretezza.

Il quantile di livello $\alpha$, con $\alpha \in (0,1)$, di una variabile statistica $Y$ corrisponde a ogni valore $y_{\alpha}$ tale che:
* almeno $\alpha 100\%$ unità statistiche presenta modalità inferiori o pari a $y_a$
* almeno $(1-\alpha)100\%$ unità statistiche presenta modalità superiori o pari a $y_{\alpha}$

È evidente che, se $\alpha = 0.5$, si ottiene la definizione di mediana.

I quantili di livello $\alpha = 0.25,\ 0.5,\ 0.75$ vengono chiamati **quartili** e dividono le osservazioni ordinate in 4 parti uguali. 
I quantili di livello $\alpha = 0.10,\ 0.20,\ . . . ,\ 0.90$ vengono chiamati **decili** e dividono le osservazioni ordinate in 10 parti uguali. 
I quantili di livello $\alpha = 0.01,\ 0.02,\ . . . ,\ 0.99$ vengono chiamati **percentili** dividono le osservazioni ordinate in 100 parti uguali.

Se si dispone dei dati grezzi $y_1, . . . , y_n$, ordinati secondo un ordinamento non decrescente, per individuare $y_{\alpha}$ si calcola $\alpha(n + 1)$.
* Se si ottiene un valore intero, $y_{\alpha}$ è la modalità che si trova nella posizione $\alpha(n+1)$, cioè $y_{\alpha(n+1)}$
* Se si ottiene un valore non intero, $y_{\alpha}$ corrisponde alle modalità che hanno come posizioni i valori interi che seguono o precedono immediatamente $\alpha(n+1)$
Se $\alpha = 0.5$, la procedura è equivalente a quella utilizzata per il calcolo della mediana in presenza di dati grezzi.
Se tali valori non coincidono, il quantile può non essere unico.

Nel caso di variabili quantitative si può avere anche un intervallo di valori che soddisfano alla definizione di quantile. In questo caso di può prendere il punto di mezzo come **quantile convenzionale**.

Con riferimento alla nozione di quantile si possono fare considerazioni analoghe a quelle introdotte per la mediana, per quanto riguarda il calcolo nel caso in cui si disponga solo della distribuzione di frequenza, [[Frequenze Assolute|assoluta]] o [[Frequenze Relative|relativa]], e la situazione con modalità raggruppate in [[Classi di modalità|classi]].


Il livello di riferimento non sarà più 0.5 ma, in generale, il valore $\alpha$.

>[!info] Esempio di applicazione
Una applicazione dei percentili riguarda la definizione di curve di crescita, come evidenziato nel grafico seguente
![[Pasted image 20240114170331.png]]

>[!example] **Esempio**
*Asfalto*. Si considerano i dati relativi ai valori di resistenza alla rottura di $n = 24$ misture di asfalto (in megapascal)
>
| 30 | 75 | 79 | 80 |
| ---- | ---- | ---- | ---- |
| 80 | 105 | 126 | 138 |
| 149 | 179 | 179 | 191 |
| 223 | 232 | 232 | 236 |
| 240 | 242 | 245 | 247 |
| 254 | 274 | 384 | 470 |
>
La [[Media Aritmetica|media aritmetica]] corrisponde a $E(Y) = 195.4$. Per il calcolo dei quantili di livello $\alpha$ si segue la procedura indicata in precedenza, che richiede in via preliminare in calcolo di $\alpha(n+1)$.
>
Avendo ordinato le osservazioni in senso crescente, si ottengono i quartili(convenzionali) 
$$ 0.25(24+1)=6.25 \Rightarrow y_{0.25}=(y_6 + y_7)/2=115.5$$ $$ 0.5(24+1)=12.5 \Rightarrow y_{0.5} = (y_{12} + y_{13})/2 = 207 $$ $$ 0.75(24+1) = 18.75 \Rightarrow y_{0.75} = (y_{18}+y_{19})/2 = 243.5 $$


***
Riferimenti:
[[Lucidi & materiale/2_Statdescr_Univ_L2.pdf#page=80&selection=10,0,10,8|Lucido]]

%%Footnotes%%

[^1]: Equivale a dire $\alpha \times 100$

#statistica_descrittiva 
#statistica_descrittiva/analisi_univariate
#ppt-2 
#indici_sintetici 
#indici_sintetici/indici_di_posizione