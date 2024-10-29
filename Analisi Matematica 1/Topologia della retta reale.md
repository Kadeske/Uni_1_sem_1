### Due metodi di rappresentazione degli insiemi

1. **Per elencazione**: vengono elencati gli elementi dell'insieme.
    - **Esempio**: $A = {1, 2, 3, 4}$.
2. **Per intervalli**: si usa una notazione che descrive l'intervallo in cui gli elementi appartengono.
    - **Esempio**: $B = [1, 4]$ indica che l'insieme contiene tutti i numeri reali tra 1 e 4, estremi inclusi.

---

### Definizione di intervallo

Un **intervallo** è un sottoinsieme della retta reale $R$, costituito da tutti i punti compresi tra due estremi $a$ e $b$.  
In notazione matematica:

$$I={x∈R∣a<x<b}⊂RI = \{x \in \mathbb{R} \mid a < x < b\} \subset \mathbb{R} I={x∈R∣a<x<b}⊂R$$

- **Intervallo chiuso**: quando entrambi gli estremi sono inclusi. Si rappresenta con parentesi quadre, $[a, b]$.
    - **Esempio**: $[1, 3]$ include 1 e 3.
- **Intervallo aperto**: quando nessuno degli estremi è incluso. Si rappresenta con parentesi tonde, $(a, b)$.
    - **Esempio**: $(1, 3)$ non include né 1 né 3.

---

### Intervalli limitati e illimitati

- **Intervallo limitato**: se entrambi gli estremi sono numeri reali finiti.
    
    - **Esempio**: $[1, 3]$ è limitato.
- **Intervallo illimitato**: se uno degli estremi è $\pm \infty$.
    
    - **Esempio**: $(-\infty, 5]$ è un intervallo illimitato a sinistra.

---

### Definizione di intorno

Un **intorno** di un punto $x_0$ è un intervallo aperto che contiene $x_0$, estendendosi sia a sinistra che a destra di esso.  
Si rappresenta come:
$$I(x0)={x∈R∣x0−r1<x<x0+r2}$$

dove $r_1$ e $r_2$ sono numeri reali positivi che determinano l'estensione dell'intorno.

---

### Intervallo circolare

Un **intorno circolare** è un intorno dove $r_1 = r_2$, quindi l'intervallo si estende della stessa quantità a sinistra e a destra del punto centrale $x_0$:

$$Ir(x0)={x∈R∣x0−r<x<x0+r}$$

In notazione con il **valore assoluto**:

$$Ir(x0)={x∈R∣∣x−x0∣<r}$$

---

### Intorni sinistro e destro

- **Intorno sinistro**: un intervallo che si estende solo a sinistra di un punto $x_0$:

$$I(x0)={x∈R∣x0−r<x<x0}=(x0−r,x0)$$

- **Intorno destro**: un intervallo che si estende solo a destra di un punto $x_0$:

$$I(x0)={x∈R∣x0<x<x0+r}=(x0,x0+r)$$

---

### Punti interni

Un punto $x_0$ è detto **punto interno** di un insieme $A \subseteq \mathbb{R}$ se esiste un intorno di $x_0$ contenuto interamente in $A$.  
In simboli:

$$∃Ir(x0)⊂Aconx0∈A$$

- **Esempio**: Se $A = (1, 3)$, il punto $x_0 = 2$ è interno a $A$ perché esiste un intorno di $x_0$ (ad esempio $(1.5, 2.5)$) che è completamente contenuto in $A$.

---

### Punti esterni

Un punto $x_0$ è detto **punto esterno** di un insieme $A \subseteq \mathbb{R}$ se esiste un intorno di $x_0$ che non contiene alcun punto di $A$.  
In simboli:

$$∃Ir(x0)⊂Acconx0∉A$$

- **Esempio**: Se $A = (1, 2)$, il punto $x_0 = 3$ è esterno ad $A$ perché esiste un intorno di $x_0$ (ad esempio $(2.5, 3.5)$) che non interseca $A$.

---

### Punti di frontiera o bordo

Un punto di frontiera di un insieme A è un punto che **non è né interno né esterno all'insieme**

Un **punto** è considerato **interno** ad un insieme A se esiste un intorno circolare del punto interamente contenuto in A

Un **punto** è considerato **esterno** ad un insieme A se esiste un intorno circolare del punto interamente contenuto nel complementare di A.1

In altre parole, un punto di frontiera "**tocca**" *sia l'insieme A che il suo complementare*. Ogni intorno di un punto di frontiera conterrà sempre punti sia dell'insieme A sia del suo complementare.

##### Esempio
Consideriamo l'intervallo A = {x ∈ R | 1 < x < 2}
- Il punto x₀ = 2 è un punto di frontiera per A.
	- x₀ non appartiene ad A.
	- Qualsiasi intorno di x₀, per quanto piccolo, conterrà punti sia di A (ad esempio 1.999) sia del complementare di A (ad esempio 2.001).

Punti di Frontiera e Insiemi Chiusi

Un insieme è chiuso se contiene tutti i suoi punti di frontiera.3 Negli intervalli chiusi, tutti i punti sono di accumulazione, compresi gli estremi.

Punti di Accumulazione
Un punto di accumulazione per un insieme A è un punto tale che ogni suo intorno contiene almeno un punto di A diverso dal punto stesso. Un punto di frontiera può essere, ma non necessariamente, un punto di accumulazione.


### Punti di accumulazione

Un punto $x_0$ è detto **punto di accumulazione** di un insieme $A$ se in ogni intorno di $x_0$ esiste almeno un punto di $A$ diverso da $x_0$.  
In simboli:

$$∀Ir(x0), ∃x∈Aconx≠x0\forall I_r(x_0), \ \exists x \in A \quad \text{con} \quad x \neq x_0 ∀Ir​(x0​), ∃x∈Aconx=x0​$$

- **Esempio**: Se $A = \left( 1, 3 \right)$, il punto $x_0 = 2$ è un punto di accumulazione perché ogni intorno di $x_0$ contiene altri punti di $A$.

---

### Insiemi aperti e chiusi

- **Insieme aperto**: Un insieme è aperto se **tutti i suoi punti sono interni**.
    
    - **Esempio**: $A = (1, 3)$ è aperto perché ogni punto ha un intorno contenuto in $A$.
- **Insieme chiuso**: Un insieme è chiuso se **contiene tutti i suoi punti di frontiera**.
    
    - **Esempio**: $A = [1, 3]$ è chiuso perché contiene i suoi punti di frontiera $1$ e $3$.

---

### Esempi grafici

1. **Punti interni**: ![Punti interni](https://upload.wikimedia.org/wikipedia/commons/thumb/3/3d/Interior_point_example.svg/200px-Interior_point_example.svg.png)
    
    - Il punto rosso è interno all'intervallo aperto.
2. **Punti di frontiera**: ![Frontiera](https://upload.wikimedia.org/wikipedia/commons/thumb/7/71/Boundary_point.svg/200px-Boundary_point.svg.png)
    
    - Il punto sulla linea è di frontiera.