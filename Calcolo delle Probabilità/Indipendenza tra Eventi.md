Intuitivamente, due [[Evento|eventi]] si dicono indipendenti se il realizzarsi o meno di uno dei due non modifica la probabilità di realizzazione dell'altro.

Formalmente, due eventi $A$ e $B$ si dicono (**stocasticamente**[^defDizionario1]) **indipendenti**, se $$ P(A \cap B) = P(A)P(B) $$Se, invece, l'eguaglianza non si verifica sono detti **dipendenti**.
Si verifica che:
* se $A$ e $B$ sono non [[Assiomi di Kolmogorov#^c15cc2|trascurabili]], la definizione di indipendenza è equivalente a $P(B|A) = P(B)$ oppure $P(A|B) = P(A)$;
* se $A$ e $B$ sono indipendenti, allora lo sono anche $A$ e $B^C$, $A^C$ e $B$, $A^C$ e $B^C$;
* $\Omega,\ \emptyset$, ed anche ogni evento trascurabile, non indipendenti da qualsiasi evento.


>[!example] **Esempio**
>*Dado* (continua). Si suppone di lanciare un dado equilibrato e si vuole verificare l'indipendenza tra $A = \set{1,2,6}$ e $B = \set{3,6}$.
>
>Nonostante $A$ e $B$ sembrino, a prima vista, dipendenti, si ha che $P(A \cap B) = 1/6,\ P(A) = 3/6$ e $P(B) = 2/6$, da cui segue invece l'indipendenza stocastica.

L'indipendenza è un concetto diverso dall'[[Evento#^74aea2|incompatibilità]]. 
Ad esempio, se due eventi non trascurabili $A$ e $B$ sono incompatibili, allora $P(A \cap B) = 0$ e quindi necessariamente sono dipendenti, poiché $P(A \cap B) \neq P(A)P(B) \gt 0$.

La definizione di indipendenza può venire estesa al *caso di più di due eventi*. In particolare, $A_1, A_2, A_3$ sono indipendenti se: $$ \begin{gather} 
P(A_1 \cap A_2 \cap A_3) = P(A_1)P(A_2)P(A_3),\quad P(A_1 \cap A_2) = P(A_1)P(A_2), \\
\\
P(A_2 \cap A_3) = P(A_2)P(A_3),\quad P(A_1 \cap A_3) = P(A_1)P(A_3)
\end{gather}$$
>[!example] **Esempio**
>*Circuito*. Si consideri un circuito di sei componenti dal funzionamento indipendente. La probabilità di rottura, in un certo intervallo di tempo, è 0.5 per il primo componente, 0.2 per il secondo e 0.1 per i rimanenti quattro
>
>Si determini la probabilità che il circuito si blocchi nell'intervallo di tempo prefissato, nel caso in cui i componenti siano in serie e nel caso siano in parallelo.
>
>Sia $A_i =$ "il componente $i$-esimo si rompe", $i = 1,...,6$, e $B =$ "il circuito si interrompe". Poiché gli eventi $A_i$ sono indipendenti, lo sono anche i corrispondenti complementari.
>
>Se i componenti sono in serie, il circuito si interrompe se almeno un componente si rompe, quindi: $$ P(B) = 1-P(B^C) = 1 - P(A^C_1 \cap ... \cap A^C_6) = 1 - \prod^6_{i=1} P(A^C_i) \doteq 0.738 $$

Se i componenti sono in parallelo, il circuito si interrompe se tutti i componenti si rompono, quindi $$ P(B) = P(A_1 \cap ... \cap A_6) = \prod^6_{i=1} P(A_1) = 0.00001 $$
>[!example] **Esempio**
>*Uomini e donne*. In una stanza ci sono 5 uomini e 5 donne. Si scelgono a caso due persone (senza reinserimento). Quale è la probabilità che siano entrambe donne?
>
>Sia $A_i =$ "L'$i$-esima persona scelta è donna", $i = 1,2$.
>Visto che $P(A_1) = 5/10$ e $P(A_1 | A_1)  = 4/9$, la probabilità cercata è $$ P(A_1 \cap A_2) = P(A_1)P(A_2 | A_1) \doteq 0.22$$ Gli eventi non trascurabili $A_1$ e $A_2$ sono dipendenti poiché $$ P(A_2) = 1/2 \quad \text{e} \quad P(A_2 | A_1) = 4/9$$

>[!example] **Esempio**
>Banca. Una filiale di un istituto bancario a 1210 clienti titolari di conto corrente.
>
>L'ufficio crediti distingue tra *buoni* e *cattivi* clienti, tenendo conto delle eventuali insolvenze. Inoltre, sono noti i dati sull'eventuale possesso della carta di credito.
>
>Le informazioni disponibili vengono sintetizzate nella seguente tabella
>
|  | *cattivo cliente* | *buon cliente* |  |
| ---- | ---- | ---- | ---- |
| con carta di credito | 60 | 520 | 580 |
| senza carta di credito | 21 | 609 | 630 |
|  | 81 | 1129 | 1210 |
>
>Si sceglie casualmente un cliente e si vuole valutare l'eventuale indipendenza tra gli eventi $A =$ "si sceglie un *buon* cliente" e $B =$ "si sceglie un possessore di carta di credito".
>
>Dalla tabella si ricava che $$ \begin{gather}
>P(A) = \frac{1229}{1210} \doteq 0.933,\quad P(B) = \frac{580}{1210} \doteq 0.479, \\
>P(A \cap B) = \frac{520}{1210} \doteq 0.430.
>\end{gather} $$ Poiché $$ P(A \cap B) = 0.43 \neq P(A)P(B) = 0.45, $$si conclude che i due eventi sono dipendenti. Inoltre, la [[probabilità condizionata]] $$P(A|B) = \frac{P(A \cap B)}{P(B)} = \frac{520/1210}{580/1210} = \frac{520}{580} \doteq 0.897$$risulta diversa da $P(A) = 0.933$.

***
Riferimenti:
[[Lucidi & materiale/4_prob_probelem_L4.pdf#page=30&selection=12,0,12,23|4_prob_probelem_L4, page 30]]

[^defDizionario1]: stocasticamente: probabilistico, relativo al calcolo delle probabilità, casuale, aleatorio. (da Wikidizionario)

#probabilità 
#ppt-4 