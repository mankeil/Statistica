Per descrivere fenomeni o esperimenti aleatori si considera la nozione di variabile casuale, che fornisce un modello matematico utile anche per le applicazioni statistiche.

Lo [[spazio fondamentale]] $\Omega$ potrebbe non essere un insieme numerico oppure potrebbe non rappresentare in modo chiaro gli aspetti dell'esperimento a cui si è interessati. In alcuni casi $\Omega$ potrebbe essere astratto e molto complesso da specificare.

Le variabili casuali permettono di svincolarsi dallo spazio $\Omega$ e di operare in insiemi numerici dove le probabilità si calcolano mediante somme e integrali.

>[!example] **Esempio**
>L'esperimento del lancio di una moneta non da luogo ad un risultato numerico, poiché $\Omega = \set{T, C}$. Se si considera il numero di esiti "Testa" in $n = 1$ lanci, si ottiene una descrizione numeri del fenomeno in esame.
>In una procedura di controllo della qualità si può non essere interessati all'esito completo dell'esperimento ma soltanto al numero di oggetti che soddisfano opportuni standard di qualità, tra quelli selezionati.
>
>Nel lancio di due dadi, si può prestare attenzione non tanto alla coppia di valori che appaiono sulle facce superiori dei singoli dadi, ma alla somma di tali valori numerici.
>

Dato un [[esperimenti aleatori|esperimento (fenomeno) aleatorio]] descritto da uno spazio fondamentale $\Omega$ e una probabilità $P$, si definisce **variabile casuale** (**aleatoria**) $X$ una *applicazione* da $\Omega$ in $\mathbb{R}$ *misurabile*, cioè tale che sia possibile "probabilizzare" gli eventi ad essa riferiti.

Quindi una variabile casuale è una funzione che, a seconda del risultato dell'esperimento in esame, assume valori numerici a cui è possibile attribuire una probabilità di realizzazione coerente con $P$.

>[!example] **Esempio**
>*Moneta*. Si consideri l'esperimento che consiste nel lanciare tre volte una moneta regolare e si supponga di essere interessati al numero totale degli esiti in testa.
>
>Quindi $\Omega = \set{CCC,CCT,CTC,TCC,CTT,TCT,TTC,TTT}$ e la variabile casuale $X : \Omega \rightarrow R$ associa ad ogni [[eventi elementari|evento elementare]] di $\Omega$ il numero di esiti $T$. Ad esempio, $X(TTC)=2$.
>
>$X$ assume valori in $\set{0,1,2,3}$ e tali valori corrispondono a veri e propri eventi elementari, indicati con la scrittura simbolica $X = i,\ i = 0,1,2,3$.
>
>È immediato concludere che $X = i$ ha probabilità $1/8$, se $i = 0,3$, e $3/8$, se $i = 1, 2$. Si noti che la somma delle probabilità di $X$ è pari a 1.

^5b5547

***
Riferimenti:
[[Lucidi & materiale/5_prob_varcasual_L5.pdf#page=4&selection=12,0,12,17|5_prob_varcasual_L5, page 4]]

#variabili_casuali
#ppt-5