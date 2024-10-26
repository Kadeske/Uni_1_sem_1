### Proposizione o enunciato

Una **proposizione** è un'espressione del linguaggio per la quale ha senso domandarsi se è **vera** o **falsa**.

**Esempi:**

- _Hai sonno?_ → non è una proposizione (è una domanda).
- _2 + 1 = 3_ → è una proposizione **vera**.
- _x > 4_ → non è decidibile finché non si assegna un valore a xxx.
- _La luna è lontana._ → non è chiaro da cosa, quindi non ha senso domandarsi se è vera o falsa.

Ad ogni proposizione può essere associato un **valore di verità** che può essere **VERO** o **FALSO**. Non esistono altri valori.

Una proposizione è **decidibile** se è possibile attribuirle un valore di verità attraverso una serie finita di passi.

---

### Principi della logica binaria

- **Principio di identità:** ogni proposizione ha lo stesso valore di verità di se stessa.
- **Principio di non contraddizione:** una proposizione non può essere simultaneamente vera e falsa.
- **Principio del terzo escluso:** una proposizione può essere solo vera o falsa. Non esistono altri valori di verità.

---

### Connettivi logici

Un **enunciato semplice** ha un valore di verità determinabile direttamente.  
Un **enunciato composto** è formato da due o più enunciati semplici legati da **connettivi logici**.

**Connettivo**: operatore che permette di costruire enunciati composti a partire da quelli elementari.

---

## Connettivi unari

| **p** | **i** (Identità) | **¬p** (Negazione) |
| ----- | ---------------- | ------------------ |
| VERO  | VERO             | FALSO              |
| FALSO | FALSO            | VERO               |

**Esempio:**

- **Identità**: se p = VERO allora i(p) = VERO.
    - _Giusto_: "La Terra è un pianeta" → è vera e resta vera con l'identità.
    - _Sbagliato_: "La Terra è piatta" → è falsa e non diventa vera con l'identità.
- **Negazione**: se p = VERO allora ¬(p) = FALSO
    - _Giusto_: "Non è vero che 2 + 2 = 5" → correttamente negato.
    - _Sbagliato_: "Non è vero che 2 + 2 = 4" → errato, perché nega una verità.

---

## Connettivi binari

### Tabella dei connettivi binari

| **p** | **q** | **p ∧ q** (AND) | **p ∨ q** (OR) | **p ⇒ q** (Implica) | **p ⇔ q** (Equivalente) | **p ⊕ q** (XOR) |
| ----- | ----- | --------------- | -------------- | ------------------- | ----------------------- | --------------- |
| VERO  | VERO  | VERO            | VERO           | VERO                | VERO                    | FALSO           |
| VERO  | FALSO | FALSO           | VERO           | FALSO               | FALSO                   | VERO            |
| FALSO | VERO  | FALSO           | VERO           | VERO                | FALSO                   | VERO            |
| FALSO | FALSO | FALSO           | FALSO          | VERO                | VERO                    | FALSO           |

### Esempi per ciascun connettivo

1. **Congiunzione (AND, ∧)**:
    
    - *p*∧*q* è vero solo se entrambi *p* e *q* sono veri.
    - _Giusto_: "Piove **e** fa freddo" → entrambe le condizioni sono vere.
    - _Sbagliato_: "Piove **e** c'è il sole" → falsa perché una delle condizioni è falsa.
2. **Disgiunzione (OR, ∨)**:
    
    - p∨q è vero se almeno uno tra p e q è vero.
    - _Giusto_: "Piove **o** fa freddo" → vero, perché fa freddo (anche se non piove).
    - _Sbagliato_: "Piove **o** nevica" → falso se entrambe le condizioni sono false.
3. **Implicazione (IF-THEN, ⇒)**:
	- **Definizione**: p⇒q è falso solo se p è vero e q è falso.
	- **Esempio Corretto**:
	    - "Se studio, passo l'esame" → Questo è vero se lo studio porta al risultato desiderato.
	- **Esempio Errato**:
	    - "Se studio, fallisco l'esame" → Questo è errato, perché se si studia, non dovrebbe portare al fallimento.
	- **Attenzione**:
	    - "Se non studio, passo l'esame" → Questo può essere vero, perché il risultato è stato ugualmente raggiunto nonostante la mancanza di studio.
1. **Equivalenza (IF AND ONLY IF, ⇔)**:
	-  l'espressione a↔b è equivalente all'espressione (a→b)∧(b→a)
    - p⇔q  è vero se p e q hanno lo stesso valore di verità.
    - _Giusto_: "Un numero è pari **se e solo se** è divisibile per 2".
    - _Sbagliato_: "Un numero è pari **se e solo se** è dispari" → contraddittorio.
5. **Disgiunzione esclusiva (XOR, ⊕)**:
    
    - p⊕q  è vero solo se uno tra p e q è vero, ma non entrambi.
    - _Giusto_: "Oggi vado al mare **o** in montagna" → vero se faccio una sola delle due cose.
    - _Sbagliato_: "Vado al mare **o** vado al mare" → falsa perché entrambe le scelte sono la stessa.

#### Condizioni

- **Sufficiente**: Se p è vero, allora q è vero ( $p→q$ ).
    - Esempio: "Se piove, la strada davanti casa è bagnata".
- **Necessaria**: Se p non è vero, allora q non è vero ( $p\⟸q$).
    - Esempio: "Per avere un diploma, bisogna aver frequentato l'ultimo anno di scuola".
- **Necessaria e sufficiente**: p è vero se e solo se q è vero ( $p\↔q$ ).
    - Esempio: "Se una persona non è sposata, allora è celibe".

#### Proposizioni Aperte e Predicati

- **Proposizione aperta**: Contiene variabili, il cui valore di verità dipende dal valore assegnato.
    - Esempio: "A<4 AND (C=3 OR B>0)".
- **Quantificatori**: Usati per chiudere un predicato.
    - **Universale (∀)**: "Per ogni" (es. "∀x, x è un triangolo").
    - **Esistenziale (∃)**: "Esiste almeno uno" (es. "∃x, x è un triangolo").
    - **Esistenziale unico (∃!)**: "Esiste uno e un solo" (es. "∃! x, x è un triangolo").
- **Negazione dei quantificatori**:
    - Es. "Non tutti i cani sono bianchi" ⇔ "Esiste almeno un cane che non è bianco".

### Differenza tra Implicazione Materiale e Implicazione Logica

**Implicazione Materiale (p -> q)**:

- Non esprime una relazione di causa-effetto, ma si basa sui valori di verità. È falsa solo se p è vera e q è falsa. 

- **NON** esprime una relazione di causa - effetto 
- **NON** esprime un legame semantico tra l’antecedente e il conseguente
- È falsa solo quando p è vera e q è falsa.
- Si basa esclusivamente sui valori di verità delle proposizioni senza considerare il contenuto.

**Implicazione Logica (p ⇒ q)**:

- Esprime un legame semantico tra p e q. q è una conseguenza necessaria di p.

- **NON** è un connettivo ma simboleggia una deduzione, un ragionamento.
- Esprime un legame semantico tra l’antecedente e il conseguente
- Richiede che vi sia una connessione logica tra p e q, cioè che q sia una conseguenza necessaria di p.