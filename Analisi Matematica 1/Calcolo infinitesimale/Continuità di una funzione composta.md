## Continuità di una Funzione Composta

La **continuità di una funzione composta** è un concetto importante nel calcolo infinitesimale che si basa sulla continuità delle singole funzioni componenti. 

- Date due funzioni continue, la loro composizione è anch'essa continua.

**Dimostrazione:**

Siano $f: A \rightarrow B$ e $g: B \rightarrow C$ due funzioni continue. Per dimostrare che la funzione composta $g \circ f$ è continua, dobbiamo dimostrare che il limite di $g(f(x))$ per $x$ che tende a un punto $x_0$ nel dominio di $f$ è uguale a $g(f(x_0))$.

- **Continuità di $f$:** Poiché $f$ è continua in $x_0$, sappiamo che:

$$
\lim_{{x \to x_0}} f(x) = f(x_0)
$$

- **Continuità di $g$:** Poiché $g$ è continua in $f(x_0)$, sappiamo che:

$$
\lim_{{y \to f(x_0)}} g(y) = g(f(x_0))
$$

- **Limite della funzione composta:** Utilizzando il teorema del limite di una funzione composta, possiamo scrivere:

$$
\lim_{{x \to x_0}} g(f(x)) = \lim_{{y \to f(x_0)}} g(y)
$$

- **Conclusione:** Combinando le equazioni precedenti, otteniamo:

$$
\lim_{{x \to x_0}} g(f(x)) = g(f(x_0))
$$

Questa equazione dimostra che **la funzione composta $g \circ f$ è continua in $x_0$**. Poiché $x_0$ è un punto arbitrario nel dominio di $f$, possiamo concludere che **la funzione composta $g \circ f$ è continua in tutto il suo dominio**.

**Esempio dalla nostra conversazione:**

Nell'esempio precedente, abbiamo considerato le funzioni $f(x) = x - 2$ e $g(y) = \frac{1}{y}$. Entrambe queste funzioni sono continue nei loro rispettivi domini. La funzione composta $g(f(x)) = \frac{1}{x - 2}$ è anch'essa continua nel suo dominio, che è $\mathbb{R} \setminus \{2\}$ (tutti i numeri reali tranne $2$, dove la funzione non è definita).

**Punti importanti da ricordare:**

- La continuità di una funzione composta dipende dalla continuità delle singole funzioni che la compongono.
- Se una delle funzioni componenti non è continua in un punto, la funzione composta potrebbe non essere continua in quel punto.
- Il dominio della funzione composta è determinato dal dominio della funzione interna e dalle restrizioni imposte dalla funzione esterna.
