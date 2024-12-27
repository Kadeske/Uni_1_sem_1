### **Esempio 1**  
**Espressioni**:  
$f_1(x_1, x_2, x_3) = x_1x_2 + x_1x_3$  
$f_2(x_1, x_2, x_3) = x_1(x_2 + x_3)$  

#### **Risoluzione**:
1. **Verifica mediante distribuzione**:  
   Espandiamo $f_2$ usando la proprietà distributiva:  
   $f_2 = x_1(x_2 + x_3) = x_1x_2 + x_1x_3.$  
   Ora $f_2 = x_1x_2 + x_1x_3$, che è esattamente $f_1$.

2. **Conclusione**:  
   Le espressioni $f_1$ e $f_2$ sono **equivalenti**.

---

### **Esempio 2**  
**Espressioni**:  
$f_1(x_1, x_2, x_3) = x_1x_2 + \overline{x_1}x_3$  
$f_2(x_1, x_2, x_3) = (x_1 + x_3)(x_2 + x_3)$  

#### **Risoluzione**:
1. **Espansione di $f_2$**:  
   Usiamo la distribuzione per espandere $f_2$:  
   $f_2 = (x_1 + x_3)(x_2 + x_3) = x_1x_2 + x_1x_3 + x_3x_2 + x_3.$  

2. **Riduzione di $f_2$**:  
   Usiamo le proprietà di assorbimento e commutatività:  
   - $x_1x_3 + x_3$ si semplifica in $x_3$ (assorbimento).  
   - Quindi:  
     $f_2 = x_1x_2 + x_3.$  

3. **Confronto tra $f_1$ e $f_2$**:  
   $f_1 = x_1x_2 + \overline{x_1}x_3.$  
   $f_2 = x_1x_2 + x_3.$  
   Non sono uguali perché $f_2$ include un termine $x_3$ indipendente, mentre $f_1$ richiede la condizione $\overline{x_1}x_3$.

4. **Conclusione**:  
   Le espressioni $f_1$ e $f_2$ sono **non equivalenti**.

---

### **Esempio 3**  
**Espressioni**:  
$f_1(x_1, x_2, x_3) = \overline{x_1}x_2 + x_1x_3$  
$f_2(x_1, x_2, x_3) = (x_1 + x_2)(\overline{x_1} + x_3)$  

#### **Risoluzione**:
1. **Espansione di $f_2$**:  
   Usiamo la distribuzione per espandere $f_2$:  
   $f_2 = (x_1 + x_2)(\overline{x_1} + x_3).$  
   Espandiamo ogni termine:  
   $f_2 = x_1\overline{x_1} + x_1x_3 + x_2\overline{x_1} + x_2x_3.$  

2. **Semplificazione di $f_2$**:  
   - $x_1\overline{x_1} = 0$ (complemento).  
   - Quindi:  
     $f_2 = x_1x_3 + x_2\overline{x_1} + x_2x_3.$  

3. **Riduzione di $f_2$**:  
   - Il termine $x_2x_3$ è già incluso.  
   - Quindi:  
     $f_2 = x_1x_3 + x_2\overline{x_1}.$  

4. **Confronto tra $f_1$ e $f_2$**:  
   - $f_1 = \overline{x_1}x_2 + x_1x_3.$  
   - $f_2 = x_1x_3 + x_2\overline{x_1}.$  
   - Sono identiche perché l’ordine dei termini non cambia la somma.

5. **Conclusione**:  
   Le espressioni $f_1$ e $f_2$ sono **equivalenti**.
