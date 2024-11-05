## **Limite infinito per $x$ che tende a $x_0$**

Sia $f: A \to \mathbb{R}$ una funzione definita su un sottoinsieme $A \subset \mathbb{R}$ e sia $x_0$ un **punto di accumulazione** per $A$.

Si dice che:  
$$
\lim_{x \to x_0} f(x) = \infty
$$

se, per ogni numero reale positivo $M$, **esiste** un numero reale positivo $\delta_M$ tale che, quando la distanza tra $x$ e $x_0$ è minore di $\delta_M$, il valore assoluto di $f(x)$ è maggiore di $M$. In simboli:
$$
\forall M > 0, \ \exists \delta_M > 0 \text{ tale che } |x - x_0| < \delta_M \implies |f(x)| > M.
$$

In altre parole, **per ogni numero positivo** $M$, esiste una distanza $\delta_M$ dal punto $x_0$ entro la quale i valori di $f(x)$ sono maggiori di $M$ in valore assoluto. Questo significa che **$f(x)$ cresce illimitatamente (in valore assoluto) quando $x$ si avvicina a $x_0$.**

### **Esempio**

Consideriamo il limite
$$
\lim_{x \to 0} \frac{1}{x} = \infty.
$$

In questo caso, quando $x$ si avvicina a $0$ da destra, i valori della funzione $\frac{1}{x}$ diventano sempre più grandi in valore assoluto, tendendo a $+\infty$. Se $x$ si avvicina a $0$ da sinistra, $\frac{1}{x}$ tende invece a $-\infty$.

### **[[Asintoto verticale]]**

Se
$$
\lim_{x \to x_0} f(x) = \infty,
$$
allora la retta $x = x_0$ è detta **asintoto verticale** per il grafico della funzione $f(x)$.

- Nell’esempio precedente, la retta $x = 0$ (asse delle ordinate) rappresenta un **asintoto verticale** per la funzione $\frac{1}{x}$, poiché $f(x) = \frac{1}{x}$ tende a infinito quando $x$ si avvicina a $0$.

### **Nota**

Il limite infinito per $x$ che tende a $x_0$ rappresenta una condizione di crescita illimitata per la funzione $f(x)$: quando $x$ si avvicina a $x_0$, i valori di $f(x)$ aumentano senza alcun limite superiore (o inferiore, se il limite è verso $-\infty$), suggerendo un **comportamento asintotico**.



## Dimostrazione di un Limite Finito per $x$ che Tende a Infinito

Per dimostrare un limite finito per $x$ che tende a infinito usando la definizione, bisogna seguire questi passaggi:

### 1. **Definire la Funzione e il Dominio**
   * Sia $f: A \to \mathbb{R}$ una funzione definita su un dominio illimitato $A$, ad esempio $A = \mathbb{R}$.

### 2. **Stabilire il Limite**
   * Vogliamo dimostrare che $\lim_{x \to \infty} f(x) = l$, con $l \in \mathbb{R}$.

### 3. **Applicare la Definizione**
   * Per definizione, si ha $\lim_{x \to \infty} f(x) = l$ se:
     $$
     \forall \epsilon > 0, \ \exists M > 0 \ \text{tale che} \ |x| > M \implies |f(x) - l| < \epsilon.
     $$
   * In altre parole, vogliamo mostrare che, per ogni $\epsilon > 0$, esiste un $M > 0$ tale che quando $x$ è sufficientemente grande (cioè $|x| > M$), i valori di $f(x)$ si trovano entro una distanza $\epsilon$ da $l$.

### 4. **Trovare $M$ in Funzione di $\epsilon$**
   * Manipoliamo la disuguaglianza $|f(x) - l| < \epsilon$ per ottenere un'espressione in cui compare $|x|$, e cerchiamo un valore $M$ tale che $|x| > M$ soddisfi $|f(x) - l| < \epsilon$.

### 5. **Verificare la Definizione**
   * Sostituiamo $M$ nella disuguaglianza e verifichiamo che l'implicazione $|x| > M \implies |f(x) - l| < \epsilon$ sia valida per ogni $\epsilon > 0$.

---

### **Esempio di Applicazione**

Dimostriamo che:
$$
\lim_{x \to +\infty} \frac{x}{x+1} = 1.
$$

#### 1. **Definire Funzione e Dominio**
   * La funzione è $f(x) = \frac{x}{x+1}$, con dominio $A = \mathbb{R} \setminus \{-1\}$, un dominio illimitato.

#### 2. **Stabilire il Limite**
   * Vogliamo dimostrare che $\lim_{x \to +\infty} \frac{x}{x+1} = 1$.

#### 3. **Applicare la Definizione**
   * La definizione da verificare è:
     $$
     \forall \epsilon > 0, \ \exists M > 0 \ \text{tale che} \ x > M \implies \left|\frac{x}{x+1} - 1\right| < \epsilon.
     $$

#### 4. **Trovare $M$ in Funzione di $\epsilon$**
   * Consideriamo l'espressione:
     $$
     \left|\frac{x}{x+1} - 1\right|.
     $$
   * Semplifichiamola:
     $$
     \left|\frac{x - (x+1)}{x+1}\right| = \left|\frac{-1}{x+1}\right| = \frac{1}{|x+1|}.
     $$
   * Ora vogliamo che:
     $$
     \frac{1}{|x+1|} < \epsilon,
     $$
     ovvero, invertendo la disuguaglianza,
     $$
     |x+1| > \frac{1}{\epsilon}.
     $$
   * Poiché stiamo considerando $x \to +\infty$, possiamo assumere $x + 1 > 0$, quindi:
     $$
     x + 1 > \frac{1}{\epsilon}.
     $$
   * Isolando $x$, otteniamo:
     $$
     x > \frac{1}{\epsilon} - 1.
     $$
   * Dunque, possiamo scegliere $M = \frac{1}{\epsilon} - 1$.

#### 5. **Verifica della Definizione**
   * Se $x > M = \frac{1}{\epsilon} - 1$, allora:
     $$
     x + 1 > \frac{1}{\epsilon},
     $$
     e quindi:
     $$
     \frac{1}{x+1} < \epsilon.
     $$
   * Questo implica:
     $$
     \left|\frac{x}{x+1} - 1\right| = \frac{1}{x+1} < \epsilon,
     $$
     che verifica la definizione di limite. Pertanto, abbiamo dimostrato che:
     $$
     \lim_{x \to +\infty} \frac{x}{x+1} = 1.
     $$

---

### **Nota**

La procedura per dimostrare un limite finito per $x$ che tende a infinito può variare a seconda della funzione, ma i passaggi generali rimangono gli stessi: applicare la definizione di limite e trovare un valore di $M$ tale che la disuguaglianza sia soddisfatta per ogni $\epsilon > 0$.
