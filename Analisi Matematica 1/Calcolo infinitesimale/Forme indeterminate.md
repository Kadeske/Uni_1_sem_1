## Forme Indeterminate e Loro Risoluzioni

Le **forme indeterminate** sono espressioni matematiche che si ottengono quando si cerca di calcolare il limite di una funzione e il risultato non può essere determinato direttamente applicando le regole algebriche standard.

**Le forme indeterminate più comuni sono:**

- $\infty - \infty$
- $0 \cdot \infty$
- $\frac{\infty}{\infty}$
- $\frac{0}{0}$
- $0^0$
- $1^{\infty}$
- $\infty^0$

**Risoluzione delle Forme Indeterminate:**

La risoluzione delle forme indeterminate richiede l'utilizzo di tecniche specifiche, come:

- **Manipolazione algebrica:** Semplificazione dell'espressione, fattorizzazione, razionalizzazione, ecc.
- **Teorema di de l'Hôpital:** Applicabile a forme indeterminate del tipo $\frac{0}{0}$ o $\frac{\infty}{\infty}$, consente di calcolare il limite derivando numeratore e denominatore.
- **Sviluppi di Taylor:** Utili per approssimare funzioni in un intorno di un punto.
- **Confronto tra infinitesimi e infiniti:** Determinare l'ordine di infinitesimo o di infinito di una funzione rispetto ad un’altra.

## **Perché si Prende il Termine di Grado Maggiore?**

Quando si ha a che fare con limiti che tendono a infinito, spesso si cerca di semplificare l'espressione mettendo in evidenza il termine di grado maggiore. Questo perché, per valori di $x$ molto grandi, **il termine di grado maggiore domina il comportamento della funzione**.

Ad esempio, consideriamo il limite:

$$
\lim_{{x \to \infty}} \frac{2x^3 - 5x^2 + 3x - 1}{x^3 + 2x^2 - 7}
$$

Mettendo in evidenza il termine di grado maggiore ($x^3$) sia al numeratore che al denominatore, otteniamo:

$$
\lim_{{x \to \infty}} \frac{x^3 \left( 2 - \frac{5}{x} + \frac{3}{x^2} - \frac{1}{x^3} \right)}{x^3 \left( 1 + \frac{2}{x} - \frac{7}{x^3} \right)}
$$

Quando $x$ tende a infinito, i termini $\frac{5}{x}$, $\frac{3}{x^2}$, $\frac{1}{x^3}$, $\frac{2}{x}$ e $\frac{7}{x^3}$ tendono tutti a $0$. Quindi, il limite si semplifica a:

$$
\lim_{{x \to \infty}} \frac{2x^3}{x^3} = 2
$$

**In questo caso, il termine di grado maggiore ($x^3$) ha determinato il valore del limite.**

### Spiegazione approfondita (richiesta all'orale)
## Il Termine di Grado Maggiore nei Limiti

Quando si calcola il limite di una funzione per $x$ che tende all'infinito, **il termine di grado maggiore** è quello che influenza in modo determinante il risultato finale. Per capire questo concetto, è utile analizzare il comportamento delle funzioni razionali, cioè funzioni espresse come rapporto tra due polinomi.

Consideriamo un esempio generale di una funzione razionale:

$$
f(x) = \frac{a_n x^n + a_{n-1} x^{n-1} + \dots + a_1 x + a_0}{b_m x^m + b_{m-1} x^{m-1} + \dots + b_1 x + b_0}
$$

dove $a_n$, $a_{n-1}$, $\dots$, $a_0$ e $b_m$, $b_{m-1}$, $\dots$, $b_0$ sono coefficienti reali e $n$ e $m$ sono i gradi dei polinomi al numeratore e al denominatore, rispettivamente.

Quando $x$ tende all'infinito, i termini con esponente minore diventano progressivamente insignificanti rispetto al termine di grado maggiore. Questo perché la crescita del termine di grado maggiore è molto più rapida rispetto a quella dei termini di grado inferiore.

Per visualizzare questo concetto, possiamo riscrivere la funzione razionale mettendo in evidenza il termine di grado maggiore sia al numeratore che al denominatore:

$$
f(x) = \frac{x^n \left( a_n + \frac{a_{n-1}}{x} + \dots + \frac{a_1}{x^{n-1}} + \frac{a_0}{x^n} \right)}{x^m \left( b_m + \frac{b_{m-1}}{x} + \dots + \frac{b_1}{x^{m-1}} + \frac{b_0}{x^m} \right)}
$$

Quando $x$ tende all'infinito, tutti i termini del tipo $\frac{a_i}{x^k}$ e $\frac{b_j}{x^l}$, dove $k$ e $l$ sono interi positivi, tendono a zero.

Di conseguenza, il limite della funzione razionale dipende esclusivamente dal rapporto tra i coefficienti dei termini di grado maggiore:

- Se $n > m$, il limite di $f(x)$ per $x$ che tende all'infinito sarà infinito (positivo o negativo a seconda del segno di $\frac{a_n}{b_m}$).
- Se $n < m$, il limite di $f(x)$ per $x$ che tende all'infinito sarà zero.
- Se $n = m$, il limite di $f(x)$ per $x$ che tende all'infinito sarà uguale a $\frac{a_n}{b_m}$.

**Esempio:**

Consideriamo il limite:

$$
\lim_{{x \to \infty}} \frac{3x^2 + 2x - 1}{x^2 - 5x + 2}
$$

Mettendo in evidenza il termine di grado maggiore ($x^2$), otteniamo:

$$
\lim_{{x \to \infty}} \frac{x^2 \left(3 + \frac{2}{x} - \frac{1}{x^2}\right)}{x^2 \left(1 - \frac{5}{x} + \frac{2}{x^2}\right)}
$$

Quando $x$ tende all'infinito, i termini $\frac{2}{x}$, $\frac{1}{x^2}$, $\frac{5}{x}$ e $\frac{2}{x^2}$ tendono a zero. Quindi il limite si semplifica a:

$$
\lim_{{x \to \infty}} \frac{3x^2}{x^2} = 3
$$

**In questo caso, il termine di grado maggiore ($x^2$) ha determinato il valore del limite (3).**

**In conclusione:**

Quando si calcola il limite di una funzione per $x$ che tende all'infinito, **il termine di grado maggiore è quello che influenza in modo determinante il risultato finale**. Questo è dovuto al fatto che la crescita del termine di grado maggiore è molto più rapida rispetto a quella dei termini di grado inferiore, rendendo questi ultimi insignificanti per valori di $x$ molto grandi.



