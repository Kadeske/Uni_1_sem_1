### Relazioni binarie

Una **relazione binaria** tra due insiemi $A$ e $B$ è un sottoinsieme del **prodotto cartesiano** $A \times B$. Il prodotto cartesiano rappresenta tutte le possibili coppie ordinate tra elementi di $A$ e $B$, mentre una relazione binaria seleziona alcune di queste coppie, stabilendo un legame specifico.

- **Esempio**: Se $A = {2}$ e $B = {1, 3}$, il prodotto cartesiano $A \times B = {(2, 1), (2, 3)}$. Una possibile relazione è $R = {(2, 3)}$.

### Modi di rappresentare una relazione

1. **Elencazione**: elenca le coppie della relazione.
	    
    - **Esempio**: $R = {(2, 3)}$
2. **Proprietà caratteristica**: si descrive con una proprietà che devono soddisfare le coppie.
    
    - **Esempio**: $R = {(a, b) \in A \times B \mid a < b}$
3. **Diagramma a frecce**: le frecce collegano i valori di $A$ con quelli di $B$.
    
    - **Esempio grafico**:  
        $A = {2}$, $B = {1, 3}$  
        
4. **Tabella a doppia entrata**: le righe corrispondono agli elementi di $A$ e le colonne a quelli di $B$.
    
    - **Esempio**:
    
    $132(2, 1)(2, 3)\begin{array}{c|c c} & 1 & 3 \\ 2 & \text{(2, 1)} & \text{(2, 3)} \\ \end{array}2​1(2, 1)​3(2, 3)​$

---

### Proprietà di una relazione

Le relazioni possono avere alcune **proprietà** particolari:

1. **Riflessiva**: Ogni elemento è in relazione con se stesso.
	    $A = {1,2}$
	    $AxA = {(1,1),(2,2)}$
	- **Esempio**: $\forall a \in A$, $a R a$
2. **Antiriflessiva**: Nessun elemento è in relazione con se stesso.
    
    - **Esempio**: $\forall a \in A$, $a R a$ non è vero.
3. **Simmetrica**: Se $a R b$, allora $b R a$.
    
    - **Esempio**: Se $a = 1$, $b = 2$, allora $1 R 2 \implies 2 R 1$.
4. **Antisimmetrica**: Se $a R b$ e $b R a$, allora $a = b$.
    
    - **Esempio**: Se $1 R 2$, non può accadere che $2 R 1$.
5. **Transitiva**: Se $a R b$ e $b R c$, allora $a R c$.
    
    - **Esempio**: Se $1 R 2$ e $2 R 3$, allora $1 R 3$.

---

### Relazioni di equivalenza

Una relazione è detta **relazione di equivalenza** se è:

- **Riflessiva**: $\forall a \in A$, $a R a$.
- **Simmetrica**: Se $a R b$, allora $b R a$.
- **Transitiva**: Se $a R b$ e $b R c$, allora $a R c$.

**Esempio**: La relazione "avere lo stesso resto nella divisione per 5" è una relazione di equivalenza.

---

### Relazioni d'ordine

Una relazione è detta **relazione d'ordine** se è:

- **Antisimmetrica**: Se $a R b$ e $b R a$, allora $a = b$.
- **Transitiva**: Se $a R b$ e $b R c$, allora $a R c$.

**Esempio**: La relazione "essere maggiore o uguale a" ($\geq$) è una relazione d'ordine.

---

## Funzioni

Una **funzione** da un insieme $A$ a un insieme $B$ è una particolare relazione binaria che associa **ad ogni elemento di $A$ uno ed un solo elemento di $B$**.

- **Dominio**: l'insieme $A$, cioè l'insieme di partenza.
- **Codominio**: l'insieme $B$, cioè l'insieme di arrivo.
- **Immagine**: il sottoinsieme di $B$ formato dagli elementi effettivamente associati a qualche elemento di $A$.

### Esempio

- Funzione $f: A \rightarrow B$
- $A = {1, 2}$, $B = {2, 4, 6}$
- Definizione di $f$: $f(x) = 2x$

Rappresentazione della funzione:

- $f(1) = 2$
- $f(2) = 4$

**Grafico** della funzione:

- Coppie ordinate $(x, f(x))$: ${(1, 2), (2, 4)}$
- **Rappresentazione grafica**:  
    

---

### Tipi di funzioni

1. **Iniettiva**: Una funzione $f: A \rightarrow B$ si dice **iniettiva** se a ogni elemento distinto di $A$ corrisponde un elemento distinto di $B$.
    
    - **Esempio**: $f(x) = 2x$ con $A = {1, 2}$ e $B = {2, 4}$ è iniettiva perché $f(1) \neq f(2)$.
2. **Suriettiva**: Una funzione $f: A \rightarrow B$ si dice **suriettiva** se l'immagine di $A$ è uguale a tutto $B$, cioè ogni elemento di $B$ è immagine di almeno un elemento di $A$.
    
    - **Esempio**: Se $A = {1, 2}$ e $B = {2, 4}$, $f(x) = 2x$ è suriettiva perché tutti gli elementi di $B$ sono coperti.
3. **Biunivoca (Bigettiva)**: Una funzione è **biunivoca** se è sia iniettiva che suriettiva. In questo caso, ogni elemento di $B$ è associato a un solo elemento di $A$ e viceversa.
    

---

### Funzione inversa

Una funzione $f: A \rightarrow B$ ha una **funzione inversa** $f^{-1}: B \rightarrow A$ se e solo se $f$ è biunivoca. La funzione inversa "inverte" le coppie della funzione originale, cioè scambia il dominio con il codominio.

- **Esempio**: Se $f(x) = 2x$, la funzione inversa è $f^{-1}(x) = \frac{x}{2}$.

---

### Composizione di funzioni

Se $f: A \rightarrow B$ e $g: B \rightarrow C$ sono due funzioni, la **composizione** $g \circ f$ è una funzione da $A$ a $C$ definita come:

(g∘f)(x)=g(f(x))(g \circ f)(x) = g(f(x))(g∘f)(x)=g(f(x))

- **Esempio**: Se $f(x) = 2x$ e $g(y) = y - 1$, allora $(g \circ f)(x) = g(f(x)) = 2x - 1$.

---

### Esempi pratici

1. **Composizione di funzioni**:
    - $f: {1, 2} \rightarrow {2, 4}$ definita come $f(x) = 2x$
    - $g: {2, 4} \rightarrow {1, 3}$ definita come $g(y) = y - 1$
    - **Composizione** $g \circ f: {1, 2} \rightarrow {1, 3}$ è data da $(g \circ f)(x) = 2x - 1$.