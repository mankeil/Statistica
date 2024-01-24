Dato un insieme $A$ di $n \in \mathbb{N}$ elementi, il numero dei suoi sottoinsiemi contenenti $k \in \mathbb{N}$ elementi, con $k \le n$, in cui l'ordine non è rilevante, è $$\begin{pmatrix} n \\ k \end{pmatrix} = \frac{n!}{k!(n − k)!} = \frac{n(n − 1) · · · (n − k + 1)}{k!} $$Tali sottoinsiemi sono chiamati **combinazioni semplici** di $n$ oggetti in gruppi di $k$, mentre la quantità $\begin{pmatrix} n \\ k \end{pmatrix}$ è detta **coefficiente binomiale**; per convenzione, $\begin{pmatrix} n \\ 0 \end{pmatrix} = 1$.


>[!example] **Esempio** 
Si vogliono contare le potenziali cinquine, in un’estrazione del lotto su una determinata ruota, che comprendono i numeri 7 e 77. Poiché i due numeri 7 e 77 devono appartenere alla cinquina, è necessario calcolare soltanto il numero di gruppi di tre elementi che si possono formare a partire dagli 88 numeri rimasti. 
La risposta è pertanto $\begin{pmatrix} 88 \\ 3 \end{pmatrix} = 109736$.

Valgono le seguenti proprietà dei coefficienti binomiali: 
* $$\begin{flalign} \binom{n}{k} = \binom{n}{n − k},\quad \forall n, k \in \mathbb{N},\ k ≤ n && \end{flalign}$$
* $$\begin{flalign} \binom{n}{k} = \binom{n-1}{k-1} + \binom{n − 1}{k},\quad \forall n,\ k \in \mathbb{N},\ k ≤ n && \end{flalign}$$
* $$\begin{flalign} (a + b)^n = \sum^n_{k=0} \binom{n}{k}a^k b^{n−k},\quad \text{con}\ a, b \in \mathbb{R}\ \text{e}\ n \in \mathbb{N}^+ && \end{flalign}$$
Quest’ultima formula è chiamata la formula del **binomio di Newton** e consente di determinare lo sviluppo di una qualsiasi potenza del binomio $(a + b)$. Si osservi che, se $a = b = 1$, si ottiene che $\sum^n_{k=0} \binom{n}{k} = 2^n$. Quindi, dato un insieme $A$ costituito da $n \in \mathbb{N}$ elementi, la cardinalità di $P(A)$e $2^n$.

***
da [[Lucidi & materiale/Appendice.pdf#page=4&selection=305,0,383,0|Appendice, page 4]]

#glossario 