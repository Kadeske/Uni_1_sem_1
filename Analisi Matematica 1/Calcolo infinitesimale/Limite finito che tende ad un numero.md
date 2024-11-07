### Da ricordare
**Significato intuitivo:** Quando $x$ si avvicina a $x_0$, il valore di $f(x)$ si avvicina a $l$.

**Asintoto:** Non genera un asintoto.

Importante per il  **[[Teorema di unicità]]**

# Definizione di Limite Finito per $x$ che Tende a $x_0$

#### Definizione in notazione matematica
$$
\text{Se } \forall \, \varepsilon > 0, \; \exists \; \delta_\varepsilon > 0 \; | \; |x - x_0| < \delta_\varepsilon \Rightarrow |f(x) - l| < \varepsilon.
$$



Data una funzione $f: A \rightarrow \mathbb{R}$ e $x_0$ un **punto di accumulazione** per $A$, il **limite finito** di $f(x)$ per $x$ che tende a $x_0$ è un **numero reale** $l$ se, per ogni **intorno** $I_\varepsilon(l)$ di $l$, esiste un **intorno** $I_\delta(x_0)$ di $x_0$ tale che, per ogni $x$ appartenente a $I_\delta(x_0)$ diverso da $x_0$, l'immagine $f(x)$ appartiene a $I_\varepsilon(l)$.

In modo più formale:

Sia $f: A \rightarrow \mathbb{R}$ e $x_0$ un punto di accumulazione per $A$. Sia $l \in \mathbb{R}$. Si dice che il **limite di $f(x)$ per $x$ che tende a $x_0$ è uguale a $l$**, e si scrive:
$$
\lim_{{x \to x_0}} f(x) = l
$$
se e solo se: **per ogni** $\varepsilon > 0$, **esiste un** $\delta > 0$ **tale che per ogni** $x$ **appartenente ad** $A$, **con** $0 < |x - x_0| < \delta$, **si ha** $|f(x) - l| < \varepsilon$.

## Spiegazione

Questa definizione afferma che, per quanto piccolo sia l'intorno $I_\varepsilon(l)$ attorno al valore limite $l$, è sempre possibile trovare un intorno $I_\delta(x_0)$ attorno al punto $x_0$ tale che, **per tutti i valori di** $x$ **in** $I_\delta(x_0)$ **diversi da** $x_0$, **le immagini** $f(x)$ **cadano all'interno di** $I_\varepsilon(l)$.

In altre parole, i valori di $f(x)$ **si avvicinano arbitrariamente a** $l$ **man mano che** $x$ **si avvicina a** $x_0$, senza necessariamente raggiungere $x_0$.

## Punti chiave da ricordare

- **Punto di accumulazione**: $x_0$ deve essere un punto di accumulazione per il dominio $A$, il che significa che ogni intorno di $x_0$ deve contenere almeno un punto di $A$ diverso da $x_0$.
- **Intorni**: Gli intorni $I_\varepsilon(l)$ e $I_\delta(x_0)$ sono **intervalli aperti** centrati rispettivamente su $l$ e $x_0$.
- **Epsilon e delta**: $\varepsilon$ e $\delta$ sono **numeri reali positivi arbitrariamente piccoli**. La scelta di $\delta$ dipende da $\varepsilon$.

**Nota**: La definizione di **limite finito** si applica anche ai casi in cui $x$ tende a $+\infty$ o $-\infty$. In questi casi, gli intorni $I_\delta(x_0)$ sono sostituiti da **intervalli illimitati**.


## Verifica e Dimostrazione di un Limite Finito

### Definizione di Limite Finito

Data una funzione $f: A \rightarrow \mathbb{R}$ e $x_0$ un punto di accumulazione per $A$, il **limite finito di $f(x)$ per $x$ che tende a $x_0$ è $l$** se, per ogni $\varepsilon > 0$, esiste un $\delta > 0$ tale che per ogni $x$ appartenente ad $A$ con $0 < |x - x_0| < \delta$, si ha $|f(x) - l| < \varepsilon$.

### Verifica di un Limite Finito: Esempio

Consideriamo la funzione $f(x) = -x + 3$ e il punto $x_0 = 2$. Vogliamo verificare che:
$$
\lim_{{x \to 2}} (-x + 3) = 1
$$

**Dimostrazione:**

1. **Fissiamo $\varepsilon > 0$.**
2. **Dobbiamo trovare un $\delta > 0$ tale che, se $0 < |x - 2| < \delta$, allora $|(-x + 3) - 1| < \varepsilon$.**
3. **Semplifichiamo la disuguaglianza $|(-x + 3) - 1| < \varepsilon$:**
   
   $$
   |(-x + 3) - 1| < \varepsilon
   $$
   $$
   |-x + 2| < \varepsilon
   $$
   $$
   |x - 2| < \varepsilon
   $$

4. **Possiamo quindi scegliere $\delta = \varepsilon$.**

5. **Conclusione:** Per ogni $\varepsilon > 0$, abbiamo trovato un $\delta > 0$ (in questo caso $\delta = \varepsilon$) tale che, se $0 < |x - 2| < \delta$, allora $|(-x + 3) - 1| < \varepsilon$. **Pertanto, il limite è verificato.**

### Spiegazione dei Passaggi

- **Passo 1:** Si fissa un valore arbitrario di $\varepsilon$, che rappresenta la distanza massima accettabile tra $f(x)$ e il valore limite $l$.
- **Passo 2:** Si cerca un valore di $\delta$, che rappresenta la distanza massima accettabile tra $x$ e $x_0$, in modo che la condizione del limite sia soddisfatta.
- **Passo 3:** Si semplifica la disuguaglianza che esprime la condizione del limite, in modo da ottenere un'espressione più semplice per $|x - x_0|$.
- **Passo 4:** Si sceglie un valore di $\delta$ che soddisfi la disuguaglianza semplificata. In questo caso, si è scelto $\delta = \varepsilon$, ma in generale la scelta di $\delta$ può dipendere da $\varepsilon$ e dalla funzione $f(x)$.
- **Passo 5:** Si conclude che la definizione di limite è soddisfatta, poiché per ogni $\varepsilon > 0$ è stato possibile trovare un $\delta > 0$ che soddisfa la condizione del limite.

### Note

- La scelta di $\delta = \varepsilon$ in questo esempio è possibile perché la funzione $f(x) = -x + 3$ è lineare. Per funzioni più complesse, la scelta di $\delta$ potrebbe essere più elaborata.
