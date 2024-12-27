# Regole di semplificazione

| **Regola**                           | **Espressione**                       | **Semplificazione**                               |
|--------------------------------------|--------------------------------------|--------------------------------------------------|
| **Legge dell'identità**              | $A \cdot 1 = A$                      | L'operatore AND con 1 non cambia l'espressione.  |
|                                      | $A + 0 = A$                          | L'operatore OR con 0 non cambia l'espressione.   |
| **Legge dell'annullamento**          | $A \cdot 0 = 0$                      | L'operatore AND con 0 annulla l'espressione.     |
|                                      | $A + 1 = 1$                          | L'operatore OR con 1 annulla l'espressione.      |
| **Legge della complementazione**     | $A \cdot \overline{A} = 0$           | AND tra una variabile e il suo complementare è 0.|
|                                      | $A + \overline{A} = 1$               | OR tra una variabile e il suo complementare è 1. |
| **Legge dell'idempotenza**           | $A \cdot A = A$                      | AND tra la stessa variabile non cambia l'espressione. |
|                                      | $A + A = A$                          | OR tra la stessa variabile non cambia l'espressione. |
| **Legge della doppia negazione**     | $\overline{\overline{A}} = A$        | La doppia negazione restituisce il valore originale. |
| **Legge di De Morgan**               | $\overline{A \cdot B} = \overline{A} + \overline{B}$ | La negazione di un AND è l'OR tra le negazioni. |
|                                      | $\overline{A + B} = \overline{A} \cdot \overline{B}$ | La negazione di un OR è l'AND tra le negazioni.  |
| **Legge di assorbimento**            | $A \cdot (A + B) = A$                | L'AND tra una variabile e un OR che la contiene è uguale alla variabile. |
|                                      | $A + (A \cdot B) = A$                | L'OR tra una variabile e un AND che la contiene è uguale alla variabile. |
| **Legge della distributività**       | $A \cdot (B + C) = (A \cdot B) + (A \cdot C)$ | L'AND distribuito sull'OR. |
|                                      | $A + (B \cdot C) = (A + B) \cdot (A + C)$ | L'OR distribuito sull'AND. |
| **Legge del complemento**            | $A \cdot \overline{A} = 0$           | AND tra una variabile e il suo complementare è 0.|
|                                      | $A + \overline{A} = 1$               | OR tra una variabile e il suo complementare è 1. |



# Esercizi di semplificazione di espressioni booleane

## "Facili"

## Esercizio 1
Semplifica l'espressione booleana:

$$
A \cdot (A + B)
$$

### Passo 1: Applicazione della Legge di Assorbimento
La legge di assorbimento afferma che:

$$
A \cdot (A + B) = A
$$

Poiché se $A$ è vero, il termine $A + B$ diventa sempre vero, quindi la moltiplicazione con $A$ lascia invariato il valore di $A$.

### Soluzione finale:
$$
A
$$

---

## Esercizio 2
Semplifica l'espressione booleana:

$$
A + A \cdot B
$$

### Passo 1: Applicazione della Legge di Assorbimento
La legge di assorbimento afferma che:

$$
A + A \cdot B = A
$$

Infatti, se $A$ è vero, l'espressione sarà vera indipendentemente dal valore di $B$.

### Soluzione finale:
$$
A
$$

---

## Esercizio 3
Semplifica l'espressione booleana:

$$
A \cdot \overline{A}
$$

### Passo 1: Applicazione della Legge del Complemento
La legge del complemento afferma che:

$$
A \cdot \overline{A} = 0
$$

Poiché $A$ e $\overline{A}$ sono due eventi mutuamente esclusivi (non possono essere veri contemporaneamente).

### Soluzione finale:
$$
0
$$

---

## Esercizio 4
Semplifica l'espressione booleana:

$$
A \cdot B + \overline{A} \cdot B
$$

### Passo 1: Applicazione della Legge di Fattorizzazione
Notiamo che entrambi i termini hanno il fattore $B$, quindi possiamo fattorizzare l'espressione come:

