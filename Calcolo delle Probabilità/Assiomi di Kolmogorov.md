Dato uno [[spazio fondamentale]] $\Omega$, si considerano tutti gli [[evento|eventi]] di interesse: $\Omega,\ \emptyset,\ A,\ B,\ C$, etc. In alcuni casi si considerano tutti i possibili eventi (sottoinsiemi di $\Omega$).

La **probabilità è una misura** che associa ad ogni evento $A \subseteq \Omega$ un numero reale, che indica la sua possibilità di realizzazione. ^bd07ea

Seguendo l'impostazione assiomatica di Kolmogorov, una **misura di probabilità** $P$ deve essere tale che:
* A1. **assioma di non negatività**: per ogni evento $A,\ P(A) \ge 0$;
* A2. **assioma di normalizzazione**: $P(\Omega) = 1$; ^71fbeb
* A3. **assioma di $\sigma-$additività** (additività numerabile): per ogni collezione finita o al più numerale di eventi
	$A_i$, $i \in I \subseteq \mathbb{N}$, tali che $A_i \cap A_j = \emptyset, i \ne j$, si ha che $P(\bigcup_{i \in I} A_i) = \sum_{i \in I} P(A_i)$. [^nota]
	  In altre parole, l'unione di una collezione numerabile di eventi disgiunti è la somma delle corrispondenti probabilità. 
Dall'assioma A3, discende che, se $A \cap B = \emptyset$, allora $P(A \cup B) = P(A)+P(B)$ (additività semplice).

Un **evento** $A$ tale che **$P(A) = 0$** è detto **trascurabile**.
Un **evento** $A$ tale che **$P(A) = 1$** è detto **quasi certo**. ^c15cc2


