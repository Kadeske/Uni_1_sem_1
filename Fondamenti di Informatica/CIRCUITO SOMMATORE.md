
I circuiti sommatori fanno parte della categoria dei circuiti combinatori (grazie al ca).

## Half Adder
Permette di fare la somma logica di 2 bit.
Dato che la somma logica è un OR logico, perchè usare questo circuito?
Il circuito half adder tiene conto del riporto durante l'operazione.

Per capire:

#### Tabella di verità OR logico

| Ingresso A | Ingresso B | risultato |
| ---------- | ---------- | --------- |
| 0          | 0          | 0         |
| 0          | 1          | 1         |
| 1          | 0          | 1         |
| 1          | 1          | 1         |

#### Tabella di verità Half Adder

| Ingresso A | Ingresso B | Somma | Resto |
| ---------- | ---------- | ----- | ----- |
| 0          | 0          | 0     | 0     |
| 0          | 1          | 1     | 0     |
| 1          | 0          | 1     | 0     |
| 1          | 1          | 0     | 1     |

E' leggermente diverso.

Questo è la rete logica dell'Half adder:

![[Pasted image 20241226212939.png]]




## Full Adder

Il problema dell'Half Adder è che il resto viene "buttato", cioè viene generato ma non serve a nulla da solo (è un orfano, inutile).
Per ottenere un circuito che effettui la somma di bit tenendo conto del riporto è necessario unire più half adder a cascata (ora è una catena di montaggio di orfani, tipo shein).

#### Tabella di verità

![[Pasted image 20241226213402.png]]


#### Circuito logico
E' l'interno della scatoletta riportata sopra (al fianco della tabella di verità).

![[Pasted image 20241226213430.png]]

Dato che a Puglisi san piace incasinare non ha inserito il circuito completo in chiaro, che spesso chiede di riconoscere all'esame.
QUUUINDI geeks for geeks (https://www.geeksforgeeks.org/implementation-of-full-adder-using-half-adders/):

![[Pasted image 20241226214021.png]]



### ESEMPI SGRAVATI 
All'esame pugli san potrebbe fornire un circuito sgravo brutto molto per fregarti chiedendoti di capire se è un full adder.

I passi da seguire sono:
- Trovare le espressioni logiche del circuito sgravo.
- Semplificare le espressioni per capirci qualcosa
- SOLO SE le espressioni trovate sono: 
	- S = A ⊕ B ⊕ Cin      (Cin è il riporto in entrata, pensa di avere due half adder, cin è il bit che segna il riport in entrata al secondo half adder)
	- Cout = AB + ACin + BCin     (Cout è il riporto, pugli lo solitamente lo segna con R, è uguale)

#### Esempio rubato dal 2016 
![[Pasted image 20241226215216.png]]

Attenzione ai nomi che da pugli, adattandolo ai nomi di prima:
- X1 = a
- X2 = b
- X3 = Cin (Il resto in entrata)
- Z1 = S
- Z2 = Cout (o R, ovvero resto in uscita)


#### ESEMPIO BALLLLLORDO 2, dove NON è un full adder

![[Pasted image 20241226215501.png]]

In questo caso Z1, ovvero la somma, è corretto, ma Z2, ovvero il resto, è sbagliato.

Se non si nota la differenza, la porta in uscita da Z2 nel caso corretto è una OR, mentre nel caso errato è una AND.
Pugli fa i trick cattivi.

## Sommatore di n bit
Non l'ha mai chiesto ma non si sa mai.

E' un circuito in grado di calcolare la somma di n bit, ovvero la somma di un numero di bit indefinito.

E' un serie di Full Adder a cascata, dove il resto in uscita di uno va nel resto in ingresso del successivo. (Come in un centipede umano)

#### Circuito logico
![[Pasted image 20241226220152.png]]

