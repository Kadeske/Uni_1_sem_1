L'**operazione di limite** in **analisi matematica** serve a descrivere il comportamento di una funzione in prossimità di un punto, in particolare di un punto di accumulazione per il suo dominio. Questo concetto è fondamentale per analizzare cosa succede a una grandezza dopo un lungo periodo di tempo (**comportamento asintotico** o **divergenza**) o per valori specifici della variabile indipendente.

Il limite di una funzione $f(x)$ per $x$ che tende a un punto $x_0$ si indica con la notazione:
$$
\lim_{x \to x_0} f(x) = l
$$
Dove **"l"** rappresenta il valore a cui la funzione si avvicina quando $x$ si avvicina a $x_0$.

Esistono diverse tipologie di limite:

- [**Limite finito per**](Limite%20finito%20che%20tende%20ad%20un%20numero) $x \to x_0$: si ha quando la funzione si avvicina a un valore finito $l$ quando $x$ si avvicina a $x_0$. La definizione formale prevede che per ogni $\varepsilon > 0$, esiste un $\delta > 0$ tale che se la distanza tra $x$ e $x_0$ è minore di $\delta$, allora la distanza tra $f(x)$ e $l$ è minore di $\varepsilon$.

- [**Limite infinito per**](Limite%20infinito%20che%20tende%20ad%20un%20numero) $x \to x_0$: si ha quando la funzione cresce illimitatamente (tende a $+\infty$) o decresce illimitatamente (tende a $-\infty$) quando $x$ si avvicina a $x_0$.

- [**Limite finito per**](Limite%20finito%20che%20tende%20a%20infinito.md) $x \to \infty$: si ha quando la funzione si avvicina a un valore finito $l$ quando $x$ cresce illimitatamente ($x \to +\infty$) o decresce illimitatamente ($x \to -\infty$).

- **Limite infinito per** $x \to \infty$: si ha quando la funzione cresce o decresce illimitatamente quando $x$ tende a $+\infty$ o $-\infty$.

- **Limite destro e sinistro per** $x \to x_0$: si ha quando si considera l'avvicinamento a $x_0$ solo da destra ($x \to x_0^+$) o solo da sinistra ($x \to x_0^-$).

Per l'**esistenza del limite**, è necessario che il limite destro e il limite sinistro esistano e siano uguali.

Il **teorema di unicità del limite** afferma che se il limite di una funzione esiste, allora è unico.

L'**operazione di limite** è strettamente legata ai concetti di **asintoti** e di **continuità**.

- Un **asintoto** è una retta a cui il grafico della funzione si avvicina indefinitamente. Esistono **asintoti verticali**, **orizzontali** e **obliqui**.

- Una funzione è **continua** in un punto $x_0$ se il limite per $x$ che tende a $x_0$ coincide con il valore della funzione in $x_0$.

Il **calcolo dei limiti** può essere semplificato applicando le regole delle **operazioni con i limiti**, che permettono di calcolare il limite di somme, differenze, prodotti, quozienti, potenze e inverse di funzioni.

In alcuni casi, il calcolo del limite può portare a **forme indeterminate**, come $\infty - \infty$, $0 \cdot \infty$, $\frac{\infty}{\infty}$ o $\frac{0}{0}$. Per risolvere queste forme indeterminate, si possono utilizzare diverse tecniche, come la messa in evidenza del termine di grado maggiore, la scomposizione e semplificazione di numeratore e denominatore, o il **teorema di de l'Hôpital**.

Infine, il concetto di **limite** è fondamentale per la definizione di **infiniti** e **infinitesimi** e per il loro confronto, che permette di stabilire l'**ordine di un infinitesimo** o di un **infinito** rispetto a un infinitesimo o a un infinito campione.
