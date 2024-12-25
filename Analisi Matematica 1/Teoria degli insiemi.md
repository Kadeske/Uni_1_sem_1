---
~
---
La **teoria degli insiemi** è la branca della matematica che studia gli insiemi, cioè collezioni di oggetti distinti chiamati **elementi**. Questa teoria, sviluppata da **Georg Cantor**, è alla base della matematica moderna.

### Definizione di insieme

Un **insieme** è una collezione di oggetti distinti e determinati, chiamati **elementi**. Gli insiemi sono indicati con lettere maiuscole, mentre i loro elementi con lettere minuscole.

**Esempio**:

- L'insieme $A = {1, 2, 3}$ contiene gli elementi 1, 2 e 3.

---

### Modi di rappresentare un insieme

1. **Rappresentazione estensiva** (per elencazione): si elencano esplicitamente tutti gli elementi dell'insieme.
    
    - **Esempio**: $A = {1, 3, 5}$
2. **Rappresentazione intensiva** (per proprietà): si definiscono le proprietà che caratterizzano gli elementi dell'insieme.
    
    - **Esempio**: $B = {x \in \mathbb{N} \mid x \text{ è dispari e } x < 6}$
3. **Rappresentazione grafica**: con i **diagrammi di Eulero-Venn**, che visualizzano gli insiemi come cerchi e le relazioni tra essi (unione, intersezione, ecc.).
    

---

### Appartenenza ad un insieme

Un oggetto **appartiene** a un insieme se soddisfa la proprietà che lo caratterizza. Si indica con il simbolo $ \in $, e la **non appartenenza** con $ \notin $.

- **Esempio**: Se $A = {1, 2, 3}$, allora $2 \in A$ (2 appartiene ad $A$) e $4 \notin A$ (4 non appartiene ad $A$).

---

### Cardinalità di un insieme

La **cardinalità** di un insieme è il numero degli elementi contenuti in esso, indicata con $\#A$.

- **Esempio**: Se $A = {1, 2, 3}$, la cardinalità di $A$ è $\#A = 3$.

---

### Insieme vuoto

L'**insieme vuoto** è l'insieme che non contiene alcun elemento e si indica con $\emptyset $ o ${}$.

- **Esempio**: L'insieme dei numeri naturali minori di 1 è l'insieme vuoto: $ \emptyset = {x \in \mathbb{N} \mid x < 1}$.

---

### Sottoinsiemi

Un **sottoinsieme** $A$ di un insieme $B$ è un insieme i cui elementi appartengono tutti a $B$. Si indica con $A \subseteq B$.

- **Esempio**: Se $A = {1, 3}$ e $B = {1, 2, 3, 4}$, allora $A \subseteq B$.

Un **sottoinsieme improprio** è un sottoinsieme che coincide con l'insieme di partenza, ossia $A \subseteq A$ e l'insieme vuoto $ \emptyset $ è sempre un sottoinsieme improprio di qualsiasi insieme.

---

### Operazioni tra insiemi

1. **Unione** $A \cup B$: l'unione di due insiemi è l'insieme degli elementi che appartengono ad almeno uno dei due insiemi.
    
    - **Esempio**: Se $A = {1, 2}$ e $B = {2, 3}$, allora $A \cup B = {1, 2, 3}$.
2. **Intersezione** $A \cap B$: l'intersezione di due insiemi è l'insieme degli elementi comuni a entrambi gli insiemi.
    
    - **Esempio**: Se $A = {1, 2}$ e $B = {2, 3}$, allora $A \cap B = {2}$.
3. **Differenza** $A \setminus B$: la differenza tra due insiemi è l'insieme degli elementi che appartengono ad $A$ ma non a $B$.
    
    - **Esempio**: Se $A = {1, 2, 3}$ e $B = {2, 3}$, allora $A \setminus B = {1}$.
4. **Complemento** $A^c$: il complemento di un insieme $A$ rispetto all'insieme universo $U$ è l'insieme degli elementi di $U$ che non appartengono ad $A$. Si rappresenta come $U \setminus A$.
    
    - **Esempio**: Se l'universo è $U = {1, 2, 3, 4}$ e $A = {1, 2}$, allora $A^c = {3, 4}$.

**Approfondimento**: La **complementazione** è utile per descrivere ciò che non è incluso in un insieme rispetto a un contesto generale (l'universo). Per esempio, in logica o teoria degli insiemi, il complemento di un insieme rappresenta tutte le alternative possibili che non soddisfano le condizioni dell'insieme originale.

---

### Insieme delle parti

L'**insieme delle parti** di un insieme $A$, indicato con $\mathcal{P}(A)$, è l'insieme di tutti i sottoinsiemi di $A$, inclusi l'insieme vuoto e $A$ stesso.

- **Esempio**: Se $A = {1, 2}$, allora $\mathcal{P}(A) = {\emptyset, {1}, {2}, {1, 2}}$.

La cardinalità dell'insieme delle parti è $2^n$, dove $n$ è il numero degli elementi di $A$.

---

### Prodotto cartesiano

Il **prodotto cartesiano** di due insiemi $A$ e $B$, indicato con $A \times B$, è l'insieme delle coppie ordinate $(a, b)$ dove $a$ appartiene ad $A$ e $b$ appartiene a $B$.

- **Esempio**: Se $A = {1, 2}$ e $B = {a, b}$, allora $A \times B = {(1, a), (1, b), (2, a), (2, b)}$.

La **cardinalità** del prodotto cartesiano è il prodotto delle cardinalità degli insiemi: $\#(A \times B) = \#A \times \#B$.

**Approfondimento**: Il **prodotto cartesiano** è un concetto fondamentale che trova applicazione in molte aree della matematica, come la teoria delle relazioni e la costruzione di funzioni. Descrive tutte le possibili combinazioni tra due insiemi.

---

### Esercizi pratici

1. **Dato** $A = {1, 3, 5, 7}$ e $B = {4, 7, 8, 9}$, trova:
    
    - $A \cap B = {7}$
    - $A \cup B = {1, 3, 4, 5, 7, 8, 9}$
    - $A \setminus B = {1, 3, 5}$
2. **Prodotto cartesiano**:
    
    - Se $A = {x, y}$ e $B = {1, 2}$, allora $A \times B = {(x, 1), (x, 2), (y, 1), (y, 2)}$.

