---
aliases:
  - variabili discrete
---
Tra le varie tipologie di variabili casuali si considerano quelle discrete, che possono assumere un numero finito o al più numerabili di valori, e quelle continue, che assumono valori in un insieme continuo.

Più precisamente, una **[[variabili casuali|variabile casuale]]** $X$ è **discreta** se esiste un insieme di numeri $\set{x_i}_{i\in I}$, **finito al più numerabile**, tale che $P(X = x_i) = p_i \gt 0$ e $\sum_{i \in I} p_i = 1$; usualmente, $S_X = \set{x_1,\ i \in I}$^[[[supporto di una variabile casuale]]].

La corrispondenza tra i possibili valori di $X$ e le rispettive probabilità individua la **funzione di probabilità** (**massa**) $$ f_X(x) = \begin{cases} P(X = x_i) = p_i & \text{se } x = x_i,& \forall i \in I,\\
0 &\text{altrimenti}
\end{cases}$$Dalla conoscenza di $f_X$ si risale alla [[funzione di ripartizione]] $F_X$ e viceversa, quindi $f_X$ caratterizza la variabile casuale $X$.

Infatti, per ogni $x \in \mathbb{R}$, $$F_X(x) = P(X \le x) = \sum_{i:x_i \le x} p_i$$Il grafico di $F_X(x)$ è una *funzione a gradini*, continua da destra, con salti in corrispondenza degli elementi del supporto $x_i \in S_X$ e ampiezza del salto da $$ p_i = f_X(x_i) = F_X(x_i) - F_X(x_{i-1})$$La conoscenza di $f_X$ permette spesso una notevole semplificazione nel calcolo di probabilità di eventi relativi a $X$, dal momento che, per ogni $B \subseteq \mathbb{R}$, $$ P(X \in B) = \sum_{i: x_i \in B} f_X(x_i) $$
>[!example] **Esempio**
>*Moneta* ([[Variabili Casuali#^5b5547|continua]]). Si considera la variabile casuale $X$, che conta il numero di esiti testa in tre lanci di una moneta regolare, e si rappresentano le associate funzioni di probabilità e ripartizione
>![[Pasted image 20240126000238.png]]
>Inoltre, si calcolano facilmente probabilità riferite a $X$, come ad esempio 
> $$ \begin{gather} 
P(X \ge 1)= \sum_{i:x_1\ge1}P(X=x_i) = 1-P(X=0)=7/8, \\
P(X \lt 2) = \sum_{i:x_i \lt 2} P(X = x_i) = F_X(1) = 1/2.
\end{gather}$$

>[!example] **Esempio**
>*Variabile casuale degenere*. Una **variabile casuale** $X$ è **degenere** nel punto $c \in \mathbb{R}$, in simboli $X \sim D(c)$, se $P(X=c) = 1$. In questo caso $S_X = \set{c}$ e le funzioni di probabilità e di ripartizione corrispondono a $$ f_X(x) =\begin{cases}
>1 & \text{se}\ x = c \\ 0 & \text{se}\ x \neq c \end{cases}\ , \qquad F_X(x) = \begin{cases}
>0 & \text{se}\ x \lt c \\ 1 & \text{se}\ x \ge c \end{cases}\ ,
>$$ con grafico, per il caso $c = 1$,
>![[Pasted image 20240126001749.png]]
>Una variabile casuale degenere descrive un esperimento non aleatorio.

<span style="color:gray; font-weight:300">Altri esempi disponibili nei lucidi.</span> 
***
Riferimenti:
[[Lucidi & materiale/5_prob_varcasual_L5.pdf#page=12&selection=12,0,12,23|5_prob_varcasual_L5, page 12]]

#variabili_casuali 
#ppt-4 