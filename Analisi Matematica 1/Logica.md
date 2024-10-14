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

|**p**|**i** (Identità)|**¬p** (Negazione)|
|---|---|---|
|VERO|VERO|FALSO|
|FALSO|FALSO|VERO|

**Esempio:**

- **Identità**: se $p=VEROp = \text{VERO}p=VERO, allora i(p)=VEROi(p) = \text{VERO}i(p)=VERO$.
    - _Giusto_: "La Terra è un pianeta" → è vera e resta vera con l'identità.
    - _Sbagliato_: "La Terra è piatta" → è falsa e non diventa vera con l'identità.
- **Negazione**: se p=VEROp = \text{VERO}p=VERO, allora ¬p=FALSO¬p = \text{FALSO}¬p=FALSO.
    - _Giusto_: "Non è vero che 2 + 2 = 5" → correttamente negato.
    - _Sbagliato_: "Non è vero che 2 + 2 = 4" → errato, perché nega una verità.

---

## Connettivi binari

### Tabella dei connettivi binari

|**p**|**q**|**p ∧ q** (AND)|**p ∨ q** (OR)|**p ⇒ q** (Implica)|**p ⇔ q** (Equivalente)|**p ⊕ q** (XOR)|
|---|---|---|---|---|---|---|
|VERO|VERO|VERO|VERO|VERO|VERO|FALSO|
|VERO|FALSO|FALSO|VERO|FALSO|FALSO|VERO|
|FALSO|VERO|FALSO|VERO|VERO|FALSO|VERO|
|FALSO|FALSO|FALSO|FALSO|VERO|VERO|FALSO|

### Esempi per ciascun connettivo

1. **Congiunzione (AND, ∧)**:
    
    - p∧qp ∧ qp∧q è vero solo se entrambi ppp e qqq sono veri.
    - _Giusto_: "Piove **e** fa freddo" → entrambe le condizioni sono vere.
    - _Sbagliato_: "Piove **e** c'è il sole" → falsa perché una delle condizioni è falsa.
2. **Disgiunzione (OR, ∨)**:
    
    - p∨qp ∨ qp∨q è vero se almeno uno tra ppp e qqq è vero.
    - _Giusto_: "Piove **o** fa freddo" → vero, perché fa freddo (anche se non piove).
    - _Sbagliato_: "Piove **o** nevica" → falso se entrambe le condizioni sono false.
3. **Implicazione (IF-THEN, ⇒)**:
    
    - p⇒qp ⇒ qp⇒q è falso solo se ppp è vero e qqq è falso.
    - _Giusto_: "Se studio, passo l'esame" → vero se lo studio porta al risultato.
    - _Sbagliato_: "Se studio, fallisco l'esame" → errato, se si studia non dovrebbe portare al fallimento.
4. **Equivalenza (IF AND ONLY IF, ⇔)**:
    
    - p⇔qp ⇔ qp⇔q è vero se ppp e qqq hanno lo stesso valore di verità.
    - _Giusto_: "Un numero è pari **se e solo se** è divisibile per 2".
    - _Sbagliato_: "Un numero è pari **se e solo se** è dispari" → contraddittorio.
5. **Disgiunzione esclusiva (XOR, ⊕)**:
    
    - p⊕qp ⊕ qp⊕q è vero solo se uno tra ppp e qqq è vero, ma non entrambi.
    - _Giusto_: "Oggi vado al mare **o** in montagna" → vero se faccio una sola delle due cose.
    - _Sbagliato_: "Vado al mare **o** vado al mare" → falsa perché entrambe le scelte sono la stessa.