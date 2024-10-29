## Definizione di Limite Infinito per $x$ che Tende a $x_0$

#### Definizione in notazione matematica
$$
\text{Se } \forall M > 0, \; \exists \; \delta_M > 0 \; | \; |x - 3| < \delta_M \Rightarrow |f(x)| > M.
$$



Sia $f: A \rightarrow \mathbb{R}$ e $x_0$ un **punto di accumulazione** per $A$. Si dice che il **limite di $f(x)$ per $x$ che tende a $x_0$ è infinito**, e si scrive:
$$
\lim_{{x \to x_0}} f(x) = +\infty
$$
se per **ogni numero reale positivo** $M$, esiste un $\delta_M > 0$ tale che **per ogni** $x$ **appartenente ad** $A$, **con** $0 < |x - x_0| < \delta_M$, **si ha** $|f(x)| > M$.

### Spiegazione

Questa definizione afferma che, **per quanto grande sia il numero positivo** $M$, è sempre possibile trovare un **intorno** $I_{\delta_M}(x_0)$ attorno al punto $x_0$ tale che, **per tutti i valori di** $x$ **in** $I_{\delta_M}(x_0)$ **diversi da** $x_0$, **il valore assoluto della funzione** $|f(x)|$ **sia maggiore di** $M$. In altre parole, i valori di $f(x)$ **crescono arbitrariamente in modulo** man mano che $x$ si avvicina a $x_0$.

### Distinzione tra $+\infty$ e $-\infty$

Il **limite infinito** può essere specificato come $+\infty$ o $-\infty$:

- **$\lim_{{x \to x_0}} f(x) = +\infty$**: se per ogni $M > 0$, esiste un $\delta_M > 0$ tale che per ogni $x$ appartenente ad $A$, con $0 < |x - x_0| < \delta_M$, si ha $f(x) > M$.
- **$\lim_{{x \to x_0}} f(x) = -\infty$**: se per ogni $M > 0$, esiste un $\delta_M > 0$ tale che per ogni $x$ appartenente ad $A$, con $0 < |x - x_0| < \delta_M$, si ha $f(x) < -M$.

### Esempio

Consideriamo la funzione $f(x) = \frac{1}{x}$ e il punto $x_0 = 0$. Intuitivamente, possiamo vedere che quando $x$ si avvicina a $0$, il valore di $\frac{1}{x}$ **diventa sempre più grande in modulo**. Possiamo quindi affermare che:
$$
\lim_{{x \to 0}} \frac{1}{x} = +\infty
$$

### Asintoti Verticali

Un **limite infinito** per $x$ che tende a un numero $x_0$ indica la presenza di un **asintoto verticale** nel grafico della funzione in corrispondenza di $x = x_0$.

### Note

- Le sources descrivono i **limiti infiniti** e gli **asintoti verticali**, ma non forniscono una definizione formale di limite infinito che tende a un numero.
- La definizione fornita qui si basa sulle informazioni presenti nelle sources e sulla nostra conversazione precedente.
- La spiegazione e l'esempio sono stati elaborati per chiarire ulteriormente il concetto di **limite infinito**.




## Dimostrazione di un Limite Infinito per $x$ che Tende a $x_0$

### Definizione di Limite Infinito

Data una funzione $f: A \rightarrow \mathbb{R}$ e $x_0$ un **punto di accumulazione** per $A$, si dice che il **limite di $f(x)$ per $x$ che tende a $x_0$ è infinito**, e si scrive:
$$
\lim_{{x \to x_0}} f(x) = +\infty
$$
se per ogni numero reale positivo $M$, esiste un $\delta_M > 0$ tale che per ogni $x$ appartenente ad $A$, con $0 < |x - x_0| < \delta_M$, si ha $|f(x)| > M$.

### Dimostrazione Passo-Passo: Esempio

Consideriamo la funzione $f(x) = \frac{1}{x^2}$ e il punto $x_0 = 0$. Vogliamo dimostrare che:
$$
\lim_{{x \to 0}} \frac{1}{x^2} = +\infty
$$

**Dimostrazione:**

1. **Fissiamo un numero reale positivo** $M$. 
2. **Dobbiamo trovare un** $\delta_M > 0$ tale che, se $0 < |x - 0| < \delta_M$, allora $|\frac{1}{x^2}| > M$.
3. **Semplifichiamo la disuguaglianza** $|\frac{1}{x^2}| > M$:

   $$
   |\frac{1}{x^2}| > M \\
   \frac{1}{x^2} > M \\
   x^2 < \frac{1}{M} \\
   |x| < \frac{1}{\sqrt{M}}
   $$

4. **Possiamo quindi scegliere** $\delta_M = \frac{1}{\sqrt{M}}$.

5. **Conclusione:** Per ogni $M > 0$, abbiamo trovato un $\delta_M > 0$ (in questo caso $\delta_M = \frac{1}{\sqrt{M}}$) tale che, se $0 < |x - 0| < \delta_M$, allora $|\frac{1}{x^2}| > M$. **Pertanto, il limite è verificato.**

### Spiegazione dei Passaggi

* **Passo 1:** Si fissa un valore arbitrario di $M$, che rappresenta un limite inferiore per il valore assoluto di $f(x)$.
* **Passo 2:** Si cerca un valore di $\delta_M$, che limita la distanza tra $x$ e $x_0$, in modo che la condizione del limite sia soddisfatta.
* **Passo 3:** Si semplifica la disuguaglianza che esprime la condizione del limite per ottenere un'espressione più semplice per $|x - x_0|$.
* **Passo 4:** Si sceglie un valore di $\delta_M$ che soddisfi la disuguaglianza semplificata. 
* **Passo 5:** Si conclude che la definizione di **limite infinito** è soddisfatta, in quanto per ogni $M > 0$ è possibile trovare un $\delta_M > 0$ che garantisce $|f(x)| > M$ quando $0 < |x - x_0| < \delta_M$.

### Note

* L'esempio della funzione $\frac{1}{x^2}$ e la dimostrazione passo-passo sono stati elaborati per fornire una spiegazione più dettagliata del concetto di **limite infinito**. Le sources forniscono informazioni sui limiti infiniti, ma non includono dimostrazioni specifiche come quella presentata. 
* La scelta di $\delta_M = \frac{1}{\sqrt{M}}$ in questo esempio è legata alla specifica funzione $f(x) = \frac{1}{x^2}$. Per altre funzioni, la scelta di $\delta_M$ potrebbe essere diversa.
* Il concetto di **asintoto verticale**, menzionato nelle sources, è strettamente correlato ai limiti infiniti. Quando un limite infinito per $x$ che tende a $x_0$ è verificato, questo implica la presenza di un **asintoto verticale** in $x = x_0$ nel grafico della funzione.


