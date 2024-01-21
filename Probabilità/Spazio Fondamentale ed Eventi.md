L'insieme di tutti i possibili risultati di un esperimento aleatorio, indicato con $\Omega$, è chiamato **spazio fondamentale** (**spazio degli eventi elementari** o **spazio campionario**) è l'insieme di tutti i possibili risultati di un esperimento aleatorio.

I singoli risultati vengono chiamati **eventi elementari** e sono supposti disgiunti in senso insiemtistico.

Nonostante lo spazio fondamentale sia noto, non si può individuare con certezza quale evento elementare si realizzerà.

Una volta osservato il fenomeno, o effettuato l'esperimento, uno e un solo evento elementare si sarà realizzato.

$\Omega$ è discreto se costituito da un **numero finito o da un'infinità numerabile** di punti. È invece detto **continuo** se è costituito da un **insieme continuo** di punti.

>[!example] **Esempio**
>Sono discreti gli spazi fondamentali generati dagli esperimenti a) e b), che corrispondono rispettivamente a $\Omega = \{1, 2, 3, 4, 5, 6\}$ e $\Omega = \{1, 2, 3, ...\} = \mathbb{N}^
>+$.
>
Sono continui gli spazi fondamentali generati dagli esperimenti c) e d), che corrispondono rispettivamente a $\Omega = \mathbb{R}^+$ e $\Omega = \mathbb{R}$.

Un **evento** è un sottoinsieme dello spazio fondamentale $\Omega$, cioè ogni elemento dell'insieme delle parti (insieme di tutti i sottoinsieme) di $\Omega$, ovvero di $P(\Omega)$.

Un **evento si realizza** se e solo se si realizza uno degli eventi elementari che lo definiscono.

>[!example] **Esempio**
>*Dado*. Nel caso del lancio del dado $\Omega = \{1,2,3,4,5,6\}$ e sono eventi, ad esempio, $A$ = "Esce un numero dispari" = ${1,3,5}$, $B = {1,3,6}$, $C$ = "Esce il numero 5" = ${5}$, se interpretato come sottoinsieme di $\Omega$ e non come elemento di $\Omega$.

^d07ac2

C'è un evidente analogia tra eventi di uno spazio fondamentale e sottoinsiemi di un dato insieme. È quindi possibile, come per questi ultimi, definire alcune **operazioni logiche sugli eventi**.

Dati due eventi $A, B \subseteq \Omega$
* $A^C$ indica l'**evento complementare** ad $A$ e contiene tutti gli eventi elementari che *non appartengono o ad $A$ o a $B$*;
* $A \cup B$ indica l'**evento unione** tra $A$ e $B$ e contiene tutti gli elementi elementari che *appartengono o ad $A$ o a $B$*;
* $A \cap B$ indica l'**evento intersezione** tra $A$ e $B$ e contiene tutti gli eventi elementari che *appartengono sia ad $A$ che a $B$*
* $A \setminus B$ indica l'**evento differenza** tra $A$ e $B$ e contiene tutti gli eventi elementari che *appartengono ad $A$ ma non a $B$*.
$\Omega$ è detto anche **evento certo** (contiene tutti gli eventi elementari), mentre con il simbolo $\emptyset$ indica l'**evento impossibile**  (non contiene eventi elementari).

Se $A \cap B = \emptyset$, gli eventi $A$ e $B$ si dicono **incompatibili** (**disgiunti**), poiché *non hanno eventi elementari in comune* e quindi non si realizzano contemporaneamente.

Se $A \subseteq B$, allora $A$ **implica** $B$, poiché *tutti gli eventi elementari di $A$ cadono anche in $B$* (il viceversa non è necessariamente vero), quindi la realizzazione di $A$ implica la realizzazione di $B$.

Se $A \subseteq B$ e $B \subseteq A$, gli **eventi** $A$ e $B$ vengono detti **equivalenti**.

>[!example] **Esempio**
*Dado* (continua). Nel caso del lancio del dado, se $A = \{1,3,5\},\ B = \{1,3,6\}$ e $C=\{5\}$, allora $$ \begin{gather} 
A^C=\{2,4,6\},\ A \cup B = \{1,3,5,6\},\ C \subseteq A, \\
A \cap B = \{1,3\},\ A \setminus C = \{1,3\},\ B \cap C = \emptyset
 \end{gather} $$
 
***
Riferimenti:
[[Lucidi & materiale/4_prob_probelem_L4.pdf#page=7&selection=12,0,12,29|4_prob_probelem_L4, page 7]]

#probabilità 
#ppt-4 