# Rappresentazione IEEE 754 in Singola Precisione

## Esercizio 1: 111,125 in IEEE 754 (Singola Precisione)

### Passo 1: Conversione in binario
- **Parte intera** di 111:
  - $111 \div 2 = 55$ resto 1
  - $55 \div 2 = 27$ resto 1
  - $27 \div 2 = 13$ resto 1
  - $13 \div 2 = 6$ resto 1
  - $6 \div 2 = 3$ resto 0
  - $3 \div 2 = 1$ resto 1
  - $1 \div 2 = 0$ resto 1  
  Quindi, la parte intera di 111 in binario è **1101111**.

- **Parte frazionaria** di 0,125:
  - $0,125 \times 2 = 0,25$ → 0
  - $0,25 \times 2 = 0,5$ → 0
  - $0,5 \times 2 = 1,0$ → 1  
  Quindi, la parte frazionaria di 0,125 in binario è **.001**.

Quindi, $111,125$ in binario è **1101111.001**.

### Passo 2: Normalizzazione
La normalizzazione consiste nel rappresentare il numero in forma $1.x \times 2^n$, dove il punto binario è spostato dopo il primo 1.  
$ 1101111.001 $ diventa $ 1.101111001 \times 2^6 $.

### Passo 3: Calcolo dell'esponente
L'esponente va modificato con un "bias", che per il formato a singola precisione è 127.  
L'esponente nella nostra normalizzazione è 6, quindi l'esponente "biased" è:

$$
\text{Esponente biased} = 6 + 127 = 133
$$

In binario, 133 è **10000101**.

### Passo 4: Mantissa
La mantissa è composta dai bit successivi al punto binario della normalizzazione, escludendo il primo 1 che è implicito.  
Per il numero normalizzato $1.101111001$, la mantissa è **10111100100000000000000** (completando i 23 bit con zeri).

### Passo 5: Composizione del risultato finale
La rappresentazione IEEE 754 a singola precisione consiste in 32 bit:

1. **Bit di segno**: 0 (perché il numero è positivo).
2. **Esponente**: **10000101** (8 bit).
3. **Mantissa**: **10111100100000000000000** (23 bit).

Quindi, la rappresentazione finale è:

$$
0\ 10000101\ 10111100100000000000000
$$

---

## Esercizio 2: 23,75 in IEEE 754 (Singola Precisione)

### Passo 1: Conversione in binario
- **Parte intera** di 23:
  - $23 \div 2 = 11$ resto 1
  - $11 \div 2 = 5$ resto 1
  - $5 \div 2 = 2$ resto 1
  - $2 \div 2 = 1$ resto 0
  - $1 \div 2 = 0$ resto 1  
  Quindi, la parte intera di 23 in binario è **10111**.

- **Parte frazionaria** di 0,75:
  - $0,75 \times 2 = 1,5$ → 1
  - $0,5 \times 2 = 1,0$ → 1  
  Quindi, la parte frazionaria di 0,75 in binario è **.11**.

Quindi, $23,75$ in binario è **10111.11**.

### Passo 2: Normalizzazione
La normalizzazione di $10111.11$ diventa $1.011111 \times 2^4$.

### Passo 3: Calcolo dell'esponente
L'esponente nella normalizzazione è 4, quindi l'esponente "biased" è:

$$
\text{Esponente biased} = 4 + 127 = 131
$$

In binario, 131 è **10000011**.

### Passo 4: Mantissa
La mantissa è **01111100000000000000000** (23 bit).

### Passo 5: Composizione del risultato finale
La rappresentazione finale in IEEE 754 è:

1. **Bit di segno**: 0 (perché il numero è positivo).
2. **Esponente**: **10000011** (8 bit).
3. **Mantissa**: **01111100000000000000000** (23 bit).

La rappresentazione finale è:

$$
0\ 10000011\ 01111100000000000000000
$$

---

## Esercizio 3: 3,5 in IEEE 754 (Singola Precisione)

### Passo 1: Conversione in binario
- **Parte intera** di 3:
  - $3 \div 2 = 1$ resto 1
  - $1 \div 2 = 0$ resto 1  
  Quindi, la parte intera di 3 in binario è **11**.

