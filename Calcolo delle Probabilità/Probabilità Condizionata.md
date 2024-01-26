La **probabilità condizionata** di un evento $B$ rispetto a un evento $A$ è la [[probabilità]] che si verifichi 

Dati due eventi $A$ e $B$, con $P(A) \gt 0$, può essere interessante specificare la probabilità di $B$ nel caso sia noto il realizzarsi di $A$, ossia la probabilità dell'**evento condizionato** $B | A$.
>[!formula]
La probabilità di $B|A$, chiamata **probabilità condizionata** di $B$ dato $A$, è definita ponendo $$ P(B|A) = \frac{P(B \cap A)}{P(A)}$$Intuitivamente, se $A$ si è realizzato, l'unica parte di $B$ che può ancora verificarsi è quella comune anche ad $A$. ^bacbea

La quantità $P(A)$ al denominatore permette di ristabilire le proporzioni, assicurando la normalizzazione. [^nota]

>[!example] **Esempio**
>*Roulette*. Si giocano alla roulette i numeri 7, 23 e 32. Poiché la roulette è suddivisa in 37 settori, numerati da 0 a 36, la probabilità di vincere è $P(B) = 3/37 \doteq 0.081$, con $B = \set{7,23,32}$.
>
>Se la roulette fosse truccata in modo che possano uscire soltanto i numeri complessi tra 0 e 15, posto $A = \set{0,...,15}$, la probabilità di vincita corrisponderebbe a $$ P(B|A) = \frac{P(B \cap A)}{P(A)} = \frac{1/37}{16/37} = \frac{1}{16} \doteq 0.062 $$

>[!example] **Esempio**
>*Da Wikipedia*
>Si consideri questo secondo esempio, la probabilità di ottenere "1" con il lancio di un comune dado (evento $B$) ha probabilità $P(B) = 1/6$ di verificarsi. Sapendo però che il risultato del lancio è un numero tra "4", "5" e "6" (evento $A$), la probabilità $B$ diventa $$ P(B|A) = \frac{P(B \cap A)}{P(A)} = \frac{P(B) + P(A) - P(B \cup A)}{P(A)} = \frac{1/6 + 3/6 - 4/6}{3/6} = 0 $$

