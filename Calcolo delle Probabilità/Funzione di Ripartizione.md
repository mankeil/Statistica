La misura di probabilità riferita agli eventi $X \in B,\ B \subseteq \mathbb{R}$, associati alla [[Variabili Casuali|variabile casuale]] $X$, soddisfa gli [[assiomi di Kolmogorov]] ed è detta **distribuzione (legge) di probabilità** di $X$.

In genere, non si fa menzione dello spazio di partenza e si identifica una variabile casuale $X$ con la sua distribuzione di probabilità.

Due variabili casuali $X$ e $Y$ sono dette **identicamente distribuite**, in simboli $X \sim Y$, se $P(X \in B) = P(Y \in B)$, per ogni $B \subseteq \mathbb{R}$.

Per specificare la distribuzione di probabilità di una variabile casuale $X$ si considera la nozione di **funzione di ripartizione**, intesa come un'applicazione $F_X : \mathbb{R} \rightarrow [0,1]$, tale che $$ F_X{x} = P(X \le x),\quad x \in \mathbb{R} $$La conoscenza di $F_X$ permette di calcolare, eventualmente con procedimenti di limite, tutte le probabilità $P(X \in B),\ B \subseteq \mathbb{R}$.
In particolare, per ogni $a,b \in \mathbb{R}, a \lt b$, $$
\begin{gather}
 P(a \lt X \le b) = F_X(b) - F_X(a),\ P(X \gt a) = 1-F_X(a) \\
 P(X = b) = F_X(b) - \lim_{x \rightarrow b^-} F_X(x)
 \end{gather} $$ La funzione di ripartizione verifica le tre seguenti **proprietà caratterizzanti**:
 * $F_X$ è monotona non decrescente;
 * $F_X$ è continua da destra;
 * $F_X$ è tale che $\lim_{x \rightarrow - \infty} F_X(x) = 0$ e $\lim_{x \rightarrow + \infty} F_X(x) = 1$.

Perciò, $F_X$ non è necessariamente continua anche da sinistra e quindi continua in ogni punto.

Si può dimostrare che $F_X$ non è necessariamente continua anche da sinistra e quindi continua in ogni punto.

Si può dimostrare che $F_X$ è continua nei punti in cui $P(X = x) = 0$ e discontinua nei punti in cui $P(X = x) \gt 0$, che sono al più un'infinità numerabile.

Vengono riportati due esempi di funzioni di ripartizione
![[Pasted image 20240124234314.png]]
L'insieme di tutti i possibili valori della variabile casuale $X$ corrisponde usualmente alla nozione di supporto.

Il **supporto** di $X$, indicato con $S_X$, è l'insieme dei punti $x \in \mathbb{R}$ in cui intorni sono eventi di probabilità strettamente positiva, cioè $$S_X = \set{x \in \mathbb{R}:\forall \varepsilon \gt 0,\ P(x-\varepsilon \lt X \lt x+\varepsilon)\gt0}$$

>[!example] **Esempio**
>*Moneta* ([[Variabili Casuali#^5b5547|continua]]). Si considera il lancio della moneta ripetuto per tre volte. In questo caso, $S_X = \set{0,1,2,3}$ e $P(X = 0) = P(X = 3) = 1/8,\ P(X = 1) = P(X = 2) = 3/8$.

***
Riferimenti:
[[Lucidi & materiale/5_prob_varcasual_L5.pdf#page=8&selection=12,0,12,24|5_prob_varcasual_L5, page 8]]

#probabilità 
#ppt-5 
#variabili_casuali 
