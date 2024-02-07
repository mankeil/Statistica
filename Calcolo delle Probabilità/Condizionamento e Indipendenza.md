Le componenti marginali $X$ e $Y$ sono indipendenti se ogni evento associato a $X$ è indipendente da ogni evento associato a $Y$. 

Formalmente, $X$ e $Y$ sono (**stocasticamente**) **indipendenti** se $$\begin{align} F_{X,Y} (x, y) = F_X (x)F_Y (y) && \text{per ogni } (x, y) \in \mathbb{R}^2 .\end{align}$$Se, invece, esiste almeno un punto $(x, y)$ per cui questo non vale, $X$ e $Y$ vengono dette **dipendenti**. Se $X$ e $Y$ sono indipendenti, il supporto congiunto è il prodotto cartesiano dei supporti marginali, cioè $S_{X,Y} = S_X \times S_Y$.

Se $(X, Y)$ è **discreta**, la definizione di indipendenza è equivalente a chiedere che, per ogni $(x_i, y_j)  \in S_{X,Y}$, $$ f_{X,Y}(x_i, y_j) = f_X (x_i)f_Y(y_j). $$Utilizzando la notazione introdotta in precedenza, ciò corrisponde a chiedere che, per ogni $(x_i, y_j) \in S_{X,Y}$, $p_{ij} = p_{i+}p_{+j}$.

Data una variabile casuale bivariata $(X, Y)$, può essere interessante determinare la distribuzione di probabilità di una componente condizionatamente ai valori assunti dall'altra.

Se $(X, Y)$ è **discreta**, in accordo con la definizione di probabilità condizionata, si ottiene la funzione di probabilità della **variabile casuale** $X$ **condizionata** a (**dato**) $Y = y_j$, dove $P (Y = y_j ) \gt 0$, in simboli $X | Y = y_j$.

In particolare, per ogni $x_i \in S_{X|Y=y_j}$, si ha $$ f_{X|Y=y_i}(x_i) = P(X=x_i | Y = y_i) = \frac{P(X=x_i, Y = y_j)}{P(Y = y_j)} = \frac{p_{ij}}{p_{+j}}, $$mentre la funzione è nulla altrove. $S_{X|Y=y_j}$ è il **supporto** della variabile casuale condizionata, definito come l'insieme dei valori che $X$ può assumere se $Y = y_j$.

Si ottengono definizioni analoghe per $Y|X = x_i$.

Se $X$ e $Y$ sono *indipendenti*, tutte le distribuzioni condizionate di $X | Y = y_j$, al variare di $y_j$ sono uguali e coincidono con la distribuzione marginale di $X$; analogamente per $Y|X = x_i$.

A partire dalla distribuzione di probabilità della variabile casuale condizionata $X|Y = y_j$, è possibile determinare, con le formule usuali, il **valore atteso condizionato** $$ E(X|Y = y_j) = \sum_{x_i} x_i f_{X|Y=y_j}(x_i) $$e la **varianza condizionata** $$ V(X|Y = y_j) = \sum_{x_i} (x_i - E(X|Y = y_j))^2 f_{X|Y = y_j}(x_i) $$Se $X$ e $Y$ sono *indipendenti*, valore atteso e varianza condizionati sono constanti e coincidono con $E(X)$ e $V(X)$

Si ottengono definizioni analoghe per $Y | X = x_i$.

***
Riferimenti:
[[Lucidi & materiale/5_prob_varcasual_L5.pdf#page=59&selection=12,0,12,30|5_prob_varcasual_L5, page 59]]

#probabilità 
#ppt-5 
#variabili_casuali/variabili_bivariate 