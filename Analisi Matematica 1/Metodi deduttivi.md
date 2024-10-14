I **metodi deduttivi** sono tecniche logiche utilizzate per derivare conclusioni a partire da premesse. I principali metodi deduttivi sono il **Modus Ponens**, il **Modus Tollens** e la **Riduzione all'assurdo**.

---

#### Modus Ponens (Affermando il conseguente)

Il **Modus Ponens** è una regola di inferenza che permette di dedurre la verità di una proposizione a partire da un'implicazione e dall'affermazione dell'antecedente.

**Forma:**

- Se p⇒qp \Rightarrow qp⇒q è vero, e ppp è vero, allora qqq è vero.

**Schema:**

1. p⇒qp \Rightarrow qp⇒q (Se ppp allora qqq)
2. ppp (Affermo che ppp è vero)
3. qqq (Concludo che qqq è vero)

**Esempio:**

- **Premessa 1**: Se piove, allora le strade sono bagnate. p⇒qp -> qp⇒q
- **Premessa 2**: Piove. ppp
- **Conclusione**: Le strade sono bagnate. qqq

**Errore comune:**

- Sbagliato: Se affermassi qqq (strade bagnate) senza sapere se ppp è vero (pioggia), non posso concludere che ppp sia vero.

---

#### Modus Tollens (Negando il conseguente)

Il **Modus Tollens** permette di dedurre la falsità di una proposizione dall'implicazione e dalla negazione del conseguente.

**Forma:**

- Se p⇒qp \Rightarrow qp⇒q è vero e qqq è falso, allora ppp è falso.

**Schema:**

1. p⇒qp \Rightarrow qp⇒q (Se ppp allora qqq)
2. ¬q\neg q¬q (Affermo che qqq è falso)
3. ¬p\neg p¬p (Concludo che ppp è falso)

**Esempio:**

- **Premessa 1**: Se piove, le strade sono bagnate. p⇒qp -> qp⇒q
- **Premessa 2**: Le strade non sono bagnate. ¬q\neg q¬q
- **Conclusione**: Non piove. ¬p\neg p¬p

**Errore comune:**

- Sbagliato: Non posso dedurre che qqq sia falso solo perché non ho osservato ppp. Ad esempio, le strade potrebbero essere bagnate per altre cause (ad esempio, un lavaggio).

---

#### Riduzione all'assurdo (Contraddizione)

La **riduzione all'assurdo** è una tecnica logica per dimostrare che una proposizione è vera, assumendo che sia falsa e mostrando che questa ipotesi conduce a una contraddizione.

**Schema:**

1. Assumo che ¬p\neg p¬p sia vero (si assume che ppp sia falso).
2. Dimostro che questa ipotesi porta a una contraddizione (q∧¬qq \land \neg qq∧¬q).
3. Concludo che ppp deve essere vero, perché l'assunzione della sua falsità è assurda.

**Esempio:**

- **Obiettivo**: Dimostrare che la radice quadrata di 2 è irrazionale.
- **Passo 1**: Supponiamo che 2\sqrt{2}2​ sia razionale, ovvero si possa scrivere come ab\frac{a}{b}ba​, con aaa e bbb interi e coprimi.
- **Passo 2**: Squadrando entrambi i lati, otteniamo 2=a2b22 = \frac{a^2}{b^2}2=b2a2​, cioè a2=2b2a^2 = 2b^2a2=2b2. Questo implica che a2a^2a2 è pari, e quindi aaa è pari.
- **Passo 3**: Se aaa è pari, allora possiamo scrivere a=2ka = 2ka=2k. Sostituendo nell'equazione otteniamo 4k2=2b24k^2 = 2b^24k2=2b2, cioè b2=2k2b^2 = 2k^2b2=2k2. Quindi anche bbb è pari.
- **Passo 4**: Se sia aaa che bbb sono pari, questo contraddice l'ipotesi che aaa e bbb fossero coprimi.
- **Conclusione**: La supposizione iniziale che 2\sqrt{2}2​ sia razionale porta a una contraddizione, quindi 2\sqrt{2}2​ deve essere irrazionale.

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