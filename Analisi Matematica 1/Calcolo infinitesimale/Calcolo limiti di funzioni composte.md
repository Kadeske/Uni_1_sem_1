Ecco una semplice spiegazione del calcolo del limite di una funzione composta:

**Limite di una funzione composta --> g(f(x))**

Il limite di una funzione composta può essere calcolato utilizzando i limiti delle singole funzioni che la compongono. Siano date due funzioni, $f: A \rightarrow B$ e $g: B \rightarrow C$. Se $x_0$ è un punto di accumulazione per $A$ e il limite di $f(x)$ per $x$ che tende a $x_0$ è $l$, ovvero:

$$
\lim_{{x \to x_0}} f(x) = l
$$

e $l$ è un punto di accumulazione per $B$ e il limite di $g(y)$ per $y$ che tende a $l$ è $L$, ovvero:

$$
\lim_{{y \to l}} g(y) = L
$$

allora esiste il limite di $g(f(x))$ per $x$ che tende a $x_0$ ed è uguale a $L$, ovvero:

$$
\lim_{{x \to x_0}} g(f(x)) = L
$$

**In parole più semplici:**

- Se si hanno due funzioni, $f(x)$ e $g(x)$, e si vuole trovare il limite della loro composizione, $g(f(x))$, quando $x$ tende a un certo valore $x_0$.
- Si trova prima il limite di $f(x)$ quando $x$ tende a $x_0$. Supponiamo che questo limite sia $l$.
- Si trova poi il limite di $g(y)$ quando $y$ tende a $l$.
- Il limite di $g(f(x))$ quando $x$ tende a $x_0$ è uguale al limite di $g(y)$ quando $y$ tende a $l$.

**Esempio:**

Consideriamo le funzioni $f(x) = x - 2$ e $g(y) = \frac{1}{y}$. Vogliamo trovare il limite di $g(f(x))$ quando $x$ tende a $2$.

- **Passo 1:** Trovare il limite di $f(x)$ quando $x$ tende a $2$.

$$
\lim_{{x \to 2}} (x - 2) = 0
$$

- **Passo 2:** Trovare il limite di $g(y)$ quando $y$ tende a $0$.

$$
\lim_{{y \to 0}} \frac{1}{y} = \infty
$$

- **Passo 3:** Il limite di $g(f(x))$ quando $x$ tende a $2$ è uguale al limite di $g(y)$ quando $y$ tende a $0$.

$$
\lim_{{x \to 2}} g(f(x)) = \lim_{{x \to 2}} \frac{1}{x - 2} = \infty
$$

**Nota:**

È importante notare che questo metodo funziona solo se i limiti delle singole funzioni esistono e se il limite interno, $l$, è un punto di accumulazione per il dominio della funzione esterna, $g(y)$.
