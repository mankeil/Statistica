Analogamente a [[Covarianza|quanto visto in statistica descrittiva]], una misura della dipendenza lineare fra due variabili casuali $X$ e $Y$, con [[Valore Atteso|media]] $E(X)$ e $E(Y)$, è data dalla **covarianza** $$ Cov(X, Y) = E[(X − E(X))(Y − E(Y ))].$$Nel caso di variabili **casuali discrete** $$Cov(X, Y) = \sum_{x_i} \sum_{y_i}(xi − E(X))(y_j − E(Y ))f_{X,Y} (x_i, y_j).$$In alternativa, si può calcolare utilizzando la *formula per il calcolo* $$ Cov(X, Y) = E(XY) − E(X)E(Y),$$dove, nel caso *discreto*, $E(XY) = \sum_{x_i} \sum_{y_j} x_i y_j f_{X,Y} (x_i, y_j).$

Spesso si indica con $\sigma_{XY}$, che ne richiama il legame con la [[Calcolo delle Probabilità/Varianza|varianza]] che corrisponde a $V (X) = \sigma^2_X= \sigma_{XX} = Cov(X, X)$.

Una misura normalizzata della dipendenza lineare è il **coefficiente di correlazione lineare** definito da $$ \rho_{XY} = Cor(X,Y) = \frac{\sigma_{XY}}{\sigma{X} \sigma{Y}}. $$Dalla diseguaglianza di Cauchy-Schwarz si ha $-1 \le \rho_{XY} \le 1$.

Se $\rho_{XY} = 0$, c'è assenza di legame tra $X$ e $Y$, che sono dette **incorrelate** (ma non necessariamente indipendenti).

In particolare questo accade con:
* $(X,Y)$ con componenti $X \sim Ber(p)$, $Y \sim Ber(p)$;
* $(X,Y)$ variabile casuale gaussiana bivariata con componenti $X \sim N(\mu_{X}, \sigma^2_{X})$, $Y \sim N(\mu Y, \sigma^2_Y)$.

Infine, si evidenzia che la covarianza è coinvolta nell'espressione della varianza di una combinazione lineare di $X$ e $Y$. Infatti, per ogni $a,b \in \mathbb{R}$, $$ V(aX + bY) = a^2 V(X)+b^2V(Y) + 2ab Cov(X,Y)$$Casi particolari sono $$ \begin{align}
V(X+Y) & = V(X) + V(Y) + 2 Cov(X,Y) \\ 
V(X-Y) & = V(X) + V(Y) - 2 Cov(X,Y).
\end{align}$$Se $X$ e $Y$ sono *incorrelate*, o a maggior ragione *[[Condizionamento e Indipendenza|indipendenti]]*, le relazioni presentate continuano a valere con $Cov(X,Y) = 0$

***
Riferimenti:
[[Lucidi & materiale/5_prob_varcasual_L5.pdf#page=62&selection=12,0,12,25|5_prob_varcasual_L5, page 62]]

#probabilità 
#ppt-5 
#variabili_casuali/variabili_bivariate 