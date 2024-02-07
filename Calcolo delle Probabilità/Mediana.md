La **mediana** della [[distribuzione di probabilità]] di $X$, o più semplicemente la mediana di $X$, indicata con $x_{0.5}$, è quel valore $x_{0.5} \in \mathbb{R}$ tale che $$ \begin{gather} P(X \le x_{0.5}) \gt 1/2 & \text{e} & P(X \ge x_{0.5}) \ge 1/2.\end{gather}$$Quindi, $x_{0.5}$ ripartisce la massa unitaria di probabilità, in modo che gli eventi $X \le x_{0.5}$ e $X \ge x_{0.5}$ abbiano probabilità pari a $1/2$, o anche maggiore di $1/2$ se $P(X = x_{0.5}) \gt 0$.

Può non essere unica e, in alcuni casi, può corrispondere anche ad un intervallo di valori reali.

Se $X$ è **[[Variabili Casuali#Variabili Casuali Continue|continua]]**, la mediana $x_{0.5}$ è tale che $$ F_X(x_{0.5}) = 1/2.$$È il valore dove la *[[funzione di ripartizione]] vale $1/2$* e che *ripartisce a metà l'area unitaria sottesa della [[funzione di densità]]*.

Se $X$ è **[[Variabili Casuali#Variabili Casuali Discrete|discreta]]**, la mediana $x_{0.5}$ è quel valore (anche più di uno) dove *la funzione di ripartizione raggiunge o supera per la prima volta 1/2*.

>[!example] **Esempio**
>*Moneta* ([[Variabili Casuali#^92e4b2|continua]]). Si consideri la variabile casuale $X$ che conta gli esiti testa in tre lanci di una moneta regolare.
>
>Le condizioni $P(X \le x_{0.5}) \ge 1/2$ e $P(X \ge x_{0.5}) \ge 1/2$ risultano verificate per $x_{0.5} = 1, x_{0.5} = 2$ e per ogni valore reale in $(1,2)$.
>
>La variabile casuale $X$ presenta come mediana tutti i valori dell'intervallo [1,2]. La mediana convenzionale è 1.5.

>[!example] **Esempio**
>Sia $X$ una variabile casuale tale che $S_X = \set{-2,0,1,2}, P(X=-2)=P(X=2)=1/4,\ P(X=0)=1/6$ e $P(X=1)=1/3$.
>Si ha allora che $$\begin{gather} 
>P(X \le 1) = P(X = -2) + P(X = 0)+P(X = 1) \gt 1/2, \\ \\
>P(X \ge 1) = P(X = 1) + P(X=2) \gt 1/2. 
>\end{gather}$$Soltanto il valore $x_{0.5} = 1$ soddisfa le due condizioni della definizione ed è quindi mediana di $X$.

>[!example] **Esempio**
>*Variabile casuale esponenziale* ([[Funzione di Densità#^b9319c|continua]]). Si considera la variabile casuale $X \sim \text{Esp}(\lambda)$, che ha [[funzione di ripartizione]] $F_X(x)=1-e^{-\lambda x}$, per $x \ge 0$, e nulla altrove, con $\lambda \gt 0$.
>
>La mediana di $X$ si ottiene risolvendo l'equazione $1-e^{-\lambda x_{0.5}} = 1/2$. In particolare, si ha che $x_{0.5} = \lambda^{-1} \log 2$.

>[!example] **Esempio**
>*Internet* ([[Funzione di Densità#^bca9ef|continua]]). Si considera la variabile casuale $X$ che misura la durata, in un'ora, dei collegamenti internet La funzione di densità di $X$ è rappresentata nella figura sottostante.
>![[Pasted image 20240201023031.png]]
>Poiché è simmetria rispetto a $x = 1/2$, si ha che $x_{0.5} = 1/2$.

***
Riferimenti:
[[Lucidi & materiale/5_prob_varcasual_L5.pdf#page=36&selection=12,0,12,28|5_prob_varcasual_L5, page 36]]

#probabilità 
#ppt-5 
#indici_sintetici 
#indici_sintetici/indici_di_posizione 