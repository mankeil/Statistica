Si considerano esperimenti che possono essere rappresentati come estrazioni con reinserimento da un'urna di composizione nota.

Ogni estrazione può essere classificata in due categorie incompatibili ed esaustive chiamate, in modo convenzionale, **successo** e **insuccesso** (osservazioni dicotomiche dove, in genere, 1 indica il successo e 0 l'insuccesso): **esperimento bernoulliano**. 

Ogni estrazione è indipendente dalle altre e presenta la stessa probabilità $p \in (0, 1)$ di successo.

Il modello binomiale descrive il *numero di successi in* $n \ge 1$ *esperimenti bernoulliani indipendenti con la stessa probabilità di successo* $p \in (0, 1)$. 

Una applicazione possibile è al *controllo di qualità*: si è interessati al numero di elementi difettosi in un campione casuale di dimensione $n \ge 1$, con $p \in (0, 1)$ la porzione di elementi difettosi.

Un'altra applicazione è al contesto delle indagini di mercato: si è interessati al numero di consumatori che apprezzano un certo prodotto in un campione casuale di dimensione $n ≥ 1$, con $p ∈ (0, 1)$ la porzione di individui che apprezzano il prodotto. 

Una ulteriore applicazione è allo studio delle popolazioni: si è interessati al numero di individui che presentano un certa caratteristica in un campione casuale di dimensione $n ≥ 1$, con $p ∈ (0, 1)$ la porzione di individui portatori della caratteristica. 

Se, come spesso accade nel campionamento da popolazione finita, si effettuano estrazioni senza reinserimento (estrazione in blocco), si può comunque utilizzare il modello binomiale se la popolazione è così elevata da essere considerata *quasi infinita*. 

In questo caso, ha poca importanza se l'estrazione è fatta con o senza reinserimento.

Una variabile casuale $X$ ha distribuzione **binomiale** di parametri $n ≥ 1$ e $p ∈ (0, 1)$, in simboli $X \sim Bi(n, p)$, se $S_X = \set{0, . . . , n}$ e 
Una variabile casuale $X$ ha distribuzione **binomiale** di parametri $n ≥ 1$ e $p ∈ (0, 1)$, in simboli $X \sim Bi(n, p)$, se $S_X = \set{0, . . . , n}$ e $$ f_X(x;n;p) = \begin{cases} 
\binom n x p^x(1-p)^{n-x} & \text{se } x \in S_X \\
0 & \text{altrimenti}
\end{cases} $$dove $n$ indica il numero di prove (esperimenti bernoulliani) indipendenti e p la comune probabilità di successo.

È chiaro che $p^x(1 − p)^{n−x}$ indica la probabilità di osservare $x$ successi e $n − x$ insuccessi, in una specifica configurazione, e il coefficiente binomiale individua il numero di possibili configurazioni con $x$ successi. 

Se $n = 1$ si ha una variabile casuale **bernoulliana**, o **binomiale elementare**, in simboli $Ber(p)$ o $Bi(1, p)$.

Si considerano i grafici delle funzioni di probabilità nel caso in cui $n = 10$ e $p = 0.2, 0.5, 0.8$ e $n = 20$ e $p = 0.5$.
![[Pasted image 20240211004852.png]]

Se le variabili casuali $X_i \sim Ber(p),\ i = 1, . . . , n$, descrivono $n$ esperimenti bernoulliani indipendenti, si può concludere che la variabile casuale somma $X = \sum^n_{i=1} X_i \sim Bi(n,p)$.
Si verifica facilmente che, per ogni $i = 1, . . . , n$, $$ \begin{gather}
E(X_i) = 1 \cdot p + 0 \cdot (1-p) = p, \\ \\
V(X_i) = E(X^2_i) - (E(X_i))^2 = p(1-p).\end{gather}$$ Quindi $$ \begin{gather} E\left( \sum^n_{i=1} X_i \right) = \left(\sum^n_{i=1}E(X_i)=np\right),\\ \\
V(X) = V\left(\sum^n_{i=1} X_i\right)=\sum^n_{i=1} V(X_i) = np(1-p).
\end{gather} $$Infine, è facile verificare che la frequenza campionaria di successo (media campionaria di variabili bernoulliane) $Y = X/n = \sum^n_{i=1} X_1/n$ è tale che $E(Y) = p$ e $V(Y) = p(1-p)/n$.

>[!example] **Esempio**
>*Atleti*. Tra i 100 iscritti ad una associazione sportiva ci sono 30 più alti di 180 cm. Si estrae casualmente un campione di n = 10 atleti con reinserimento.
>
>La variabile casuale $X$ che definisce il numero di atleti che, tra i 10 considerati, è più alto di 180 cm (*successo*) ha distribuzione $Bi(10, 0.3)$. 
>Ci si attende di osservare $E(X) = 3$ atleti con altezza superiore a 180 cm ed inoltre $V (X) = 2.1$ 
>
>La probabilità di estrarre almeno un atleta più alto di 180 cm è $$ P(X \ge 1) = 1 - P(X = 0) = 1 - [10!(0!10!)]0.3^0(1-0.3)^{10}=0.97 $$La probabilità di estrarre due atleti più alti di 180 cm è $$P (X = 2) = [10!/(2!8!)]0.32(1 − 0.3)8 = 0.23.$$Infine, la probabilità di estrarne meno di 4 è $$P(X \lt 4) = \sum^3_{i=0} P(X=x_i) = 0.27 + 0.23 + 0.12 + 0.03 = 0.65. $$

altri esempi sui lucidi.


***
Riferimenti:
[[Lucidi & materiale/6_prob_modelli_L6.pdf#page=8&selection=6,0,6,17|6_prob_modelli_L6, page 8]]

#statistica_inferenziale 
#modelli  