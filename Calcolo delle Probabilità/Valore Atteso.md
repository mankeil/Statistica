Data una variabile [[Variabili Casuali#Variabili Casuali Discrete|casuale discreta]] o [[Variabili Casuali#Variabili Casuali Continue|continua]] $X$, con [[supporto di una variabile casuale|supporto]] $S_X$ e [[funzione di densità]] di probabilità $f_X$, si chiama **valore atteso** (**medio**) o **media** di $X$, in simboli $E(X)$, la media dei suoi possibili valori ponderati cone le relative probabilità (la relativa funzione di densità di probabilità), ovvero $$E(X) = \sum_{x \in S_X} x f_X(x) = \sum_{x \in S_X} xP(X = x)$$ se $X$ è **discreta**, $$E(X) = \int^{+\infty}_{-\infty} x f_X (x) dx$$se $X$ è **continua**,
purché la serie o l'integrale siano convergenti.

È l'indice di posizione più noto. Usualmente si pone $E(X) = \mu$ e si intende tacitamente che tale valore atteso esista finito.

Sia $X$ una variabile casuale e $Y = g(X)$ una variabile casuale ottenuta come trasformata della $X$, tramite l'applicazione $g(\cdot)$.

Nota, la distribuzione di probabilità di $X$, si può calcolare il valore atteso di $Y$, ovvero $E(Y) = E(g(X))$, senza conoscere la legge di $Y$; infatti, $$E(Y) = \sum_{x \in S_X} g(x)f_X(x)$$se $X$ e $Y$ sono **discrete**, $$ E(Y) = \int^{+\infty}_{-\infty} g(x) f_X(x)dx $$se $X$ e $Y$ sono **continue**.

### Proprietà

Sulla nozione di valore atteso si possono fare considerazioni analoghe a quelle fatte in statistica descrittiva con riferimento alla media aritmetica.

Valgono inoltre le seguenti proprietà, per le quali si ommettono le dimostrazioni essendo sostanzialmente analoghe, per lo meno al caso discreto, a quelle [[Media Aritmetica#Proprietà|viste per la media aritmetica]]:

* **Proprietà di Cauchy**: $\inf\set{x \in S_X} \le E(X) \le \sup\set{x \in S_X}$.
* **Proprietà di baricentro:** $E(X-E(X)) = 0$.
* **Proprietà di linearità**: $E(aX+b) = aE(X)+b$, per ogni $a,b \in \mathbb{R}$
Inoltre si può dimostrare che vale la seguente estensione della proprietà di linearità: date due variabili casuali $X$ e $Y$, per ogni $a,b \in \mathbb{R}$, $$E(aX+bY) = aE(X)+bE(Y);$$tale proprietà si può estendere anche al caso di combinazioni lineari di variabili casuali.

>[!example] **Esempio**
>*Voti*. La seguente tabella di frequenza sintetizza i voti ottenuti da 30 alunni in un compito in classe.
>
| voto | 4 | 5 | 6 | 7 | 8 |
| ---- | ---- | ---- | ---- | ---- | ---- |
| no. alunni | 2 | 3 | 10 | 11 | 4 |
>
>Si può calcolare la [[media aritmetica]] (statistica descrittiva) che corrisponde a 6.4.
>
>Si supponga di avere un'urna con 30 palline, ciascuna contenente il voto di un alunno, e si estragga a caso una pallina.
>
>La variabile casuale $X$, che indica il voto ottenuto con l'estrazione, ha distribuzione di probabilità
>
| $x$ | 4 | 5 | 6 | 7 | 8 |
| ---- | ---- | ---- | ---- | ---- | ---- |
| $P(X=x)$ | 2/30 | 3/30 | 10/30 | 11/30 | 4/30 |
>
>e valore atteso $E(X) = 6.4$ (calcolo delle probabilità). Il valore è lo stesso, ma l'interpretazione è evidentemente diversa.

>[!example] **Esempio**
>*Gioco*. Si lancia una moneta che da testa con probabilità $p \in (0,1)$; se esce testa Tizio paga a Caio un euro, se esce croce è Caio a dover dare a Tizio la stessa somma.
>
>Indicata con $X$ la variabile casuale che descrive il guadagno di Tizio, si ha che $E(X) = (-1)p + 1(1-p) = 1-2p$.
>
>Quindi, $E(X)$ è positivo, nullo o negativo se, rispettivamente, $p \lt 1/2, p = 1/2$ (moneta regolare) o $p \gt 1/2$.

>[!example] **Esempio**
>*Variabile casuale esponenziale* ([[Funzione di Densità#^b9319c|continua]]). Si consideri la variabile casuale $X \sim Esp(\lambda)$. Poiché la funzione di densità è nulla fuori dal supporto $S_X = [0, +\infty)$, $$ E(X) = \int^{+\infty}_{-\infty} x f_X(x)dx = \int^{+\infty}_0 x\lambda e^{-\lambda x} dx = \frac{1}{\lambda} \int^{+\infty}_{0} te^{-1}dt = \frac{1}{\lambda}$$
>avendo operato il cambio di variabile $t = \lambda x$ e poi integrato per parti.

>[!example] **Esempio**
>*Variabile casuale uniforme* ([[Funzione di Densità#^774c2e|continua]]). Si consideri la variabile casuale $X \sim U(0,1)$. Poiché la funzione di densità è nulla fuori dal supporto $S_X = [0,1]$, $$ E(X) = \int^1_0 x \cdot 1 dx = \frac{1}{2} $$

***
Riferimenti:
[[Lucidi & materiale/5_prob_varcasual_L5.pdf#page=30&selection=12,0,12,34|5_prob_varcasual_L5, page 30]]

#probabilità 
#ppt-5 
#indici_sintetici 
#indici_sintetici/indici_di_posizione 