Dalla [[Probabilità Condizionata#^bacbea|definizione]] di probabilità condizionata si ottiene la **formula della probabilità composta** (**formula di moltiplicazione**) $$ P(B\cap A) = P(A) P(B|A) $$con $A,\ B$ eventi tali che $P(A) \gt 0$. ^3bf48e

La formula di moltiplicazione si può estendere anche al caso di tre o più eventi. Ad esempio, dati $A_1,\ A_2,\ A_3$, tali che $P(A_1 \cap A_2) \gt 0$, $$ P(A_1 \cap A_2 \cap A_3) = P(A_1)P(A_2|A_1)P(A_3|A_1 \cap A_2)$$  ^a019ca
>[!example] **Esempio**
>*Due palline*. Si consideri l'estrazione, senza reinserimento, di due palline da un'urna contenente dieci palline nere e cinque bianche. Si vuole calcolare la probabilità che esca pallina nera in entrambe le estrazioni.
>
>Indicati con $A_1$ e $A_2$ gli eventi "esce una pallina nera", rispettivamente alla prima e seconda estrazione, si ha che $P(A_1) = 10/15$ e $P(A_2|A_1) = 9/14$.
>
>Utilizzando la formula di moltiplicazione, la probabilità cercata è $P(A_2|A_1) = 10/15 = P(A_1)$ e quindi $P(A_1 \cap A_2) = 4/9$.

Utilizzando alcune relazioni considerate in precedenza, si ottiene il seguente risultato, che risulta molto utile nelle applicazioni.

Dato un evento $B$ e una [[partizione]] $A_i, i \in I \subseteq \mathbb{N}$, di $\Omega$, con $P(A_i) \gt 0$, vale la **formula della probabilità totale** $$ P(B) = \sum_{i \in I} P(B \cap A_i) = \sum_{i \in I} P(A_i) P(B|A_i)$$Infatti, considerando la [[Assiomi di Kolmogorov#^0533a7|formula di addizione]], dal momento che, per la [[Probabilità Condizionata#^3bf48e|formula di moltiplicazione]], $P(B \cap A_i) = P(A_i)P(B|A_i),\ i \in I$, si ottiene immediatamente il risultato. ^0630c5

>[!example] **Esempio**
>*Spam*. Si suppone di possedere tre caselle di posta elettronica.
>È noto che il 70% della posta proviene dalla prima casella, il 20% dalla seconda e il 10% dalla terza.
>
>Dalla prima casella si riceve abitualmente l'1% di messaggi spam, mentre dalle altre due si riceve il 2% e il 5% di messaggi spam, rispettivamente.
>Si vuole calcolare la probabilità di ricevere un messaggio spam.
>
>Si considerino gli eventi $B=$ "ricevere un messaggio spam" e $A_i=$ "ricevere posta dalla casella $i$", con $i=1,2,3$.
>
Evidentemente $\set{A_1,\ A_2,\ A_3}$ è una partizione di $\Omega$ costituita da eventi di probabilità $0.7,\ 0.2$ e $0.1$, rispettivamente.
(Nota: Il rateo di messaggi di spam in % è la probabilità condizionata che arrivi un messaggio di spam).
>
Poiché $$P(B|A_1) = 0.01,\ P(B|A_2) = 0.02,\ P(B|A_3)=0.05,$$utilizzando la formula della probabilità totale, si ottiene che $$ \begin{gather} 
P(B) = \sum^3_{i=1} P(A_1)P(B|A_i) = \\ 
= 0.7 \cdot 0.01 + 0.2 \cdot 0.02 + 0.1 \cdot 0.05 \doteq 0.016 \end{gather}$$

^e57a3b


>[!example] **Esempio**
>*Dado e moneta*. Si suppone di lanciare un dado equilibrato e quindi di lanciare una moneta equilibrata tante volte quanto è il punteggio realizzato dal dado. Si vuole calcolare la probabilità dell'evento $B =$ "si ottengono (almeno) cinque testa nei lanci della moneta".
>
>Si considerino gli eventi $A_i =$ "il punteggio del dado è $i$", con $i = 1,...,6$. Evidentemente, $\set{A_i,\ i = 1,...,6}$ è una partizione di $\Omega$ costituita da eventi di probabilità $1/6$.
>
>Poiché $P(B|A_i) = 0,\ i=1,2,3,4$ e $$ P(B|A_5) = \left( \frac{1}{2} \right)^5,\ P(B|A_5) = \begin{pmatrix} 6 \\ 5 \end{pmatrix} \left( \frac{1}{2} \right)^6$$
utilizzando la formula della probabilità totale si ottiene che $$\begin{gather} P(B) = \sum^6_{i=5} P(A_i)P(B|A_i) = \frac{1}{6} \left( \frac{1}{2} \right)^5 + \frac{1}{6} \begin{pmatrix} 6 \\ 5 \end{pmatrix} \left(\frac{1}{2}\right)^6 = \\ 
= \frac{1}{6} \left(\frac{1}{2}\right)^2 + \frac{1}{6} \left( \frac{6!}{5!(6-5)!} \right) \left(\frac{1}{2}\right)^6 \doteq 0.021 \end{gather}$$dove $\binom{n}{k}$ è il [[coefficiente binomiale]] (quanti sottoinsiemi di cardinalità $k$ possono essere contenuti in un insieme di cardinalità $n$)

***
Riferimenti:
[[Lucidi & materiale/4_prob_probelem_L4.pdf#page=23&selection=12,0,12,24|4_prob_probelem_L4, page 23]]
[Wikipedia - Probabilità condizionata](https://it.wikipedia.org/wiki/Probabilit%C3%A0_condizionata?useskin=vector)

[^nota]:Nota: Consente di esprimere la probabilità in proporzione all'evento condizionante ($A$).

#probabilità 
#ppt-4 