### Da ricordare
**Significato intuitivo:** Quando $x$ diventa arbitrariamente grande, il valore assoluto di $f(x)$ diventa arbitrariamente grande.

**Asintoto:** Potrebbe generare un asintoto obliquo di equazione $y = mx + q$, se $q$ e $m \neq 0$ esistono e sono finiti. Per determinare l'asintoto obliquo, si calcolano i limiti:

- $$\lim_{x \to \infty} \frac{f(x)}{x} = m$$
- $$\lim_{x \to \infty} [f(x) - mx] = q$$

## Limite infinito che tende a infinito

Un limite infinito che tende a infinito si verifica quando, man mano che il valore della variabile indipendente $x$ cresce indefinitamente, il valore della funzione $f(x)$ tende anche a infinito (positivo o negativo). In altre parole, per quanto grande sia un numero $N$, è possibile trovare un valore di $x$ tale che $f(x)$ sia maggiore di $N$ (o minore di $-N$).

**Formalmente, si dice che:**

$$
\lim_{x \to \infty} f(x) = \infty
$$

**se per ogni $N > 0$, esiste un $M > 0$ tale che per ogni $|x| > M$ si ha $|f(x)| > N$.**

**Significato Intuitivo:**

Un limite infinito che tende a infinito indica che la funzione cresce senza limiti man mano che $x$ cresce. Il grafico della funzione si estende all'infinito lungo l'asse delle $y$ man mano che si sposta a destra o a sinistra lungo l'asse delle $x$.

**Asintoto:**

A differenza di un limite finito che tende a infinito, che genera un asintoto orizzontale, un limite infinito che tende a infinito non genera un asintoto orizzontale. Tuttavia, potrebbe esistere un **asintoto obliquo** se il limite di  $\frac{f(x)}{x}$ per $x$ che tende a infinito esiste ed è un numero finito diverso da zero.

**Esempio:**

La funzione $f(x) = x²$ ha un limite infinito per $x$ che tende a infinito. Infatti, per quanto grande sia un numero $N$, è sempre possibile trovare un valore di $x$ tale che $x²$ sia maggiore di $N$. Il grafico della funzione è una parabola che si estende all'infinito verso l'alto.

**Nota:**

Il concetto di limite infinito che tende a infinito è importante in matematica per descrivere il comportamento di funzioni che crescono senza limiti. Ha applicazioni in diversi ambiti, come lo studio della crescita di popolazioni, la diffusione di epidemie e l'analisi di algoritmi.

## Dimostrazione di un limite infinito che tende a infinito

Per dimostrare che un limite è infinito che tende a infinito, si utilizza la definizione formale. Sia $f(x)$ una funzione e si voglia dimostrare che:

**$$
\lim_{x \to \infty} f(x) = \infty
$$**

**Definizione:** Per ogni $N > 0$, esiste un $M > 0$ tale che per ogni $|x| > M$ si ha $|f(x)| > N$.

**Procedura di Dimostrazione:**

1. **Scegliere un valore arbitrario di $N > 0$.** Questo valore rappresenta un limite inferiore per $|f(x)|$.

2. **Trovare un valore di $M > 0$ tale che, per ogni $|x| > M$, si abbia $|f(x)| > N$.** Questo passaggio richiede di manipolare algebricamente la funzione $f(x)$ per trovare un'espressione che sia maggiore di $N$ quando $|x|$ è maggiore di $M$.

3. **Dimostrare che la disuguaglianza $|f(x)| > N$ è vera per ogni $|x| > M$.** Questo passaggio potrebbe richiedere l'utilizzo di disuguaglianze note o proprietà della funzione $f(x)$.

**Esempio:**

Si dimostri che $$\lim_{x \to \infty} x² = \infty$$.

1. **Sia $N > 0$ un numero arbitrario.**

2. **Si scelga $M = \sqrt{N}$.** Allora, per ogni $|x| > M$, si ha:

   $$|x| > \sqrt{N}$$  
   $$x² > N$$  
   $$|x²| > N$$

3. **Pertanto, per ogni $N > 0$, esiste un $M > 0$ (in questo caso $M = \sqrt{N}$) tale che per ogni $|x| > M$ si ha $|f(x)| > N$.** Questo dimostra che $$\lim_{x \to \infty} x² = \infty$$.

**Conclusione:**

La dimostrazione di un limite infinito che tende a infinito richiede di applicare la definizione formale e di utilizzare tecniche algebriche e proprietà delle funzioni per dimostrare che la disuguaglianza $|f(x)| > N$ è vera per valori di $x$ sufficientemente grandi.
