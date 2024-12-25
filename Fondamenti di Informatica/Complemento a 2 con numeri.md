Ecco 3 esercizi sul **complemento a 2 e operazioni aritmetiche in binario**. Ogni esercizio include una risoluzione passo passo.

---

### **Esercizio 1**  
Rappresenta i numeri decimali $a = -25$ e $b = 15$ in complemento a 2 su una parola di 8 bit. Esegui le operazioni $a + b$ e $a - b$, indicando la presenza di eventuali overflow.

---

#### **Risoluzione passo passo**:
1. **Rappresentazione di $a$ e $b$ in complemento a 2**:  
   - $a = -25$: Convertiamo $|25| = 11001$ in binario, aggiungendo i bit per ottenere 8 bit: $00011001$.  
     Calcoliamo il complemento a 2 invertendo i bit ($11100110$) e aggiungendo 1: $11100111$.  
     Quindi, $a = 11100111$.  
   - $b = 15$: In binario è $00001111$.  

2. **Operazione $a + b$**:
   - Sommiamo:
     $$
     \begin{aligned}
     11100111 \, (a) \\
     + 00001111 \, (b) \\
     \hline
     11110110 \, \text{(risultato)} \\
     \end{aligned}
     $$
   - $11110110$ è negativo in complemento a 2. Per calcolarne il valore:  
     Invertiamo i bit ($00001001$) e sommiamo 1: $00001010$ ($|risultato| = 10$).  
     Quindi, il risultato è $-10$.  
   - Non c'è overflow: il segno resta coerente.

3. **Operazione $a - b$**:
   - Per calcolare $a - b$, sommiamo $a + (-b)$.  
     Il complemento a 2 di $b = 15$ è $11110001$.  
     Sommiamo:
     $$
     \begin{aligned}
     11100111 \, (a) \\
     + 11110001 \, (-b) \\
     \hline
     11011000 \, \text{(risultato)} \\
     \end{aligned}
     $$
   - $11011000$ è negativo. Invertiamo i bit ($00100111$) e sommiamo 1: $00101000$ ($|risultato| = 40$).  
     Quindi, il risultato è $-40$.  
   - Non c'è overflow.

---

### **Esercizio 2**  
Rappresenta i numeri $a = -58$ e $b = 22$ in complemento a 2 su una parola di 8 bit. Esegui le operazioni $a + b$ e $a - b$, specificando eventuali overflow.

---

#### **Risoluzione passo passo**:
1. **Rappresentazione di $a$ e $b$**:  
   - $a = -58$: Convertiamo $|58| = 111010$ in binario, aggiungendo i bit: $00111010$.  
     Complemento a 2: invertiamo i bit ($11000101$) e sommiamo 1: $11000110$.  
     Quindi, $a = 11000110$.  
   - $b = 22$: In binario è $00010110$.  

2. **Operazione $a + b$**:
   - Sommiamo:
     $$
     \begin{aligned}
     11000110 \, (a) \\
     + 00010110 \, (b) \\
     \hline
     11011100 \, \text{(risultato)} \\
     \end{aligned}
     $$
   - $11011100$ è negativo. Invertiamo i bit ($00100011$) e sommiamo 1: $00100100$ ($|risultato| = 36$).  
     Quindi, il risultato è $-36$.  
   - Non c'è overflow.

3. **Operazione $a - b$**:
   - $a - b = a + (-b)$. Il complemento a 2 di $b = 22$ è $11101010$.  
     Sommiamo:
     $$
     \begin{aligned}
     11000110 \, (a) \\
     + 11101010 \, (-b) \\
     \hline
     10110000 \, \text{(risultato)} \\
     \end{aligned}
     $$
   - $10110000$ è negativo. Invertiamo i bit ($01001111$) e sommiamo 1: $01010000$ ($|risultato| = 80$).  
     Quindi, il risultato è $-80$.  
   - Non c'è overflow.

---

### **Esercizio 3**  
Rappresenta i numeri $a = -19$ e $b = 9$ in complemento a 2 su una parola di 8 bit. Esegui le operazioni $a + b$ e $a - b$, specificando eventuali overflow.

---

