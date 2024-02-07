Nelle applicazioni, è assai frequente dover prendere in considerazione più di una variabile casuale contemporaneamente

Dal punto di vista concettuale la trattazione è molto simile al caso univariato, tuttavia dal punto di vista matematico vi sono delle difficoltà aggiuntive, basti pensare che sia la [[funzione di ripartizione]] che [[Funzione di Densità|quella di densità]] (probabilità) sono funzioni di più variabili. 

Una **variabile casuale multivariata** (**vettore aleatorio**) $(X_1, . . . , X_n)$ è un vettore i cui elementi sono variabili casuali.

>[!example]+ **Esempio**
>*Campione bernulliano*. Si svolgono $n$ esperimenti bernoulliani indipendenti con la stessa probabilità di successo $p$. L'esperimento nel suo complesso è descritto da una variabile casuale multivariata $(X_1, . . . , X_n)$, dove $X_i \sim Ber(p)$, $i = 1, . . . , n$. Questa è la situazione che si presenta tipicamente nella statistica inferenziale.

 Si limita la trattazione alle variabili **casuali bivariate**, che tuttavia risulta sufficiente per introdurre tutti i concetti che sono importanti per il caso generale.

Una **variabile casuale bivariata** $(X, Y)$ risulta specificata dalla sua **funzione di ripartizione congiunta** $$\begin{align} F_{X,Y}(x,y) = P(X \le x, Y \le y), && (x,y) \in \mathbb{R}^2\end{align}$$
Inoltre, il **supporto congiunto** $S_{X,Y}$ è dato dall'insieme dei punti $(x, y) \in \mathbb{R}^2$ nei cui intorni si possono osservare valori per $(X, Y)$ con probabilità strettamente positiva.

Dalla conoscenza della funzione di ripartizione congiunta si ottiene la **funzione di ripartizione marginale** delle due componenti  $X$ e $Y$; ad esempio, per la componente marginale $X$ $$\begin{align} F(x) =\lim_{y \rightarrow + \infty} F_{X,Y}(x,y), && x \in \mathbb{R}\end{align}$$e analogamente per $F_Y(y)$.

Si considera il **caso discreto**; quando presentato si piò estendere al caso continuo con opportune attenzioni.

Una **variabile casuale bivariata** $(X, Y)$ è **discreta** se esiste un insieme di coppie di numeri reali $\set{(x_i, y_i)}_{(i,j) \in I \times J}$, *finito o al più numerabile*, tale che $P(X = x_i, Y=y_i) = p_{ij} \gt 0$; usualmente, $S_{X,Y} = \set{(x_i, y_i), (i,j) \in I \times J}$.

Analogamente al caso univariato, risulta definita la **funzione di probabilità** (**massa**) **congiunta** $$ f_{X,Y} (x,y) = \begin{cases}p_{ij} & \text{se } (x,y)=(x_i, y_i), & \forall(i,j) \in I \times J, \\ 0 & \text{altrimenti.}\end{cases} $$Dalla conoscenza di $f_{X,Y}$ si risale facilmente alla funzione di ripartizione congiunta $F_{X,Y}$ e viceversa.

Quindi anche $f_{X,Y}$ caratterizza la variabile casuale bivariata $(X, Y )$ e permette il calcolo delle probabilità di eventi ad essa associati. 

$f_{X,Y}$ può essere rappresentata mediante una *tabella a doppia entrata*, analoga alle [[Tabella di Contingenza|tabelle di contingenza]], che fornisce la probabilità $p_{ij}$ riferite alle coppie $(x_i, y_j)$, $i,j \in I \times J$.

Una variabile casuale bivariata $(X, Y )$ è un vettore che ha, come **componenti marginali**, le variabili casuali univariate $X$ e $Y$.

In precedenza si è visto come determinare la **funzione di ripartizione marginale** di $X$ e di $Y$ a partire dalla funzione di ripartizione congiunta. 
Il **supporto marginale $S_X$** corrisponde, intuitivamente, a tutti i possibili valori della componente $X$; analogamente per $S_Y$.

Data una **variabile casuale bivariata discreta** $(X, Y )$, con funzione di probabilità congiunta $f_{X,Y}$ , si può ricavare facilmente la funzione di **probabilità marginale** di $X$, poiché per ogni $x_i \in S_X$ $$ P(X=x_i) = \sum_{j \in J} P(X = x_i, Y=y_i) = \sum_{j \in J} p_{ij} = p_{i+} $$Analogamente, per la componente $Y$ $$ \begin{align} P(Y=y_j) = \sum_{i \in I} = p_{+j}, && y_j \in S_Y \end{align}$$Se si considera la rappresentazione di $f_X,Y$ mediante una tabella a doppia entrata, la funzione di probabilità marginale di $X$ (di $Y$) si ottiene calcolando i totali di riga (di colonna). 

A partire dalla distribuzione marginale delle due componenti si possono calcolare [[valore atteso]] e [[Calcolo delle Probabilità/Varianza|varianza]], che vengono chiamati **valore atteso marginale** e **varianza marginale** di $X$ e di $Y$. 

Viene ora rappresentata in generale una tabella a doppia entrata con le probabilità congiunte e marginali associate a $(X, Y)$.
![[Pasted image 20240205212236.png]]

***
Riferimenti:
[[Lucidi & materiale/5_prob_varcasual_L5.pdf#page=54&selection=12,0,12,27|5_prob_varcasual_L5, page 54]]

#probabilità 
#ppt-5 
#variabili_casuali/variabili_bivariate