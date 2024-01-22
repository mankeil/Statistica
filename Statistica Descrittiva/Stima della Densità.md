In alternativa all'istogramma, è possibile definire una stima della distribuzione delle [[frequenze]] tramite una curva che risulti essere più smussata (in questo modo si tiene conto che la variabile è continua).

Date le osservazioni $y_1,...,y_i,...,y_n$, la funzione che rappresenta la **stima della densità con il metodo del nucleo** è definita come $$f_n(y) = \frac{1}{nb} \sum^n_{i=1} K(\frac{y-y_1}{b}),\ y \in \mathbb{R}$$ dove $K(\cdot$) è detto **nucleo** (**kernel**), $b \gt 0$ è la **banda** e $\mathbb{R}$ è l'insieme dei numeri reali.

 Ad un ogni dato $y_i$ si sovrappone non un rettangolo ma una curva che risulta essere più smussata. La sua altezza è proporzionale alla
 frequenza dei punti e la sua ampiezza dipende dalla banda $b$.

Si possono scegliere diversi nuclei $K(\cdot)$, che devono soddisfare ad alcune proprietà; in particolare, $K(u) \ge 0$ e $\int u^2 K (u) du = 1$.

È importante scegliere la banda $b$ in modo opportuno (in genere i software opera una scelta ottimale): se $b$ è troppo grande il grafico risulta appiattito, mentre se $b$ è troppo piccolo in grafico si avvicina ad un [[diagramma a bastoncini]].

Dato un insieme di osservazioni numeriche, si costruisce l'istogramma delle [[frequenze relative]], la stima della densità con scelta ottimale per $b$ (**nero**), con $b$ troppo grande (<span style="color:red">rosso</span>) e troppo piccolo (<span style="color:dodgerBlue">blu</span>).
![[Pasted image 20240116135019.png]]

***
Riferimenti:
[[Lucidi & materiale/2_Statdescr_Univ_L2.pdf#page=47&selection=10,0,10,19|2_Statdescr_Univ_L2, pagina 47]]

#statistica_descrittiva 
#statistica_descrittiva/analisi_univariate
#ppt-2 
#grafici