#### **Risoluzione passo passo**:
1. **Rappresentazione di $a$ e $b$**:  
   - $a = -19$: Convertiamo $|19| = 10011$ in binario, aggiungendo i bit: $00010011$.  
     Complemento a 2: invertiamo i bit ($11101100$) e sommiamo 1: $11101101$.  
     Quindi, $a = 11101101$.  
   - $b = 9$: In binario è $00001001$.  

2. **Operazione $a + b$**:
   - Sommiamo:
     $$
     \begin{aligned}
     11101101 \, (a) \\
     + 00001001 \, (b) \\
     \hline
     11110110 \, \text{(risultato)} \\
     \end{aligned}
     $$
   - $11110110$ è negativo. Invertiamo i bit ($00001001$) e sommiamo 1: $00001010$ ($|risultato| = 10$).  
     Quindi, il risultato è $-10$.  
   - Non c'è overflow.

3. **Operazione $a - b$**:
   - $a - b = a + (-b)$. Il complemento a 2 di $b = 9$ è $11110111$.  
     Sommiamo:
     $$
     \begin{aligned}
     11101101 \, (a) \\
     + 11110111 \, (-b) \\
     \hline
     11011100 \, \text{(risultato)} \\
     \end{aligned}
     $$
   - $11011100$ è negativo. Invertiamo i bit ($00100011$) e sommiamo 1: $00100100$ ($|risultato| = 36$).  
     Quindi, il risultato è $-36$.  
   - Non c'è overflow.

---

## Esempio con overflow

### **Esercizio: Calcolo con overflow**  
Rappresenta i numeri $a = 70$ e $b = 80$ in complemento a 2 su una parola di 8 bit. Calcola $a + b$ e verifica la presenza di overflow.

---

#### **Risoluzione passo passo**:
1. **Rappresentazione di $a$ e $b$ in complemento a 2**:  
   - $a = 70$: Convertiamo $70$ in binario su 8 bit:  
     $$
     70 = 1000110 \ \ (\text{7 bit, aggiungiamo uno 0 iniziale: } 01000110).
     $$  
     Quindi, $a = 01000110$.  
   - $b = 80$: Convertiamo $80$ in binario su 8 bit:  
     $$
     80 = 1010000 \ \ (\text{7 bit, aggiungiamo uno 0 iniziale: } 01010000).
     $$  
     Quindi, $b = 01010000$.  

2. **Operazione $a + b$**:  
   Sommiamo i due numeri in binario:
   $$
   \begin{aligned}
   01000110 \, (a) \\
   + 01010000 \, (b) \\
   \hline
   10010110 \, \text{(risultato)} \\
   \end{aligned}
   $$
   Il risultato è $10010110$.

3. **Interpretazione del risultato**:
   - Il risultato $10010110$ è in complemento a 2 e rappresenta un numero **negativo** (il bit più significativo, $MSB = 1$, indica un numero negativo).  
   - Per verificare il valore: invertiamo i bit ($01101001$) e sommiamo 1:  
     $$
     01101001 + 1 = 01101010 = 106.
     $$
     Quindi, il risultato è $-106$.

4. **Verifica dell’overflow**:  
   - In binario con complemento a 2 su 8 bit, i numeri rappresentabili vanno da $-128$ a $+127$.  
   - Qui, stiamo sommando due numeri **positivi** ($a = 70$ e $b = 80$), quindi ci aspettiamo un risultato positivo. Tuttavia, il risultato è negativo ($-106$), il che non ha senso!  
   - Questo è un caso di **overflow** perché la somma ($70 + 80 = 150$) eccede il massimo rappresentabile ($127$).  

5. **Come riconoscere l’overflow**:  
   - L’overflow si verifica se:
     - Entrambi gli operandi hanno lo stesso segno (positivi o negativi).
     - Il risultato ha un segno opposto rispetto agli operandi.  
   - In questo caso, sia $a$ che $b$ sono positivi ($MSB = 0$), ma il risultato è negativo ($MSB = 1$).  
   **Conclusione**: **C’è overflow.**

---

Quindi la somma $a + b$ produce $-106$, ma questo risultato non è valido a causa dell’overflow. In realtà, la somma $70 + 80 = 150$ non può essere rappresentata correttamente con 8 bit in complemento a 2.

