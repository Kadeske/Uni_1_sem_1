I limiti destro e sinistro sono strumenti matematici per analizzare il comportamento di una funzione in prossimità di un punto, quando ci si avvicina a questo punto specificamente da destra o da sinistra.

---

### **Limite Destro:**

* **Definizione:** Sia $f: A \to \mathbb{R}$ e sia $x_0$ un punto di accumulazione per $A$. Si dice che il limite destro di $f(x)$ per $x$ che tende a $x_0$ è uguale a $l$, e si scrive:

  $$
  \lim_{x \to x_0^+} f(x) = l
  $$

  se per ogni $\epsilon > 0$, esiste un $\delta > 0$ tale che:
  $$
  0 < (x - x_0) < \delta \implies |f(x) - l| < \epsilon.
  $$

* **Spiegazione:** Questa definizione indica che per ogni valore di $\epsilon$ (piccolo a piacere) esiste un valore di $\delta$ tale che, se la differenza tra $x$ e $x_0$ è positiva e minore di $\delta$, allora la differenza tra $f(x)$ e $l$ è minore di $\epsilon$. In sostanza, la funzione si avvicina a $l$ quando $x$ si avvicina a $x_0$ da destra.

---

### **Limite Sinistro:**

* **Definizione:** Sia $f: A \to \mathbb{R}$ e sia $x_0$ un punto di accumulazione per $A$. Si dice che il limite sinistro di $f(x)$ per $x$ che tende a $x_0$ è uguale a $l$, e si scrive:

  $$
  \lim_{x \to x_0^-} f(x) = l
  $$

  se per ogni $\epsilon > 0$, esiste un $\delta > 0$ tale che:
  $$
  -\delta < (x - x_0) < 0 \implies |f(x) - l| < \epsilon.
  $$

* **Spiegazione:** Analogamente al limite destro, questa definizione indica che per ogni $\epsilon$ esiste un $\delta$ tale che, se la differenza tra $x$ e $x_0$ è negativa e maggiore di $-\delta$, allora la differenza tra $f(x)$ e $l$ è minore di $\epsilon$. In questo caso, la funzione si avvicina a $l$ quando $x$ si avvicina a $x_0$ da sinistra.

---

### **Quando Utilizzare i Limiti Destro e Sinistro:**

I limiti destro e sinistro sono particolarmente utili nei seguenti casi:

* **Funzioni definite a tratti:** Quando una funzione ha definizioni diverse a destra e a sinistra di un punto, è necessario utilizzare i limiti destro e sinistro per determinare il comportamento della funzione in quel punto.
* **Discontinuità:** I limiti destro e sinistro permettono di classificare i tipi di discontinuità di una funzione. Ad esempio, se i limiti destro e sinistro esistono ma sono diversi, la funzione presenta una discontinuità di prima specie.
* **Studio del comportamento asintotico:** I limiti destro e sinistro possono essere utilizzati per studiare il comportamento di una funzione in prossimità di punti specifici, aiutando a identificare eventuali asintoti verticali.

---

### **Condizione Necessaria e Sufficiente per l'Esistenza del Limite:**

Affinché il limite di una funzione in un punto $x_0$ esista, è necessario e sufficiente che esistano **sia il limite destro che il limite sinistro in quel punto e che siano uguali**. 

* In altre parole:
  $$
  \lim_{x \to x_0} f(x) = l \iff \lim_{x \to x_0^+} f(x) = l = \lim_{x \to x_0^-} f(x).
  $$

---

### **Esempio di Non Esistenza del Limite:**

Un esempio classico di funzione in cui il limite non esiste in un punto è la funzione segno:

  $$
  y = \operatorname{sgn}(x) = \begin{cases} 
  1 & \text{se } x > 0 \\ 
  0 & \text{se } x = 0 \\ 
  -1 & \text{se } x < 0 
  \end{cases}
  $$

In questo caso:

* Il limite destro per $x \to 0^+$ è 1.
* Il limite sinistro per $x \to 0^-$ è -1.

Poiché i limiti destro e sinistro sono diversi, il limite per $x \to 0$ non esiste.


## Verifica di un Limite Destro e uno Sinistro usando le Definizioni

Per verificare un limite destro e uno sinistro, applichiamo le definizioni formali di limite destro e sinistro e dimostriamo che queste sono soddisfatte.

---

### **Esempio di Verifica**

Consideriamo la funzione $f(x) = 2x - 1$ e verifichiamo i seguenti limiti:

1. $\lim_{x \to 1^+} (2x - 1) = 1$
2. $\lim_{x \to 1^-} (2x - 1) = 1$

---

### **Limite Destro:**

1. **Definizione:** Per il limite destro, dobbiamo dimostrare che:
   $$\forall \epsilon > 0, \exists \delta > 0 \text{ tale che } 0 < (x - 1) < \delta \implies |(2x - 1) - 1| < \epsilon.$$

2. **Manipolazione della Disuguaglianza:** L'obiettivo è riscrivere $|(2x - 1) - 1| < \epsilon$:
   * $|(2x - 1) - 1| = |2x - 2|$
   * $|2x - 2| = 2 |x - 1|$
   * Otteniamo quindi la condizione $2 |x - 1| < \epsilon$.

3. **Scelta di $\delta$:** Per soddisfare la disuguaglianza, possiamo scegliere $\delta = \frac{\epsilon}{2}$.

4. **Verifica:** Se $0 < (x - 1) < \delta = \frac{\epsilon}{2}$, allora:
   * $|x - 1| < \frac{\epsilon}{2}$
   * $2 |x - 1| < \epsilon$
   * $|2x - 2| < \epsilon$
   * $|(2x - 1) - 1| < \epsilon$

   Quindi, la definizione di limite destro è soddisfatta con $\lim_{x \to 1^+} (2x - 1) = 1$.

---

### **Limite Sinistro:**

1. **Definizione:** Per il limite sinistro, dobbiamo dimostrare che:
   $$\forall \epsilon > 0, \exists \delta > 0 \text{ tale che } -\delta < (x - 1) < 0 \implies |(2x - 1) - 1| < \epsilon.$$

2. **Manipolazione della Disuguaglianza:** Come nel caso del limite destro, otteniamo:
   * $|(2x - 1) - 1| = 2 |x - 1|$
   * Quindi, $2 |x - 1| < \epsilon$.

3. **Scelta di $\delta$:** Scegliamo $\delta = \frac{\epsilon}{2}$ anche in questo caso.

4. **Verifica:** Se $-\delta = -\frac{\epsilon}{2} < (x - 1) < 0$, allora:
   * $|x - 1| < \frac{\epsilon}{2}$
   * $2 |x - 1| < \epsilon$
   * $|2x - 2| < \epsilon$
   * $|(2x - 1) - 1| < \epsilon$

   La definizione di limite sinistro è quindi soddisfatta, e abbiamo $\lim_{x \to 1^-} (2x - 1) = 1$.

---

### **Conclusione:**

Poiché abbiamo verificato sia il limite destro che il limite sinistro, e sono entrambi uguali a $1$, possiamo concludere che:
$$\lim_{x \to 1} (2x - 1) = 1.$$

---

### **Note:**

* Questo esempio mostra un caso di limite destro e sinistro uguali, e quindi esistenza del limite in $x = 1$.
* La procedura può variare a seconda della funzione, ma l'obiettivo è sempre quello di rispettare le disuguaglianze delle definizioni formali per i limiti destro e sinistro.         