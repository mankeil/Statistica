Il modello Poisson descrive *problemi di conteggio* quando non c'è una limitazione superiore per il supporto o problemi in cui tale limitazione è praticamente irrilevante.

Sotto alcune ipotesi, descrive il *numero di arrivi o accadimenti* di un evento di interesse (*successo*) in un intervallo di tempo (o anche su una superficie) di dimensione fissata. 

Una variabile casuale *$X$* ha distribuzione **Poisson** con parametro $λ > 0$, in simboli $X ∼ P (λ)$, se $S_X = \mathbb{N}$ e $$fX (x; λ) = \begin{cases} λ^xe−λ/x! & \text{se } x ∈ S_X \\ 0 & \text{altrimenti} \end{cases} $$Si dimostra che $E(X) = λ$ e $E(X^2) = λ^2 + λ$, da cui si ottiene che $V (X) = E(X^2) − (E(X))^2 = λ^2 + λ − λ^2 = λ$. Quindi, media e varianza coincidono e corrispondono al parametro $λ$.
