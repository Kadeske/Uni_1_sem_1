### Da ricordare
Non è da dimostrare all'orale, ma va conosciuto.
All'orale chiederà il nome. Es. "Perchè il risultato di questo limite è positivo?" --> "Per via del teorema della permanenza del segno bla bla bla".

**Significato Intuitivo:**

Il teorema della permanenza del segno stabilisce una connessione tra il segno del limite di una funzione in un punto e il segno della funzione stessa in un intorno di quel punto. Se il limite è positivo, la funzione deve essere positiva in un intorno del punto, e viceversa.


## Il Teorema della Permanenza del Segno

Il teorema della permanenza del segno afferma che se il limite di una funzione $f(x)$, per $x$ che tende a $x_0$, è positivo (o negativo), allora esiste un intorno di $x_0$ in cui la funzione assume lo stesso segno del limite, escluso al più il punto $x_0$ stesso.

**Formalmente:**

Sia $f: A \to \mathbb{R}$ ed $x_0$ un punto di accumulazione per $A$. Se esiste $$\lim_{x \to x_0} f(x) = l > 0$$, allora esiste un intorno $I(x_0)$ in cui $f(x) > 0$, per ogni $x \in I(x_0)\setminus \{x_0\}$.

**Corollario:** 
(corollario = "Verità conseguente da un'altra precedentemente dimostrata.")

Se esiste un intorno $I(x_0)$ in cui $f(x) > 0$, per ogni $x \in I(x_0)\setminus \{x_0\}$ e se esiste $$\lim_{x \to x_0} f(x) = l$$, allora $l \geq 0$.

**Esempio:**

Consideriamo la funzione $f(x) = x^2$. Il limite di $f(x)$ per $x$ che tende a 0 è 0. Tuttavia, la funzione è positiva per ogni $x$ diverso da 0.

* In questo caso, il limite è 0, che non è positivo. Quindi, il teorema non garantisce che la funzione sia positiva in un intorno di 0. Infatti, la funzione è positiva in un intorno di 0, ma questo non è dovuto al teorema della permanenza del segno.

Consideriamo ora la funzione $g(x) = x^2 + 1$. Il limite di $g(x)$ per $x$ che tende a 0 è 1, che è positivo.

* Il teorema della permanenza del segno garantisce che $g(x)$ sia positiva in un intorno di 0. Infatti, $g(x)$ è sempre positiva, quindi è positiva anche in un intorno di 0.

**Funzioni Positive/Negative:** (Promemoria)

* Una funzione si dice **positiva** in un intervallo se assume valori positivi per tutti i punti dell'intervallo.
* Una funzione si dice **negativa** in un intervallo se assume valori negativi per tutti i punti dell'intervallo.

Il teorema della permanenza del segno può essere applicato sia a funzioni positive che a funzioni negative. Se il limite è negativo, la funzione sarà negativa in un intorno del punto.
