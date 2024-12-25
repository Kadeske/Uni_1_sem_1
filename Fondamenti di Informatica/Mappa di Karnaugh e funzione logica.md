Ecco 3 esercizi sul tema **mappa di Karnaugh e funzione logica**. Ogni esercizio include una spiegazione dettagliata della risoluzione.

---

### **Esercizio 1**  
Dati i seguenti minterm di una funzione booleana $f(x_1, x_2, x_3, x_4)$, rappresenta la funzione sulla mappa di Karnaugh e trova l'espressione minima.  
Minterm: $f(x_1, x_2, x_3, x_4) = \Sigma(0, 2, 6, 8, 10, 14)$.

#### **Risoluzione passo passo**:
1. **Rappresentazione sulla mappa di Karnaugh**  
   Riportiamo i minterm $0, 2, 6, 8, 10, 14$ nella mappa:
   - Indichiamo l’asse $x_1x_2$ e $x_3x_4$ rispettivamente con le combinazioni (00, 01, 11, 10).
   - Posizioniamo un $1$ nei rispettivi riquadri dei minterm.  

   La mappa sarà:


| $x_1x_2 / x_3x_4$ | 00  | 01  | 11  | 10  |
| ----------------- | --- | --- | --- | --- |
| 00                | 1   | 0   | 0   | 1   |
| 01                | 1   | 0   | 0   | 0   |
| 11                | 0   | 0   | 0   | 1   |
| 10                | 0   | 1   | 1   | 0   |
|                   |     |     |     |     |
|                   |     |     |     |     |



2. **Individuazione dei gruppi**  
- Gruppo da 2 (colonna 00): $x_1'x_2'$.
- Gruppo da 2 (riga 10, colonne 01 e 11): $x_1x_2x_3$.
- Singolo minterm $x_1'x_2'x_3x_4$.  

3. **Espressione finale**  
La funzione minima è:
$$
f(x_1, x_2, x_3, x_4) = x_1'x_2' + x_1x_2x_3 + x_1'x_2'x_3x_4
$$

---

### **Esercizio 2**  
La mappa di Karnaugh di una funzione logica $f(x_1, x_2, x_3)$ è data di seguito. Determina la funzione minima.  



| $x_1x_2 / x_3$ | 0   | 1   |
| -------------- | --- | --- |
| 00             | 1   | 0   |
| 01             | 1   | 1   |
| 11             | 0   | 1   |
| 10             | 1   | 0   |



#### **Risoluzione passo passo**:
1. **Raggruppamenti**  
   - Gruppo da 2 nella colonna $x_3 = 0$: $x_1'x_3'$.
   - Singolo $x_1'x_2x_3$ (seconda riga).
   - Singolo $x_1x_2'x_3'$ (ultima riga).

2. **Espressione minima**  
   La funzione minima è:
   $$
   f(x_1, x_2, x_3) = x_1'x_3' + x_1'x_2x_3 + x_1x_2'x_3'
   $$

---

### **Esercizio 3**  
Costruisci la mappa di Karnaugh e trova l'espressione minima di una funzione con minterm $\Sigma(1, 3, 7, 9, 11)$ in $f(x_1, x_2, x_3, x_4)$.

#### **Risoluzione passo passo**:
1. **Costruzione della mappa**  
   Inseriamo i minterm dati:


| $x_1x_2 / x_3x_4$ | 00  | 01  | 11  | 10  |
| ----------------- | --- | --- | --- | --- |
| 00                | 0   | 1   | 0   | 1   |
| 01                | 0   | 0   | 1   | 0   |
| 11                | 0   | 0   | 1   | 0   |
| 10                | 0   | 0   | 0   | 0   |



2. **Individuazione dei gruppi**  
- Gruppo singolo $1$ (colonna $01$, riga 00): $x_1'x_2'x_3x_4'$.
- Gruppo da 2: $x_1x_2'x_3x_4$.
- Gruppo da 2: $x_1x_2x_3$.

3. **Espressione finale**  
$$
f(x_1, x_2, x_3, x_4) = x_1'x_2'x_3x_4' + x_1x_2'x_3x_4 + x_1x_2x_3
$$
