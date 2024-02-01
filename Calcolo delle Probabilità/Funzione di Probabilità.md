>[!premise]- Ripasso %% Rimuovere? definizione forse superflua, presente nei lucidi %%
>![[Variabili Casuali#Variabili Casuali Discrete]]

La corrispondenza tra i possibili valori di $X$ e le rispettive probabilità individua la **funzione di probabilità** (**massa**) $$ f_X(x) = \begin{cases} P(X = x_i) = p_i & \text{se } x = x_i,& \forall i \in I,\\
0 &\text{altrimenti}
\end{cases}$$[^formula1]
Dalla conoscenza di $f_X$ si risale alla [[funzione di ripartizione]] $F_X$ e viceversa, quindi $f_X$ caratterizza la variabile casuale $X$.

Infatti, per ogni $x \in \mathbb{R}$, $$F_X(x) = P(X \le x) = \sum_{i:x_i \le x} p_i$$Il grafico di $F_X(x)$ è una *funzione a gradini*, continua da destra, con salti in corrispondenza degli elementi del [[supporto di una variabile casuale|supporto]] $x_i \in S_X$ e ampiezza del salto da $$ p_i = f_X(x_i) = F_X(x_i) - F_X(x_{i-1})$$La conoscenza di $f_X$ permette spesso una notevole semplificazione nel calcolo di probabilità di eventi relativi a $X$, dal momento che, per ogni $B \subseteq \mathbb{R}$, $$ P(X \in B) = \sum_{i: x_i \in B} f_X(x_i) $$[^formula2]
>[!example] **Esempio**
>*Moneta* ([[Variabili Casuali#^92e4b2|continua]]). Si considera la variabile casuale $X$, che conta il numero di esiti testa in tre lanci di una moneta regolare, e si rappresentano le associate funzioni di probabilità e ripartizione
>![[Pasted image 20240126000238.png]]
>Inoltre, si calcolano facilmente probabilità riferite a $X$, come ad esempio 
> $$ \begin{gather} 
P(X \ge 1)= \sum_{i:x_i\ge1}P(X=x_i) = 1-P(X=0)=7/8, [^nota1] \\
P(X \lt 2) = \sum_{i:x_i \lt 2} P(X = x_i) = F_X(1) = 1/2.
\end{gather}$$
> >[!reminder]- Ripasso
> >Ricorda, i lanci di moneta sono [[Indipendenza tra Eventi|eventi indipendenti]], quindi il numero di risultati possibili è $2^3 = 8$

>[!example] **Esempio**
>*Variabile casuale degenere*. Una **variabile casuale** $X$ è **degenere** nel punto $c \in \mathbb{R}$, in simboli $X \sim D(c)$, se $P(X=c) = 1$. In questo caso $S_X = \set{c}$ e le funzioni di probabilità e di ripartizione corrispondono a $$ f_X(x) =\begin{cases}
>1 & \text{se}\ x = c \\ 0 & \text{se}\ x \neq c \end{cases}\ , \qquad F_X(x) = \begin{cases}
>0 & \text{se}\ x \lt c \\ 1 & \text{se}\ x \ge c \end{cases}\ ,
>$$ con grafico, per il caso $c = 1$,
>![[Pasted image 20240126001749.png]]
>Una variabile casuale degenere descrive un esperimento non aleatorio.

>[!example] **Esempio**
>*Interruzioni*. Sia $X$ una variabile [[Variabili Casuali#Variabili Casuali Discrete|casuale discreta]] che descrive il numero di interruzioni registrate in una linea di produzione di una certa azienda in una settimana. La sua funzione di probabilità è $$ f_X(x) = \begin{cases}
>0.4 & \text{se}\ x = 0 \\
>0.2 & \text{se}\ x = 1 \\
>0.1 & \text{se}\ x = 2 \\
>0.05 & \text{se}\ x = 3 \\
>0.25 & \text{se}\ x = 4 \\
>0 & \text{altrimenti} 
\end{cases}$$con grafico:
![[Pasted image 20240201013632.png]]

^e2fe75


<span style="color:gray; font-weight:300">Altri esempi disponibili nei lucidi.</span> 
***
Riferimenti:
[[Lucidi & materiale/5_prob_varcasual_L5.pdf#page=12&selection=12,0,12,23|5_prob_varcasual_L5, page 12]]

Risorse Esterne:
[Funzione di Probabilità - Wikipedia](https://it.wikipedia.org/w/index.php?title=Funzione_di_probabilit%C3%A0&useskin=vector)

[^formula2]:La probabilità che la variabile casuale discreta $X$ cada nell'insieme $B$ è uguale alla somma delle probabilità che ciascun elemento $x_i$​ nell'insieme $B$ assuma il proprio valore.

[^formula1]:La funzione di probabilità $f_X(x)$ restituisce la probabilità associata a un particolare valore $x$. La funzione di probabilità è zero per tutti gli altri valori che $X$ potrebbe assumere al di fuori di quelli specificati.

#variabili_casuali 
#ppt-4 