- **Parte frazionaria** di 0,5:
  - $0,5 \times 2 = 1,0$ → 1  
  Quindi, la parte frazionaria di 0,5 in binario è **.1**.

Quindi, $3,5$ in binario è **11.1**.

### Passo 2: Normalizzazione
La normalizzazione di $11.1$ diventa $1.11 \times 2^1$.

### Passo 3: Calcolo dell'esponente
L'esponente nella normalizzazione è 1, quindi l'esponente "biased" è:

$$
\text{Esponente biased} = 1 + 127 = 128
$$

In binario, 128 è **10000000**.

### Passo 4: Mantissa
La mantissa è **11000000000000000000000** (23 bit).

### Passo 5: Composizione del risultato finale
La rappresentazione finale in IEEE 754 è:

1. **Bit di segno**: 0 (perché il numero è positivo).
2. **Esponente**: **10000000** (8 bit).
3. **Mantissa**: **11000000000000000000000** (23 bit).

La rappresentazione finale è:

$$
0\ 10000000\ 11000000000000000000000
$$

---

## Esercizio 4: 0,75 in IEEE 754 (Singola Precisione)

### Passo 1: Conversione in binario
- **Parte intera** di 0:  
  Non c'è parte intera, quindi la parte intera è **0**.

- **Parte frazionaria** di 0,75:
  - $0,75 \times 2 = 1,5$ → 1
  - $0,5 \times 2 = 1,0$ → 1  
  Quindi, la parte frazionaria di 0,75 in binario è **.11**.

Quindi, $0,75$ in binario è **0.11**.

### Passo 2: Normalizzazione
La normalizzazione di $0.11$ diventa $1.1 \times 2^{-1}$.

### Passo 3: Calcolo dell'esponente
L'esponente nella normalizzazione è -1, quindi l'esponente "biased" è:

$$
\text{Esponente biased} = -1 + 127 = 126
$$

In binario, 126 è **01111110**.

### Passo 4: Mantissa
La mantissa è **10000000000000000000000** (23 bit).

### Passo 5: Composizione del risultato finale
La rappresentazione finale in IEEE 754 è:

1. **Bit di segno**: 0 (perché il numero è positivo).
2. **Esponente**: **01111110** (8 bit).
3. **Mantissa**: **10000000000000000000000** (23 bit).

La rappresentazione finale è:

$$
0\ 01111110\ 10000000000000000000000
$$

---

## Esercizio 5: 1024,5 in IEEE 754 (Singola Precisione)

### Passo 1: Conversione in binario
- **Parte intera** di 1024:
  - $1024 \div 2 = 512$ resto 0
  - $512 \div 2 = 256$ resto 0
  - $256 \div 2 = 128$ resto 0
  - $128 \div 2 = 64$ resto 0
  - $64 \div 2 = 32$ resto 0
  - $32 \div 2 = 16$ resto 0
  - $16 \div 2 = 8$ resto 0
  - $8 \div 2 = 4$ resto 0
  - $4 \div 2 = 2$ resto 0
  - $2 \div 2 = 1$ resto 0
  - $1 \div 2 = 0$ resto 1  
  Quindi, la parte intera di 1024 in binario è **10000000000**.

- **Parte frazionaria** di 0,5:
  - $0,5 \times 2 = 1,0$ → 1  
  Quindi, la parte frazionaria di 0,5 in binario è **.1**.

Quindi, $1024,5$ in binario è **10000000000.1**.

### Passo 2: Normalizzazione
La normalizzazione di $10000000000.1$ diventa $1.0000000001 \times 2^{10}$.

### Passo 3: Calcolo dell'esponente
L'esponente nella normalizzazione è 10, quindi l'esponente "biased" è:

$$
\text{Esponente biased} = 10 + 127 = 137
$$

In binario, 137 è **10001001**.

### Passo 4: Mantissa
La mantissa è **00000000010000000000000** (23 bit).

### Passo 5: Composizione del risultato finale
La rappresentazione finale in IEEE 754 è:

1. **Bit di segno**: 0 (perché il numero è positivo).
2. **Esponente**: **10001001** (8 bit).
3. **Mantissa**: **00000000010000000000000** (23 bit).

La rappresentazione finale è:

$$
0\ 10001001\ 00000000010000000000000
$$
