>[!premise]- Premessa
>Si considera la situazione in cui, noto il risultato di un qualche esperimento, si vuole determinare la probabilità che esso sia dovuto ad una certa causa, o condizione sperimentale.
>
>Ciò accade, ad esempio, quando l'esperimento avviene in due stadi e, pur essendo noto il risultato finale, non si è a conoscenza del risultato ottenuto al primo stadio.
>
> >[!example] **Esempio**
> >*Due urne*. Si considerano due urne indistinguibili. La prima contiene quattro palline bianche e sei nere, la seconda tre palline bianche e cinque nere.
> >
> >Si sceglie a caso un'urna, senza sapere quale delle due, e si estrae da essa una pallina. Se la pallina è bianca, ci si chiede quale è la probabilità che essa provenga dalla prima urna.
> >
> >Sia $B =$ "la pallina estratta bianca" e $A_i =$ "si sceglie l'urna $i$", $i = 1,2$, si cerca $P(A_1|B)$.
> >
> >Utilizzando la [[Probabilità Condizionata#^a019ca|formula di moltiplicazione]], si ottiene $$ P(A_1 \cap B) = P(A_1)P(B|A_1) = (1/2)(4/10) = 1/5 $$Per la formula delle [[Probabilità Condizionata#^0630c5|probabilità totali]] ha che$$ \begin{gather}
> > P(B) = P(A_1)P(B|A_1) + P(A_2)P(B|A_2) = \\
> >  = (1/2)(4/10) + (1/2)(3/8) = 31/80 
> >  \end{gather}$$Quindi, per la definizione di [[probabilità condizionata]], $$P(A1|B) = \frac{P(A_1 \cap B)}{P(B)} = \frac{1/5}{31/80} \doteq 0.516 $$Si noti che $P(A_1|B) \gt P(A_1)$ e questo trova una giustificazione nel fatto che la prima urna contiene una porzione maggiore di palline bianche ed inoltre si suppone di avere estratto una pallina bianca.
> 

Il **teorema di Bayes** [^appendice1] afferma che:
dato un evento $B$ non trascurabile e una [[partizione]] $A_i,\ i \in I \subseteq \mathbb{N}$, di $\Omega$ costituita da eventi non trascurabili, si ha che, per ogni $i \in I$, $$ P(A_i | B) = \frac{P(A_i)P(B|A_i)}{P(B)} $$Se $P(B)$ non è nota, si può utilizzare la formula della [[Probabilità Condizionata#^0630c5|probabilità totale]] $P(B) = \sum_{j \in I} P(A_j)P(B|A_j)$.
Infatti, per la definizione di [[probabilità condizionata]], applicando la [[Probabilità Condizionata#^3bf48e|formula di moltiplicazione]], si ha che, per ogni $i \in I$, $$ P(A_i|B) = \frac{P(B \cap A_i)}{P(B)} = \frac{P(A_i)P(B|A_i)}{P(B)}$$che è il risultato cercato.

Si possono fare le seguenti considerazioni:
* le probabilità $P(A_i),\ i \in I$, vengono chiamate **probabilità a priori** (**iniziali**) della condizione sperimentale $i$-esima e riflettono quelle che sono le conoscenze disponibili prima della realizzazione dell'esperiemento;
* le probabilità $P(A_i | B),\ i \in I$, vengono chiamate **probabilità a posteriori** (**finali**) e tengono conto del fatto che l'esperimento si è concluso e l'evento $B$ si è realizzato;
* il teorema di Bayes esprime formalmente una procedura coerente di apprendimento dall'esperienza;
* $P(A_i | B)$ risulta proporzionale a $P(A_i)P(B|A_i)$, mentre la quantità $P(B)$, presente al denominatore, è un fattore di normalizzazione;
* $P(A_i|B)$ è chiamata **verosimiglianza** di $A_i$; si può interpretare concettualmente come la verosimiglianza che il verificarsi di $B$ ha attribuito alla condizione sperimentale $A_i$.

>[!example] **Esempio**
>*Linee di produzione*. Un'azienda produce il 30% dei suoi articoli con una prima linea di produzione, che fornisce 8 pezzi difettosi su 100, mentre il restante 70% con una seconda linea, che fornisce 5 pezzi difettosi su 100.
>
>Si sceglie a caso un articolo, senza sapere da quale linea provenga, e viene scartato perché difettoso. Si vuole calcolare la probabilità che provenga dalla prima linea di produzione.
>
>Indicato con $B =$ "l'articolo selezionato è difettoso" e con $A_i =$ "l'articolo selezionato proviene dall'$i$-esima linea", $i = 1,2$, si ha che $P(B|A_1) = 8/100,\ P(B|A_2) = 5/100,\ P(A_1)  = 3/10, P(A_2)=7/10$.
>
>Per il teorema di Bayes, la probabilità cercata è 
>(utilizzando la formula della probabilità totale) $$
\begin{gather} P(A_1|B) = \frac{P(A_1)P(B|A_1)}{\sum_{i \in I}P(A_i)P(B|A_i)} = \\ \\
=\frac{P(A_1)P(B|A_1)}{P(A_1)P(B|A_1)+P(A_2)P(B|A_2)} = \frac{24}{59} \doteq 0.407
\end{gather}$$

>[!example] **Esempio**
>*Fumatori*. Una popolazione presenta il 32% di fumatori. È noto che il 25% dei fumatori e il 5% dei non fumatori è affetto da una patologia respiratoria cronica.
>
>Si sceglie a caso un individuo dalla popolazione. Quale è la probabilità che sia affetto dalla patologia? Se l'individuo risulta ammalato, quale è la probabilità che sia fumatore?
>
>Indicato con $B =$ "l'individuo scelto è ammalato" e con $A =$ "l'individuo scelto è fumatore", si ha che $P(B|A) = 0.25,\ P(B|A^C) = 0.05,\ P(A) = 0.32 ,\ P(A^C) = 0.68$.
>
>Per la formula della probabilità totale e per il teorema di Bayes si ottiene, rispettivamente, $$ \begin{gather} 
>P(B) = 0.32 \cdot 0.25 + 0.68 \cdot 0.25 \doteq 0.114 \\
>P(A|B) = \frac{P(A)P(B|A)}{P(B)} = \frac{0.32 \cdot 0.25}{0.114} \doteq 0.407
\end{gather}$$

>[!example] **Esempio**
>*Spam* ([[Probabilità Condizionata#^e57a3b|continua]]). Si consideri l'esempio delle tre caselle di posta elettronica.
>
>Nell'ipotesi che si riceva un messaggio catalogato come *spam*, si vuole calcolare la probabilità che provenga dalla seconda casella di posta.
>
>Avendo già calcolato in precedenza $P(B) = 0.016$, per il teorema di Bayes la probabilità cercata è $$ P(A_2 | B) = \frac{P(A_2)P(B|A_2)}{P(B)} = \frac{0.2 \cdot 0.02}{0.016} = 0.25 $$

***
Riferimenti:
[[Lucidi & materiale/4_prob_probelem_L4.pdf#page=37&selection=12,0,12,8|4_prob_probelem_L4, page 37]]

[^appendice1]: Thomas Bayes è stato un matematico e ministro presbiteriano britannico. Il teorema che prende il suo nome è stato pubblicato postumo nel 1763.

#probabilità 
#ppt-4 