## Il Teorema di Unicità del Limite

Il teorema di unicità del limite afferma che se il limite di una funzione $f(x)$ esiste per $x$ che tende ad un punto di accumulazione $x_0$, allora tale limite è unico.

**Formalmente:**

Sia $f: A \to \mathbb{R}$ ed $x_0$ un punto di accumulazione per $A$. Se esiste $$\lim_{x \to x_0} f(x)=l$$allora è unico.

**Esempio:**

Si consideri la funzione $f(x) = x^2$. Il limite di $f(x)$ per $x$ che tende a 2 è 4. Questo limite è unico. Non è possibile trovare un altro valore al quale $f(x)$ si avvicina man mano che $x$ si avvicina a 2.

**Significato Intuitivo:**

Il teorema di unicità del limite garantisce che se una funzione converge ad un valore specifico in un punto, non può convergere anche ad un altro valore nello stesso punto. Questo è fondamentale per la coerenza del concetto di limite e per la sua applicabilità in vari ambiti della matematica.


## Non Unicità del Limite Quando Non Esiste

Se il limite di una funzione non esiste, non ha senso parlare di unicità. La definizione di unicità del limite, come affermata dal teorema di unicità, presuppone l'esistenza del limite. Il teorema afferma che *se* esiste il limite, allora è unico. Non dice nulla sull'unicità o meno quando il limite non esiste.

Quando il limite non esiste, significa che la funzione non si avvicina ad un singolo valore definito quando $x$ si avvicina al punto di accumulazione. Potrebbero esserci diversi comportamenti della funzione che portano alla non esistenza del limite, come:

* **Limiti destro e sinistro diversi:** Se i limiti destro e sinistro della funzione in un punto sono diversi, allora il limite in quel punto non esiste.
* **Oscillazioni:** La funzione potrebbe oscillare infinitamente tra diversi valori quando $x$ si avvicina al punto di accumulazione.
* **Divergenza a infinito:** La funzione potrebbe crescere o decrescere senza limiti quando $x$ si avvicina al punto di accumulazione.

### Esempio: $$\lim_{x \to x_0} \cos(x)$$

La funzione $\cos(x)$ oscilla tra -1 e 1 per ogni valore di $x$. Quando $x$ tende a un qualsiasi punto $x_0$, la funzione continua ad oscillare e non si avvicina a un valore specifico. Pertanto, il limite di $\cos(x)$ per $x$ che tende a $x_0$ non esiste.

In questo caso, non ha senso parlare di unicità del limite. Il limite non esiste, quindi non può essere né unico né non unico.
