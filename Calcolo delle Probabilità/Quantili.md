---
aliases:
  - quantile di livello α
---
Sia $\alpha \in (0,1)$, si chiama **quantile di livello $\alpha$** della [[distribuzione di probabilità]] di $X$, o più semplicemente quantile di livello $\alpha$ di $X$, indicato con $x_\alpha$, quel valore $x_a \in \mathbb{R}$ tale che $$\begin{gather} P(X \le x_\alpha) \ge \alpha & \text{e} & P(X \ge x_\alpha) \ge 1-\alpha.\end{gather} $$Quindi, a meno di effetti legati alla discretezza, $x_\alpha$ ripartisce la massa unitaria di probabilità lasciando una porzione pari ad $\alpha$ alla propria sinistra e pari a $1 - \alpha$ alla propria destra.

Può non essere unico e, in alcuni casi, può corrispondere anche ad un intervallo di valori reali.

Se $X$ è una variabile **[[Variabili Casuali#Variabili Casuali Continue|continua]]**, $x_\alpha$ è tale che $$ F_X(x_a) = a $$È il valore dove la [[funzione di ripartizione]] vale $\alpha$ e che ripartisce in due porzioni pari ad $\alpha$ e $1-\alpha$ l'area unitaria sottesa dalla [[funzione di densità]].

Se $X$ è una variabile **[[Variabili Casuali#Variabili Casuali Discrete|discreta]]**, in quantile $x_\alpha$ è quel valore (anche più di uno) dove la funzione di ripartizione raggiunge o supera per la prima volta $\alpha$.

Quindi la mediana corrisponde al quantile di livello $\alpha = 1/2$. Se $\alpha$ è espresso in termini decimali o percentuali si parla allora di **decili** o di **percentili**. Se $\alpha = 1/4,\ 1/2,\ 3/4$, hanno i **quartili**.

>[!example] **Esempio**
>Sia $X$ una variabile casuale tale che $S_X = \set{-2, 0, 1, 2},\ P(X = -2) = P(X=2) = 1/4,\ P(X=0) = 1/6$ e $P(X=1) = 1/3$. Si cerca il quantile di livello $\alpha = 0.4$. Si ha che $$\begin{gather}
>P(X \le 0) = P(X = -2) + P(X = 0) \gt 0.4, \\
>P(X \ge 0) = P(X = 0) + P(X=1) + P(X=2) \gt 0.6.
\end{gather}$$
>
Poiché soltanto il valore 0 soddisfa le due condizioni della definizione, si conclude che $x_{0.4} = 0$.

>[!example] **Esempio**
>*Variabile casuale esponenziale* ([[Funzione di Densità#^b9319c|continua]]). Si considera la variabile casuale $X \sim \text{Esp}(\lambda)$, che ha [[funzione di ripartizione]] $F_X(x) = 1 - e^{-\lambda x}$, per $x \ge 0$, e nulla altrove, con $\lambda \gt 0$.
>
>Il quantile $x_\alpha$ si ottiene risolvendo l'equazione $1-e^{-\lambda x_\alpha} = \alpha$. In particolare, ci ha che $c = -\lambda^{-1} \log(1-\alpha)$.

>[!example] **Esempio**
>*Internet* ([[Funzione di Densità#^bca9ef|continua]]). Si considera la variabile casuale $X$ che misura la durata, in un'ora, dei collegamenti internet degli utenti di una certa compagnia telefonica. La funzione di densità di $X$ è rappresentata nella figura sottostante.
>![[Pasted image 20240201032823.png]]
>Poiché è [[Calcolo delle Probabilità/Simmetria|simmetrica]] rispetto a $x = 1/2$, si può concludere che, per ogni $\alpha \in (0, 0.5)$, l'area della coda di sinistra di $x_\alpha$ coincide con l'area della coda alla destra di $x_{1-\alpha}$.

***
Riferimenti:
[[Lucidi & materiale/5_prob_varcasual_L5.pdf#page=41&selection=12,0,12,8|5_prob_varcasual_L5, page 41]]

 #probabilità 
 #ppt-5 
 #indici_sintetici 
 #indici_sintetici/indici_di_posizione 