>[!example] **Esempio**
>*Dado* ([[Esperimenti Aleatori#^d07ac2|continua]]). Nel caso del lancio di un dado regolare, lo spazio fondamentale è $\Omega = \set{i : i = 1, . . . , 6}$ e ogni faccia ha la stessa probabilità di uscire. 
>
>In accordo con tale congettura, si associa ad ogni [[eventi elementari|evento elementare]] i un peso $p_i = 1/6,\ i = 1, . . . , 6$, e, dato un generico evento $A$, $P(A) =\sum_{i \in A} p_i$.
>
>Se $A = \set{1, 3, 5}$, allora $P (A) = 1/6 + 1/6 + 1/6 = 1/2$, che corrisponde alla somma dei pesi degli eventi elementari che compongono $A$. 

>[!example] **Esempio**
>*Dado* ([[Esperimenti Aleatori#^d07ac2|continua]]). Si consideri l'esperimento che consiste nel lanciare un dado regolare. Si è interessati al numero di lanci necessari per ottenere l'esito 6 per la prima volta. In questo caso $\Omega = \mathbb{N}^+$.
>Si può pensare di associare ad ogni evento elementare $i \in \mathbb{N}^+$, "l'esito 6 si verifica per la prima volta al lancio $i$-esimo", il peso $p_i = (5/6)^{i-1} (1/6)$, che traduce il fatto che ci sono $i-1$ insuccessi prima di osservare l'esito 6 per la prima volta.
>
>Anche in questo caso, dato un evento $A$, $P(A) = \sum_{i \in A}p_i$.
>
>Se si ha l'evento $A = \{2,4,6,...\}$, "l'esito 6 si verifica per la prima volta in un numero pari di lanci", allora $P(A) = \sum^{+\infty}_{i=1} p_{2i}$.

Questi due esempi suggeriscono il seguente **criterio costruttivo per definire misure di probabilità** che soddisfano i tre assiomi di Kolmogorov, nel caso di esperimenti con **$\Omega$ finito o numerabile**.

Ad ogni [[eventi elementari|evento elementare]] $\omega_i \in \Omega$ si associa un peso $p_i$ tale che $p_i \gt 0$ e $\sum_i p_i = 1$ e si definisce la misura di probabilità $P$ tale che, per ogni evento $A,\ P(A) = \sum_{i \in A} p_i$. [^nota2]

In altre parole ==ad ogni evento elementare si associa un peso==, ==maggiore di 0==, dove ==la somma totale dei pesi di tutti gli eventi elementari è uguale a 1==.
La misura di probabilità ==$P$ è uguale alla somma dei pesi di tutti gli eventi elementari contenuti in $A$==.

In entrambi gli esempi vengono soddisfatte le condizioni sui pesi $p_i$.

Se $\Omega$ è **finito** e gli **eventi elementari** sono **equiprobabili**, come ad esempio nel caso del singolo di un dado regolare, il criterio evidenziato in precedenza corrisponde alla **definizione classica di probabilità**.

Infatti, se $\Omega$ è costituito da $n$ eventi elementari equiprobabili e $A = \{\omega_i, i \in I\}$, con $I \subseteq \{1,...,n\}$, allora $p_i = 1 / n,\ i=1,...,n$, e $$ P(A) = \sum_{i \in I} \frac{1}{n} = \frac{\text{no. casi favorevoli ad } A}{\text{no. casi possibili}}$$ Quando si parla di "scelta a caso di un elemento di un insieme" $\Omega$ finito, si intende implicitamente che tutti gli eventi elementari sono ugualmente probabili.

In molti casi bisogna fare attenzione a definire in modo corretto gli eventi elementari.

## Conseguenze degli Assiomi

Si presentano alcuni risultati che sono *conseguenze* immediate degli *assiomi di Kolmogorov*.
1. $P(\emptyset) = 0$. 
    Infatti, per il secondo e terzo assioma, $$ 1 = P(\Omega) = P (\Omega \cup \emptyset) = P(\Omega) + P(\emptyset) = 1 + P(\emptyset)$$da cui $P(\emptyset)=0$.
2. Per ogni evento $A,\ P(A^C) = 1 - P(A)$. Dove $A^C$ è l'[[Evento#^5e6f30|evento complementare]]
    Infatti, per il secondo e terzo assioma $$ 1 = P(\Omega) = P(A \cup A^C) = P(A) + P(A^C) $$da cui $P(A^C) = 1-P(A)$. 
3. Se $A \subseteq B$, allora $P(A) \le P(B)$ e $P(B \setminus A) = P(B) - P(A)$.
    Infatti, per il terzo assioma $$P(B) = P((B \setminus A) \cup A) = P(B \setminus A) + P(A)$$ da cui si ottengono entrambi i risultati.
4.  Dati gli eventi $A$ e $B$, $P(A \cup B) = P(A) + P(B) - P(A \cap B)$.
      Poiché $$A \cup B = (A \cap B) \cup [B \setminus (A\cap B)] \cup [A \setminus (A \cap B)] $$il risultato si ottiene dalla seguente relazione $$P(A \cup B) = P (A \cap B) + P(B) - P(A \cap B) + P(A) - P(A \cap B)$$ ![[Pasted image 20240121203745.png]]
5. Dato un evento $B$ e una [[partizione]] $A_i,\ i \in I \subseteq \mathbb{N}$, di $\Omega$, allora $P(B) = \sum_{i \in I} P(B \cap A_i)$ (**formula di addizione**).
    Poiché gli eventi $A,\ i \in I$, sono incompatibili e la loro unione da $\Omega$, anche gli eventi $B \cap A_i,\ i \in I$, sono incompatibili e per il terzo assioma si ha che $$ \begin{gather}
   P(B) = P(B \cap \Omega) = P \left(B \cap \bigcup_{i \in I} A_i \right) = \\
   = P \left( \bigcup_{i \in I} B \cap A_i \right) = \sum_{i \in I} P(B \cap A_i)
   \end{gather}$$![[Pasted image 20240121204449.png]]
>[!reminder]- Ripasso
   >L'insieme delle partizioni ricopre tutto $\Omega$: $\bigcup^n_{i=1} A_i = \Omega$ ^0533a7

>[!example] **Esempio**
>*Lotteria*. Una lotteria è costituita 1000 biglietti, di cui 5 vincenti. Si scelgono a caso 10 biglietti. Si vuole determinare la probabilità di $A =$ "un biglietto vincente".
>
>Tutti i gruppo di dieci biglietti hanno la stessa probabilità di venire estratti. Quindi, utilizzando la definizione classica di probabilità, $$ P(A) = \frac{\begin{pmatrix} 5 \\ 1 \end{pmatrix} \begin{pmatrix} 995 \\ 9 \end{pmatrix}}{\begin{pmatrix} 1000 \\ 10 \end{pmatrix}} \doteq 0.048 $$ Per $B$ = "almeno un biglietto vincente", conviene determinare la probabilità dell'evento complementare "nessun biglietto vincente" $$ P(B^C) = \frac{\begin{pmatrix} 5 \\ 0 \end{pmatrix} \begin{pmatrix} 995 \\ 10 \end{pmatrix}}{\begin{pmatrix} 1000 \\ 10 \end{pmatrix}} \doteq 0.951$$ da cui si ricava che $P(B) = 1 - 0.951 = 0.049$.

>[!example] **Esempio**
>*Indirizzi*. Una rete aziendale è costituita da un server e dieci PC. Quando un PC accede alla rete, riceve un indirizzo IP scelto in modo casuale tra 200 disponibili.
>
>Nell'ipotesi che tutti e dieci i PC accedano insieme alla rete, quale è la probabilità che il server abbia assegnato almeno due indirizzi IP identici?
>
>I casi elementari equiprobabili sono le sequenze ordinate di 10 indirizzi scelti tra i 200 disponibili e corrispondono alle disposizioni con ripetizione di 200 elementi in gruppi di 10, cioè $200^10$.
>
>Poiché le configurazioni favorevoli all'evento complementare "tutti i PC hanno indirizzo diverso" sono date dalle disposizioni semplici di 200 elementi in gruppi di 10, si conclude che $$ 1 - (200!/190!) / (200^{10}) \doteq 0.204 $$ è la probabilità dell'evento cercato.

>[!example] **Esempio**
>*Dadi*. Si lanciano tre dadi regolari, uno rosso, uno verde e uno nero, e si vuole calcolare la probabilità dell'evento $A =$ "almeno due lati presentano la cifra sei".
>
>Le possibili terne di risultati sono $6^3 = 216$. Dal momento che i dadi sono regolari, tutte le terne hanno la stessa probabilità di presentarsi e tale probabilità corrisponde a $1/216$.
>
>Le terne favorevoli all'evento $A$ sono date da:
>* 1 terna con tutti sei;
>* 5 terne con sei nei dadi rosso e verde, e uno nei restanti cinque numeri del dado nero;
>* 5 terne con sei nei dadi rosso e nero e uno dei restanti cinque numeri nel dado verde;
>* 5 terne con sei nei dadi nero e verde e uno dei restanti cinque numeri nel dado rosso.
>  
Quindi la probabilità cercata è $P(A) = 16/216 = 0.006$.

***
Riferimenti:
[[Lucidi & materiale/4_prob_probelem_L4.pdf#page=12&selection=12,0,12,25|4_prob_probelem_L4, page 12]]
[UnInsubria - Laboratorio Virtuale di Probabilità e Statistica](https://www.eco.uninsubria.it/VL/VL_IT/prob/prob4.html#:~:text=dell%27unione%20di%20una%20collezione%20finita%20o%20infinita%20ma%20numerabile%20di%20eventi%20disgiunti%20%C3%A8%20la%20somma%20delle%20corrispondenti%20probabilit%C3%A0.)

[^nota]:Nota: $A$ rappresenta un evento non elementare, mentre $A_i, i \in I$ rappresenta una collezione di eventi. $A_i,\ i = n$ invece rappresenta un'evento parte della collezione alla posizione $n$.

[^nota2]:Nota: $\sum_{i \in A} p_i$ è uguale a scrivere $\sum_{\omega_i \in A} p_i$, rappresenta sempre la somma dei pesi degli eventi elementari contenuti in A.

#probabilità 
#ppt-4 