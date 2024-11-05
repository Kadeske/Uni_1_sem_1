Un asintoto verticale è una retta verticale a cui il grafico di una funzione si avvicina indefinitamente man mano che la variabile indipendente si avvicina a un certo valore finito.

* **Definizione:** Una retta $x = x_0$ è un asintoto verticale per il grafico della funzione $f: \mathbb{R} \to \mathbb{R}$ se:
  $$
  \lim_{x \to x_0} f(x) = \infty \quad \text{oppure} \quad \lim_{x \to x_0} f(x) = -\infty.
  $$
  In altre parole, il valore assoluto di $f(x)$ cresce indefinitamente quando $x$ si avvicina a $x_0$.

* **Significato:**  La funzione $f(x)$ cresce illimitatamente (in valore assoluto) quando $x$ si avvicina a $x_0$, avvicinandosi sempre di più a una retta verticale (asintoto) ma senza mai toccarla.

---

### **Esempio**

La retta $x = 3$ è un asintoto verticale per una funzione $f(x)$ se:
$$
\lim_{x \to 3} f(x) = +\infty \quad \text{oppure} \quad \lim_{x \to 3} f(x) = -\infty.
$$

---

### **Rappresentazione Grafica**

Nel grafico di una funzione, un asintoto verticale si manifesta come una linea verticale a cui la curva della funzione si avvicina sempre di più man mano che $x$ tende a $x_0$, senza mai intersecare questa retta.

![[Asintoto verticale 2.png]]

---

### **Esempio Concreto:**

La funzione $f(x) = \frac{1}{x}$ ha un asintoto verticale in $x=0$ (l'asse delle ordinate). Questo è visibile perché:
$$
\lim_{x \to 0^+} \frac{1}{x} = +\infty \quad \text{e} \quad \lim_{x \to 0^-} \frac{1}{x} = -\infty.
$$
Quando $x$ si avvicina a $0$ da destra, $f(x)$ tende a $+\infty$, mentre avvicinandosi da sinistra, $f(x)$ tende a $-\infty$.

![[Asintoto verticale 1.png]]



---

### **Come Identificare gli Asintoti Verticali**

Per trovare gli asintoti verticali di una funzione, bisogna individuare i punti in cui il denominatore della funzione si annulla, ma il numeratore non si annulla in tali punti. In queste condizioni, la funzione tenderà a infinito o a meno infinito.

* **Passi per Identificare gli Asintoti Verticali:**
  1. Individuare i punti $x = x_0$ per cui il denominatore si annulla.
  2. Verificare che in tali punti il numeratore non sia zero.
  3. Calcolare $\lim_{x \to x_0} f(x)$, $\lim_{x \to x_0^+} f(x)$ e $\lim_{x \to x_0^-} f(x)$ per determinare se la funzione tende a $\pm \infty$ in questi punti.

---

### **Nota**

La definizione di asintoto verticale si applica anche ai limiti laterali, cioè per $x$ che tende a $x_0$ da destra ($x \to x_0^+$) o da sinistra ($x \to x_0^-$). Se almeno uno dei due limiti laterali tende a $\infty$ o a $-\infty$, $x = x_0$ sarà un asintoto verticale.

## ATTENZIONE
L'asintoto TENDE ad una retta.

Non la tocca SOLO nel caso dell'asintoto verticale.
Quindi dire che un asintoto (generale) tende ad una retta 'ma non la tocca' è sbagliato. 


![[Limite destro e sinistro]]