$$
B \cdot (A + \overline{A})
$$

### Passo 2: Applicazione della Legge di Identità
La legge di identità afferma che:

$$
A + \overline{A} = 1
$$

Quindi l'espressione diventa:

$$
B \cdot 1 = B
$$

### Soluzione finale:
$$
B
$$

---

## Esercizio 5
Semplifica l'espressione booleana:

$$
A + A \cdot B + B
$$

### Passo 1: Applicazione della Legge di Assorbimento
Possiamo applicare la legge di assorbimento:

$$
A + A \cdot B = A
$$

Quindi l'espressione diventa:

$$
A + B
$$

### Soluzione finale:
$$
A + B
$$


## "Medi"

# Esercizi di semplificazione di espressioni booleane (Difficoltà Media)

## Esercizio 1
Semplifica l'espressione booleana:

$$
A \cdot (B + \overline{A}) + A \cdot B
$$

### Passo 1: Espandere l'espressione
Applichiamo la distributività per espandere:

$$
A \cdot (B + \overline{A}) = A \cdot B + A \cdot \overline{A}
$$

Quindi l'espressione diventa:

$$
A \cdot B + A \cdot \overline{A} + A \cdot B
$$

### Passo 2: Semplificare i termini simili
Notiamo che il termine $A \cdot B$ appare due volte, quindi possiamo sommarli:

$$
A \cdot B + A \cdot \overline{A}
$$

### Passo 3: Applicazione della Legge del Complemento
La legge del complemento afferma che:

$$
A \cdot \overline{A} = 0
$$

Quindi l'espressione diventa:

$$
A \cdot B + 0 = A \cdot B
$$

### Soluzione finale:
$$
A \cdot B
$$

---

## Esercizio 2
Semplifica l'espressione booleana:

$$
(A + B) \cdot (A + \overline{B})
$$

### Passo 1: Applicazione della distributività
Espandiamo l'espressione applicando la legge distributiva:

$$
(A + B) \cdot (A + \overline{B}) = A \cdot A + A \cdot \overline{B} + B \cdot A + B \cdot \overline{B}
$$

### Passo 2: Semplificare i termini
Semplifichiamo i termini in base alle leggi booleane:

