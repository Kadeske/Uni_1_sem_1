### **Esempio 1**

#### **1. Tabella degli stati successivi**

|x1x2x_1x_2|yy|Stato attuale (yy)|Stato successivo (ynext $y_{next}$)|
|---|---|---|---|
|00|0|0|1|
|01|0|1|0|
|11|1|1|0|
|10|1|0|1|

**Motivazione**:  
La tabella degli stati successivi è essenziale per capire come il circuito sequenziale si comporta in base ai suoi ingressi ($x_1$, $x_2$) e allo stato corrente ($y$).  
Ogni riga rappresenta una possibile combinazione degli ingressi e dello stato corrente, mostrando come il circuito deve evolversi.

---

#### **2. Determinare i segnali SS e RR**

Per un flip-flop SR (Set-Reset):

- $S=1$: Il flip-flop deve passare allo stato "1".
- $R=1$: Il flip-flop deve passare allo stato "0".
- $S=R=0$: Nessun cambiamento di stato.
- $S=R=1$: Non permesso, stato non valido.

Ora analizziamo la tabella stato per stato:

- **Riga 1**: Se $x_1x_2=00$ e $y=0$, il prossimo stato ($y_{next}$) sarà 1. Quindi, $S=1$, $R=0$.
- **Riga 2**: Se $x_1x_2=01$ e $y=1$, il prossimo stato sarà 0. Quindi, $S=0$, $R=1$.
- **Riga 3**: Se $x_1x_2=11$ e $y=1$, il prossimo stato sarà 0. Quindi, $S=0$, $R=1$.
- **Riga 4**: Se $x_1x_2=10$ e $y=0$, il prossimo stato sarà 1. Quindi, $S=1$, $R=0$.

Tabella aggiornata:

|x1x2x_1x_2|yy|$y_{next}$|SS|RR|
|---|---|---|---|---|
|00|0|1|1|0|
|01|1|0|0|1|
|11|1|0|0|1|
|10|0|1|1|0|

**Motivazione**:  
Definiamo SS e RR perché controllano il comportamento del flip-flop. Analizzando lo stato attuale ($y$) e quello successivo ($y_{next}$), possiamo decidere quando settare ($S=1$) o resettare ($R=1$) il flip-flop.

---

#### **3. Derivare le funzioni logiche per SS e RR**

Costruiamo le funzioni logiche per SS e RR in base alla tabella:

- **Per SS** (quando il flip-flop passa allo stato "1"):  
    Le righe 1 e 4 hanno $S=1$. Per queste righe, osserviamo che:
    
    - Riga 1: $x_1=0$, $x_2=0$, $y=0$.
    - Riga 4: $x_1=1$, $x_2=0$, $y=0$.  
        La funzione per SS è:
    
    $S = \overline{x_1}x_2 + x_1\overline{x_2}\overline{y}$.
- **Per RR** (quando il flip-flop passa allo stato "0"):  
    Le righe 2 e 3 hanno $R=1$. Per queste righe, osserviamo che:
    
    - Riga 2: $x_1=0$, $x_2=1$, $y=1$.
    - Riga 3: $x_1=1$, $x_2=1$, $y=1$.  
        La funzione per RR è:
    
    $R = x_1x_2y + \overline{x_1}\overline{x_2}y$.

**Motivazione**:  
Derivare queste funzioni logiche consente di costruire il circuito combinatorio che calcola SS e RR in base agli ingressi ($x_1$, $x_2$) e allo stato corrente ($y$).

---

#### **4. Disegnare il circuito**

Una volta ottenute le espressioni di SS e RR, possiamo costruire il circuito logico:

- **Per SS**:
    
    - Usare AND gates per calcolare $\overline{x_1}x_2$ e $x_1\overline{x_2}\overline{y}$.
    - Usare un OR gate per sommare i risultati.
- **Per RR**:
    
    - Usare AND gates per calcolare $x_1x_2y$ e $\overline{x_1}\overline{x_2}y$.
    - Usare un OR gate per sommare i risultati.

Infine, collegare le uscite di SS e RR al flip-flop SR.

**Motivazione**:  
Costruire il circuito finale completa il processo, traducendo le funzioni logiche in componenti fisici o simulabili.

Procediamo con altri due esempi sul **sesto esercizio**, seguendo la stessa struttura passo-passo e generando alla fine lo schema logico per ognuno.

---

### **Esempio 2**

#### **1. Tabella degli stati successivi**

|x1x2x_1x_2|yy|Stato attuale (yy)|Stato successivo (ynext $y_{next}$)|
|---|---|---|---|
|00|0|0|0|
|01|0|1|1|
|11|1|1|0|
|10|1|1|1|

**Motivazione**:  
La tabella ci permette di descrivere le transizioni degli stati in base agli ingressi.

#### **2. Determinare i segnali SS e RR**

