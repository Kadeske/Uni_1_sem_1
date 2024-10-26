Capito, userò `$` per le formule inlinea e `$$` per i blocchi multilinea. Ecco il testo corretto:

---

### Modus Ponens (Affermando il Consequente)

Il **Modus Ponens** è una regola di inferenza che permette di dedurre la verità di una proposizione a partire da un'implicazione e dall'affermazione dell'antecedente.

**Forma:**

- Se $ p \Rightarrow q $ è vero, e $ p $ è vero, allora $ q $ è vero.

**Schema:**

$$
\begin{align*}
1. & \; p \Rightarrow q \; \text{(Se $ p $ allora $ q $)} \\
2. & \; p \; \text{(Affermo che $ p $ è vero)} \\
3. & \; q \; \text{(Concludo che $ q $ è vero)}
\end{align*}
$$

**Esempio:**

- **Premessa 1**: Se piove, allora le strade sono bagnate. $ p \Rightarrow q $
- **Premessa 2**: Piove. $ p $
- **Conclusione**: Le strade sono bagnate. $ q $

**Errore comune:**

- Sbagliato: Se affermassi $ q $ (strade bagnate) senza sapere se $ p $ è vero (pioggia), non posso concludere che $ p $ sia vero.

---

### Modus Tollens (Negando il Consequente)

Il **Modus Tollens** permette di dedurre la falsità di una proposizione dall'implicazione e dalla negazione del conseguente.

**Forma:**

- Se $ p \Rightarrow q $ è vero e $ q $ è falso, allora $ p $ è falso.

**Schema:**

$$
\begin{align*}
1. & \; p \Rightarrow q \; \text{(Se $ p $ allora $ q $)} \\
2. & \; \neg q \; \text{(Affermo che $ q $ è falso)} \\
3. & \; \neg p \; \text{(Concludo che $ p $ è falso)}
\end{align*}
$$

**Esempio:**

- **Premessa 1**: Se piove, le strade sono bagnate. $ p \Rightarrow q $
- **Premessa 2**: Le strade non sono bagnate. $ \neg q $
- **Conclusione**: Non piove. $ \neg p $

**Errore comune:**

- Sbagliato: Non posso dedurre che $ q $ sia falso solo perché non ho osservato $ p $. Ad esempio, le strade potrebbero essere bagnate per altre cause (ad esempio, un lavaggio).

---

### Riduzione all'assurdo (Contraddizione)

La **riduzione all'assurdo** è una tecnica logica per dimostrare che una proposizione è vera, assumendo che sia falsa e mostrando che questa ipotesi conduce a una contraddizione.

**Schema:**

$$
\begin{align*}
1. & \; \text{Assumo che } \neg p \text{ sia vero (si assume che $ p $ sia falso)}. \\
2. & \; \text{Dimostro che questa ipotesi porta a una contraddizione } (q \land \neg q). \\
3. & \; \text{Concludo che } p \text{ deve essere vero, perché l'assunzione della sua falsità è assurda}.
\end{align*}
$$

**Esempio:**

- **Obiettivo**: Dimostrare che la radice quadrata di 2 è irrazionale.
- **Passo 1**: Supponiamo che $ \sqrt{2} $ sia razionale, ovvero si possa scrivere come $ \frac{a}{b} $, con $ a $ e $ b $ interi e coprimi.
- **Passo 2**: Squadrando entrambi i lati, otteniamo $ 2 = \frac{a^2}{b^2} $, cioè $ a^2 = 2b^2 $. Questo implica che $ a^2 $ è pari, e quindi $ a $ è pari.
- **Passo 3**: Se $ a $ è pari, allora possiamo scrivere $ a = 2k $. Sostituendo nell'equazione otteniamo $ 4k^2 = 2b^2 $, cioè $ b^2 = 2k^2 $. Quindi anche $ b $ è pari.
- **Passo 4**: Se sia $ a $ che $ b $ sono pari, questo contraddice l'ipotesi che $ a $ e $ b $ fossero coprimi.
- **Conclusione**: La supposizione iniziale che $ \sqrt{2} $ sia razionale porta a una contraddizione, quindi $ \sqrt{2} $ deve essere irrazionale.

---

### Esempi semplici di metodi deduttivi

1. **Modus Ponens**:
    - Se studio, allora supero l'esame.
    - Studio.
    - Conclusione: Supero l'esame.
2. **Modus Tollens**:
    - Se mangio troppo, ingrasso.
    - Non sono ingrassato.
    - Conclusione: Non ho mangiato troppo.
3. **Riduzione all'assurdo**:
    - Supponiamo che il numero 10 non sia divisibile per 2.
    - Ma 10 diviso 2 dà 5, che è un numero intero.
    - Conclusione: L'ipotesi che 10 non sia divisibile per 2 è falsa, quindi 10 è divisibile per 2.