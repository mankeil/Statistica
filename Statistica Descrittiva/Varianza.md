Il più importante indice di [[variabilità]] per variabili [[Variabili#Variabili quantitative (numeriche)|quantitative]] è la **varianza**, che si indica con $V(Y)$, con $\sigma^2_Y$ o semplicemente con $\sigma^2$.

Data una variabile statistica $Y$  con [[Media Aritmetica|media aritmetica]] $E(Y)$, si ha $$ V(Y) = [E(Y-E(Y))^2] $$ La varianza è la media aritmetica della variabile scarto $Y-E(Y)$ elevata al quadrato e misura la dispersione dei dati attorno alla media. L'unità di misura è pari a quella dei dati elevata al quadrato.

Per il calcolo di $V(Y)$, si può riprendere quanto detto con riferimento alla media aritmetica.

Lo **scarto quadratico medio** di $Y$, indicato con $\sigma_Y$ o con $\sigma$, è la radice quadrata aritmetica(l'unica positiva) della varianza $$\sigma_Y = \sqrt{V(Y)}$$ è la stessa unità di misura di $Y$.

Se si dispone dei dati grezzi $Y = (y_1,...,y_n)$, e si è preventivamente calcolata $E(Y)$, allora la varianza corrisponde a $$V(Y) = \frac{1}{n} \sum^n_{i=1}(y_i - E(Y))^2$$ Se si dispone della [[Frequenze Assolute#^e17411|distribuzione di frequenza]] [[Frequenze Assolute|assoluta]] o [[Frequenze Relative|relativa]], $$V(Y) = \frac{1}{n} \sum^J_{j=1}(y_j-E(Y))^2f_j = \sum^J_{j=1}(y_j-E(Y))^2p_j$$ Se si dispone della **distribuzione di frequenza assoluta o relativa con** [[modalità]] **raggruppate in** [[Classi di modalità|classi]] (ad esempio $y_{j-1} \dashv y_j,\ j=1,...,J$) è necessario calcolare il *punto centrale* $y^c_j = (y_{j-1}+y_j)/2,\ j=1,...,J$, delle singole classi.

***
Riferimenti:
[[2_Statdescr_Univ_L2.pdf#page=101&selection=10,0,10,31|2_Statdescr_Univ_L2, pagina 101]]

#todo
#statistica_descrittiva 
#analisi_univariate
#ppt-2 
#indici_sintetici 
#indici_di_variabilità 