Basandoci sulla tabella, determinare SS (Set) e RR (Reset):

|x1x2x_1x_2|yy|$y_{next}$|SS|RR|
|---|---|---|---|---|
|00|0|0|0|0|
|01|0|1|1|0|
|11|1|0|0|1|
|10|1|1|0|0|

**Spiegazione**:

- Riga 1 ($x_1x_2=00$, $y=0$): Nessun cambiamento di stato, quindi $S=0$ e $R=0$.
- Riga 2 ($x_1x_2=01$, $y=0$): Lo stato passa da 0 a 1, quindi $S=1$, $R=0$.
- Riga 3 ($x_1x_2=11$, $y=1$): Lo stato passa da 1 a 0, quindi $S=0$, $R=1$.
- Riga 4 ($x_1x_2=10$, $y=1$): Nessun cambiamento di stato, quindi $S=0$ e $R=0$.

---

#### **3. Derivare le funzioni logiche per SS e RR**

- **Per SS** (quando il flip-flop passa a 1):  
    Le righe con $S=1$ sono quelle in cui $x_1x_2=01$ e $y=0$.  
    La funzione logica è:
    
    $S = \overline{x_1}x_2\overline{y}$.
- **Per RR** (quando il flip-flop passa a 0):  
    Le righe con $R=1$ sono quelle in cui $x_1x_2=11$ e $y=1$.  
    La funzione logica è:
    
    $R = x_1x_2y$.

---

#### **4. Disegnare il circuito**

Con $S = \overline{x_1}x_2\overline{y}$ e $R = x_1x_2y$:

1. Calcoliamo SS utilizzando:
    - Un AND gate per $\overline{x_1}x_2$.
    - Un AND gate per combinare il risultato con $\overline{y}$.
2. Calcoliamo RR utilizzando un AND gate per $x_1x_2y$.
3. Connettiamo SS e RR al flip-flop SR.

---
### **Esempio 3**

#### **1. Tabella degli stati successivi**

| x1x2x₁x₂ | yy | Stato attuale (yy) | Stato successivo (yₙₑₓₜ) |
|----------|----|--------------------|----------------------------|
| 00       | 0  | 0                  | 1                          |
| 01       | 1  | 1                  | 0                          |
| 11       | 0  | 0                  | 1                          |
| 10       | 1  | 1                  | 1                          |

**Motivazione**:  
Questa tabella descrive un comportamento leggermente più complesso in cui gli ingressi determinano variazioni tra stati "1" e "0", o mantengono il valore corrente.

---

#### **2. Determinare i segnali SS e RR**

| x1x2x₁x₂ | yy | yₙₑₓₜ | SS  | RR  |
|----------|----|--------|-----|-----|
| 00       | 0  | 1      | 1   | 0   |
| 01       | 1  | 0      | 0   | 1   |
| 11       | 0  | 1      | 1   | 0   |
| 10       | 1  | 1      | 0   | 0   |

**Spiegazione**:

- **Riga 1** ($x_1x_2 = 00$, $y = 0$): Passa da 0 → 1, quindi $S = 1$, $R = 0$.
- **Riga 2** ($x_1x_2 = 01$, $y = 1$): Passa da 1 → 0, quindi $S = 0$, $R = 1$.
- **Riga 3** ($x_1x_2 = 11$, $y = 0$): Passa da 0 → 1, quindi $S = 1$, $R = 0$.
- **Riga 4** ($x_1x_2 = 10$, $y = 1$): Nessun cambiamento, quindi $S = 0$, $R = 0$.

---

#### **3. Derivare le funzioni logiche per SS e RR**

- **Per SS**: Le righe con $S = 1$ sono quelle in cui:

    - **Riga 1**: $x_1x_2 = 00$, $y = 0$.
    - **Riga 3**: $x_1x_2 = 11$, $y = 0$.  
      La funzione logica per $S$ è:
    
    $$ S = \overline{x_1} \overline{x_2} \overline{y} + x_1 x_2 \overline{y}. $$

- **Per RR**: Le righe con $R = 1$ sono quelle in cui:

    - **Riga 2**: $x_1x_2 = 01$, $y = 1$.  
      La funzione logica per $R$ è:
    
    $$ R = \overline{x_1} x_2 y. $$

---

#### **4. Disegnare il circuito**

Con le funzioni:

$$ S = \overline{x_1} \overline{x_2} \overline{y} + x_1 x_2 \overline{y} $$
$$ R = \overline{x_1} x_2 y $$

1. **Per SS**:
    - Un AND gate per calcolare $\overline{x_1} \overline{x_2} \overline{y}$.
    - Un AND gate per calcolare $x_1 x_2 \overline{y}$.
    - Un OR gate per combinare i risultati.

2. **Per RR**:
    - Un AND gate per calcolare $\overline{x_1} x_2 y$.

3. Connettiamo le uscite SS e RR al flip-flop SR.

---

