
>[!summary]+ Formula Veloce:
> Siano $u$ e $v$ funzioni differenziabili di $x$ su un intervallo I che contiene $a$ e $b$. Allora: $$\int u \, dv = uv - \int v \, du,$$e $$\int_{x=a}^{x=b} u \, dv = uv \Big|_{x=a}^{x=b} - \int_{x=a}^{x=b} v \, du.$$

Ecco un'integrale semplice che al momento non possiamo valutare:

$$
\int x \cos x \, dx.
$$

È semplice prendere la derivata dell'integranda usando la regola del prodotto, ma non esiste una regola del prodotto per gli integrali. Tuttavia, questa sezione introduce l'integrazione per parti, un metodo di integrazione basato sulla regola del prodotto per le derivate. Ci permetterà di valutare questo integrale.

La regola del prodotto afferma che se u e v sono funzioni di x, allora $(uv)' = u'v + uv'$.

Per semplicità, scriviamo u per u(x) e v per v(x). Supponiamo di integrare entrambi i lati rispetto a x. Questo dà:

$$
\int (uv)' \, dx = \int (u'v + uv') \, dx.
$$

Per il Teorema Fondamentale del Calcolo, il lato sinistro si integra in uv. Il lato destro può essere diviso in due integrali, ottenendo:

$$
uv = \int u'v \, dx + \int uv' \, dx.
$$

Risolvendo per il secondo integrale otteniamo:

$$
\int uv' \, dx = uv - \int u'v \, dx.
$$

Utilizzando la notazione differenziale, possiamo scrivere $du = u'(x) \, dx$ e $dv = v'(x) \, dx$ e l'espressione sopra può essere scritta come:

$$
\int u \, dv = uv - \int v \, du.
$$

Questa è la formula dell'integrazione per parti. A scopo di riferimento, la enunciamo in un teorema.

> [!formula] Teorema: Integrazione per Parti
>
> Siano $u$ e $v$ funzioni differenziabili di $x$ su un intervallo $I$ che contiene $a$ e $b$. Allora: $$\int u \, dv = uv - \int v \, du,$$e $$\int_{x=a}^{x=b} u \, dv = uv \Big|_{x=a}^{x=b} - \int_{x=a}^{x=b} v \, du.$$

> [!example] Esempio:
> Valuta $$
> \int x \cos x \, dx.
> $$La chiave per l'integrazione per parti è identificare parte dell'integranda come "u" e parte come "dv". La pratica regolare aiuterà a fare buone identificazioni, e successivamente introdurremo alcuni principi che aiutano. Per ora, poniamo $u = x$ e $dv = \cos x \, dx$.
>
Ora sostituisci tutto nella formula dell'integrazione per parti, ottenendo:
>$$ \int x \cos x \, dx = x \sin x - \int \sin x \, dx.$$Integrando poi $\sin x$ otteniamo $-\cos x + C$ e la nostra risposta finale è: $$
\int x \cos x \, dx = x \sin x - \cos x + C.
$$ Nota come l'antiderivata contiene un prodotto, $x \sin x$. Questo prodotto è ciò che rende necessaria l'integrazione per parti.
>
L'esempio sopra dimostra come funziona l'integrazione per parti in generale. Cerchiamo di identificare u e dv nell'integrale dato, e la chiave è che di solito vogliamo scegliere u e dv in modo che $du$ sia più semplice di u e $v$ sia sperabilmente non troppo più complicato di $dv$. Questo significa che l'integrale a destra della formula di integrazione per parti, $$\int v \, du,$$ sarà più semplice da integrare rispetto all'integrale originale
>
>$$
\int u \, dv.
>$$
>
Nell'esempio sopra, abbiamo scelto $u = x$ e $dv = \cos x \, dx$. Quindi $du = dx$ era più semplice di u e $v = \sin x$ non era più complicato di $dv$. Pertanto, anziché integrare $x \cos x \, dx$, avremmo potuto integrare $\sin x \, dx$, cosa che sapevamo fare.
>
Un mnemonico utile per aiutare a determinare u è "LIATE", dove
L = Logaritmica, I = Inversa Trig., A = Algebrica (polinomi),
T = Trigonometrica e E = Esponenziale.
>
Se l'integranda contiene sia un termine logaritmico che un termine algebrico, in generale è meglio lasciare che u sia il termine logaritmico, come indicato dal fatto che L precede A in LIATE.

Consideriamo ora un altro esempio.

> [!example] Esempio:
> Valuta $$
> \int x e^x \, dx.
> $$La formula dell'integranda contiene un termine algebrico (x) e un termine esponenziale ($e^x$). Il nostro mnemonico suggerisce di lasciare che u sia il termine algebrico, quindi scegliamo $u = x$ e $dv = e^x \, dx$. Quindi $du = dx$ e $v = e^x$ come indicato dalle tabelle seguenti:
>
Osserviamo che $du$ è più semplice di $u$, mentre non c'è alcun cambiamento passando da $dv$ a $v$. Questo è positivo. La formula dell'integrazione per parti ci dà $$
\int x e^x \, dx = x e^x - \int e^x \, dx.
$$L'integrale a destra è semplice; la nostra risposta finale è $$\int x e^x \, dx = x e^x - e^x + C.$$Nota di nuovo come le antiderivate contengano un termine prodotto.

---
Riferimenti:
[[Lucidi & materiale/apexcalculus.pdf#page=293&selection=6,0,6,19|apexcalculus, page 293]]

*Tradotto e generato da chatGPT*

#appendice