- $A \cdot A = A$ (legge dell'idempotenza)
- $B \cdot \overline{B} = 0$ (legge del complemento)

Quindi l'espressione diventa:

$$
A + A \cdot \overline{B} + B \cdot A
$$

### Passo 3: Fattorizzare i termini
Notiamo che $A$ appare in entrambi i termini $A$ e $A \cdot \overline{B}$ e $B \cdot A$, quindi possiamo fattorizzare:

$$
A \cdot (1 + \overline{B} + B)
$$

### Passo 4: Applicazione della Legge di Identità
La legge di identità afferma che:

$$
1 + \overline{B} + B = 1
$$

Quindi l'espressione diventa:

$$
A \cdot 1 = A
$$

### Soluzione finale:
$$
A
$$

---

## Esercizio 3
Semplifica l'espressione booleana:

$$
A \cdot (B + C) + \overline{A} \cdot (B + C)
$$

### Passo 1: Applicazione della legge distributiva
Possiamo applicare la legge distributiva per separare i termini:

$$
A \cdot (B + C) + \overline{A} \cdot (B + C) = (A + \overline{A}) \cdot (B + C)
$$

### Passo 2: Applicazione della Legge di Identità
La legge di identità afferma che:

$$
A + \overline{A} = 1
$$

Quindi l'espressione diventa:

$$
1 \cdot (B + C) = B + C
$$

### Soluzione finale:
$$
B + C
$$

---

## Esercizio 4
Semplifica l'espressione booleana:

$$
(A + B) \cdot (A + \overline{B} + C)
$$

### Passo 1: Applicazione della legge distributiva
Espandiamo l'espressione:

$$
(A + B) \cdot (A + \overline{B} + C) = A \cdot (A + \overline{B} + C) + B \cdot (A + \overline{B} + C)
$$

### Passo 2: Espandere ulteriormente
Applichiamo la distributività:

$$
A \cdot (A + \overline{B} + C) = A \cdot A + A \cdot \overline{B} + A \cdot C
$$
$$
B \cdot (A + \overline{B} + C) = B \cdot A + B \cdot \overline{B} + B \cdot C
$$

Ora l'espressione diventa:

$$
A \cdot A + A \cdot \overline{B} + A \cdot C + B \cdot A + B \cdot \overline{B} + B \cdot C
$$

### Passo 3: Semplificare i termini
Semplifichiamo i termini usando le leggi booleane:

- $A \cdot A = A$ (legge dell'idempotenza)
- $B \cdot \overline{B} = 0$ (legge del complemento)

L'espressione diventa:

$$
A + A \cdot \overline{B} + A \cdot C + B \cdot A + B \cdot C
$$

### Passo 4: Applicazione della Legge di Assorbimento
$A + A \cdot B = A$, quindi possiamo semplificare ulteriormente:

$$
A + B \cdot C
$$

### Soluzione finale:
$$
A + B \cdot C
$$

---

## Esercizio 5
Semplifica l'espressione booleana:

$$
A \cdot B + A \cdot \overline{C} + B \cdot \overline{C}
$$

### Passo 1: Fattorizzare i termini comuni
Iniziamo cercando i termini comuni. I termini $A \cdot B$ e $B \cdot \overline{C}$ hanno $B$ come fattore comune:

$$
A \cdot B + B \cdot \overline{C} + A \cdot \overline{C} = B \cdot (A + \overline{C}) + A \cdot \overline{C}
$$

### Passo 2: Semplificare ulteriormente
Ora possiamo applicare la legge distributiva al termine $B \cdot (A + \overline{C})$:

$$
B \cdot (A + \overline{C}) + A \cdot \overline{C}
$$

Espandiamo:

$$
= B \cdot A + B \cdot \overline{C} + A \cdot \overline{C}
$$

Notiamo che $A \cdot \overline{C}$ è già presente nell'espressione. Quindi, l'espressione diventa:

$$
B \cdot A + B \cdot \overline{C} + A \cdot \overline{C}
$$

### Soluzione finale:
$$
B \cdot A + A \cdot \overline{C} + B \cdot \overline{C}
$$
L'espressione non può essere semplificata ulteriormente in modo significativo. Questo è il risultato finale.


## "Difficili"
# Esercizi di semplificazione di espressioni booleane (Difficoltà Alta)

## Esercizio 1
Semplifica l'espressione booleana:

$$
A \cdot (B + C) + \overline{A} \cdot (B + \overline{C})
$$

### Passo 1: Applicazione della legge distributiva
Applichiamo la legge distributiva:

$$
A \cdot (B + C) = A \cdot B + A \cdot C
$$
$$
\overline{A} \cdot (B + \overline{C}) = \overline{A} \cdot B + \overline{A} \cdot \overline{C}
$$

Quindi l'espressione diventa:

$$
A \cdot B + A \cdot C + \overline{A} \cdot B + \overline{A} \cdot \overline{C}
$$

### Passo 2: Fattorizzare i termini comuni
Notiamo che $B$ appare in $A \cdot B$ e $\overline{A} \cdot B$, quindi possiamo fattorizzare:

$$
B \cdot (A + \overline{A}) + A \cdot C + \overline{A} \cdot \overline{C}
$$

### Passo 3: Applicazione della Legge di Identità
La legge di identità afferma che:

$$
A + \overline{A} = 1
$$

Quindi l'espressione diventa:

$$
B \cdot 1 + A \cdot C + \overline{A} \cdot \overline{C}
$$

### Passo 4: Semplificare
Ora l'espressione diventa:

$$
B + A \cdot C + \overline{A} \cdot \overline{C}
$$

### Soluzione finale:
$$
B + A \cdot C + \overline{A} \cdot \overline{C}
$$

---

## Esercizio 2
Semplifica l'espressione booleana:

$$
A \cdot (B + C) + \overline{A} \cdot (B + C) \cdot \overline{D}
$$

### Passo 1: Applicazione della legge distributiva
Applichiamo la legge distributiva alla seconda parte dell'espressione:

$$
\overline{A} \cdot (B + C) \cdot \overline{D} = \overline{A} \cdot (B \cdot \overline{D}) + \overline{A} \cdot (C \cdot \overline{D})
$$

Ora l'espressione diventa:

$$
A \cdot (B + C) + \overline{A} \cdot (B \cdot \overline{D}) + \overline{A} \cdot (C \cdot \overline{D})
$$

### Passo 2: Fattorizzare i termini comuni
Fattorizziamo il termine $A$ nella prima parte dell'espressione:

$$
A \cdot (B + C) + \overline{A} \cdot (B \cdot \overline{D} + C \cdot \overline{D})
$$

### Passo 3: Analizzare l'espressione
L'espressione ora è più semplice, ma non si può semplificare ulteriormente con leggi booleane standard. Dobbiamo lasciare l'espressione come tale.

### Soluzione finale:
$$
A \cdot (B + C) + \overline{A} \cdot (B \cdot \overline{D} + C \cdot \overline{D})
$$

---

## Esercizio 3
Semplifica l'espressione booleana:

$$
A \cdot \overline{B} \cdot C + A \cdot B \cdot C + \overline{A} \cdot B \cdot C + A \cdot \overline{C}
$$

### Passo 1: Raggruppare i termini
Raggruppiamo i termini in modo da applicare le leggi booleane:

$$
(A \cdot \overline{B} \cdot C + A \cdot B \cdot C) + (\overline{A} \cdot B \cdot C + A \cdot \overline{C})
$$

### Passo 2: Fattorizzare
Fattorizziamo i termini comuni:

$$
A \cdot C \cdot (\overline{B} + B) + \overline{A} \cdot B \cdot C + A \cdot \overline{C}
$$

### Passo 3: Applicazione della Legge di Identità
La legge di identità afferma che:

$$
\overline{B} + B = 1
$$

Quindi l'espressione diventa:

$$
A \cdot C + \overline{A} \cdot B \cdot C + A \cdot \overline{C}
$$

### Passo 4: Raggruppare ulteriormente
Notiamo che i primi due termini contengono $A$ e $C$, quindi possiamo raggrupparli:

$$
A \cdot (C + \overline{C}) + \overline{A} \cdot B \cdot C
$$

### Passo 5: Applicazione della Legge di Identità
La legge di identità afferma che:

$$
C + \overline{C} = 1
$$

Quindi l'espressione diventa:

$$
A \cdot 1 + \overline{A} \cdot B \cdot C
$$

### Passo 6: Semplificazione
L'espressione si semplifica a:

$$
A + \overline{A} \cdot B \cdot C
$$

### Soluzione finale:
$$
A + \overline{A} \cdot B \cdot C
$$


## Esercizio 4
Semplifica l'espressione booleana:

$$
A \cdot (B + C) \cdot (\overline{B} + D) + \overline{A} \cdot (B + C) \cdot (D + \overline{C})
$$

### Passo 1: Espandere i termini
Cominciamo espandendo i termini:

$$
A \cdot (B + C) \cdot (\overline{B} + D) = A \cdot (B \cdot \overline{B} + B \cdot D + C \cdot \overline{B} + C \cdot D)
$$

$$
\overline{A} \cdot (B + C) \cdot (D + \overline{C}) = \overline{A} \cdot (B \cdot D + B \cdot \overline{C} + C \cdot D + C \cdot \overline{C})
$$

$$
A \cdot \overline{B} \cdot C
$$

### Passo 2: Semplificare i termini
- $B \cdot \overline{B} = 0$ (legge del complemento)
- $C \cdot \overline{C} = 0$ (legge del complemento)

Quindi l'espressione diventa:

$$
A \cdot (B \cdot D + C \cdot \overline{B} + C \cdot D) + \overline{A} \cdot (B \cdot D + B \cdot \overline{C} + C \cdot D) + A \cdot \overline{B} \cdot C
$$

### Passo 3: Raggruppare i termini
Raggruppiamo i termini con $B \cdot D$ e $C \cdot D$:

$$
(A \cdot B \cdot D + A \cdot C \cdot \overline{B} + A \cdot C \cdot D) + (\overline{A} \cdot B \cdot D + \overline{A} \cdot B \cdot \overline{C} + \overline{A} \cdot C \cdot D) + A \cdot \overline{B} \cdot C
$$

### Passo 4: Fattorizzare
Notiamo che $B \cdot D$ e $C \cdot D$ compaiono in entrambi i gruppi. Fattorizziamo:

$$
B \cdot D \cdot (A + \overline{A}) + C \cdot D \cdot (A + \overline{A}) + A \cdot C \cdot \overline{B} + \overline{A} \cdot B \cdot \overline{C}
$$

### Passo 5: Applicazione della Legge di Identità
La legge di identità afferma che:

$$
A + \overline{A} = 1
$$

Quindi l'espressione diventa:

$$
B \cdot D + C \cdot D + A \cdot C \cdot \overline{B} + \overline{A} \cdot B \cdot \overline{C}
$$

### Soluzione finale:
$$
B \cdot D + C \cdot D + A \cdot C \cdot \overline{B} + \overline{A} \cdot B \cdot \overline{C}
$$

---

## Esercizio 5
Semplifica l'espressione booleana:

$$
A \cdot (B + C) \cdot (\overline{B} + D) + \overline{A} \cdot (B + C) \cdot (D + \overline{C}) + A \cdot \overline{B} \cdot C
$$

### Passo 1: Espandere i termini
Cominciamo espandendo i termini:

$$
A \cdot (B + C) \cdot (\overline{B} + D) = A \cdot (B \cdot \overline{B} + B \cdot D + C \cdot \overline{B} + C \cdot D)
$$

$$
\overline{A} \cdot (B + C) \cdot (D + \overline{C}) = \overline{A} \cdot (B \cdot D + B \cdot \overline{C} + C \cdot D + C \cdot \overline{C})
$$

$$
A \cdot \overline{B} \cdot C
$$

### Passo 2: Semplificare i termini
- $B \cdot \overline{B} = 0$ (legge del complemento)
- $C \cdot \overline{C} = 0$ (legge del complemento)

Quindi l'espressione diventa:

$$
A \cdot (B \cdot D + C \cdot \overline{B} + C \cdot D) + \overline{A} \cdot (B \cdot D + B \cdot \overline{C} + C \cdot D) + A \cdot \overline{B} \cdot C
$$

### Passo 3: Raggruppare i termini
Raggruppiamo i termini simili:

$$
(A \cdot B \cdot D + A \cdot C \cdot \overline{B} + A \cdot C \cdot D) + (\overline{A} \cdot B \cdot D + \overline{A} \cdot B \cdot \overline{C} + \overline{A} \cdot C \cdot D) + A \cdot \overline{B} \cdot C
$$

### Passo 4: Fattorizzare i termini
Notiamo che $B \cdot D$ e $C \cdot D$ appaiono in entrambi i gruppi. Fattorizziamo:

$$
B \cdot D \cdot (A + \overline{A}) + C \cdot D \cdot (A + \overline{A}) + A \cdot C \cdot \overline{B} + \overline{A} \cdot B \cdot \overline{C} + A \cdot \overline{B} \cdot C
$$

### Passo 5: Applicazione della Legge di Identità
La legge di identità afferma che:

$$
A + \overline{A} = 1
$$

Quindi l'espressione diventa:

$$
B \cdot D + C \cdot D + A \cdot C \cdot \overline{B} + \overline{A} \cdot B \cdot \overline{C} + A \cdot \overline{B} \cdot C
$$

### Soluzione finale:
$$
B \cdot D + C \cdot D + A \cdot C \cdot \overline{B} + \overline{A} \cdot B \cdot \overline{C} + A \cdot \overline{B} \cdot C
$$
---