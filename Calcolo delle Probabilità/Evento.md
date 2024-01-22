Un **evento** è un sottoinsieme dello [[Spazio Fondamentale]] $\Omega$, cioè ogni elemento dell'insieme delle parti (insieme di tutti i sottoinsieme) di $\Omega$, ovvero di $P(\Omega)$.

Un **evento si realizza** se e solo se si realizza uno degli eventi elementari che lo definiscono.

>[!example] **Esempio**
>*Dado*. Nel caso del lancio del dado $\Omega = \set{1,2,3,4,5,6}$ e sono eventi, ad esempio, $A$ = "Esce un numero dispari" = $\set{1,3,5}$, $B = \set{1,3,6}$, $C$ = "Esce il numero 5" = $\{5\}$, se interpretato come sottoinsieme di $\Omega$ e non come elemento di $\Omega$.
^d07ac2

C'è un evidente analogia tra eventi di uno spazio fondamentale e sottoinsiemi di un dato insieme. 
È quindi possibile, come per questi ultimi, definire alcune **operazioni logiche sugli eventi**.

Dati due eventi $A, B \subseteq \Omega$
* $A^C$ indica l'**evento complementare** ad $A$ e contiene tutti gli eventi elementari che *non appartengono o ad $A$*;
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
[[Lucidi & materiale/4_prob_probelem_L4.pdf#page=8&selection=75,0,91,1|4_prob_probelem_L4, page 8]]

#probabilità 
#ppt-4 