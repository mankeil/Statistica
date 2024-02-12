Dato un [[Campioni Casuali Semplici|campione casuale semplice]] $X_1, . . . , X_n$, la **distribuzione di probabilità** delle singole [[variabili casuali]] dipende dalla natura dei dati e del fenomeno oggetto di indagine. 

Ad esempio, per dati binari sarà naturale ipotizzare $X_i \sim Ber(p)$, per misurazioni $X_i \sim N (μ, \sigma^2)$, per conteggi $X_i \sim P (\lambda)$, per tempi di funzionamento $X_i \sim Esp(\lambda)$, ecc. Queste distribuzioni di probabilità possono rappresentare una buona approssimazione della realtà.

La distribuzione assunta per le variabili casuali del campione dipende da costanti ignote dette **parametri**; ad esempio, le quantità $p, \mu, \sigma^2, \lambda,$ ecc.

Nell'*inferenza statistica parametrica* si assume che la distribuzione delle variabili casuali del campione sia nota a meno dei valori dei *parametri*, che corrispondono tipicamente agli *aspetti di interesse dell'analisi*.

Le assunzioni viste, ed elencate nel seguito, definiscono un **modello statistico parametrico** per i dati di un campione casuale semplice: 
* le variabili casuali $X_1, . . . , X_n$ sono [[Indipendenza tra Eventi|indipendenti]]; 
* tutte le $X_i$ hanno la stessa [[distribuzione di probabilità]] (come detto in precedenza, questa ipotesi può anche essere rilassata); 
* tale distribuzione è nota a meno dei valori di uno o più parametri, indicati genericamente come $\theta = (\theta_1, . . . , \theta_d),\ d \ge 1$. 

Scopo dell'inferenza statistica parametrica è utilizzare i dati osservati $x_1, . . . , x_n$ per ottenere informazioni su $\theta$, i cui possibili valori appartengono ad un certo insieme $\Theta$, chiamato **spazio parametrico**. ^5767cb

Il supporto congiunto di $X_1, . . . , X_n$ è detto **spazio campionario** e corrisponde all'insieme dei possibili campioni $x_1, . . . , x_n$ che si possono osservare.

Le tre assunzioni citate in precedenza non è detto che siano soddisfatte nella pratica, ma possono rappresentare una *descrizione semplice e operativamente utile di una realtà complessa*. 

La **scelta del modello** è molto importante, poiché le conclusioni inferenziali dipendono fortemente dalle assunzioni fatte. 

Nella specificazione del modello statistico parametrico è importante considerare: 
* la natura dei dati (qualitativi o quantitativi, discreti o continui, ecc.);
* gli aspetti notevoli presenti nei dati come, ad esempio, posizione, variabilità, simmetria, curtosi, ecc.;
* tutte le informazioni sul meccanismo generatore dei dati. 
Esistono anche **modelli per dati dipendenti** e/o **non identicamente distribuiti** (ad esempio per serie storiche e spaziali) e modelli che prescindono dalla forma della distribuzione di probabilità delle variabili casuali del campione (**modelli non parametrici**).

esempi: [[Lucidi & materiale/7_StatInf_statcamp_L7.pdf#page=17&selection=8,0,8,7|7_StatInf_statcamp_L7, page 17]]

## Verifica del Modello
In alcuni casi, soprattutto per dati continui, la specificazione del modello statistico parametrico può non essere banale, ed è allora necessario procedere ad un **controllo empirico del modello**. 

A tal fine, come visto nel caso del modello normale, si possono utilizzare alcuni strumenti già considerati in precedenza, come ad esempio:
* l'**[[Istogramma|istogramma delle frequenze relative]]** e la **[[stima della densità]]**;
* i grafici dei quantili (**[[q-q plot]]**). 

L'*istogramma* e la *stima della densità* basate sui dati campionari possono essere interpretate, in ambito inferenziale, come **stime della [[funzione di densità]]**. 

Tali stime sono valide a prescindere da quale sia la vera distribuzione dei dati e sono tanto più precise quanto più l'informazione campionaria aumenta.

***
Riferimenti:
[[Lucidi & materiale/7_StatInf_statcamp_L7.pdf#page=13&selection=8,0,8,30|7_StatInf_statcamp_L7, page 13]]

#statistica_inferenziale 
#modelli