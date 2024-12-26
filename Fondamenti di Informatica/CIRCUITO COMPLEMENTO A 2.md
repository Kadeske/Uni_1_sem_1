E' spesso chiesto all'esamesss.
Chiede di riconoscerlo ma non l'ho mai trovato nelle slide, che grande pugli.

Questo è ciò che ho trovato tra gli esami svolti:
![[Pasted image 20241226220746.png]]



#### Spiegazione rubata da: https://www.edutecnica.it/sistemi/sommatori/sommatori.htm

Questa spiegazione parla di un circuito generale di complemento a 2, per pugli non è necessario ma è utile per capire. 


Abbiamo [precedentemente](https://www.edutecnica.it/sistemi/aritm/aritm.htm#c2) detto che solitamente nei sistemi digitali i numeri interi relativi vengono rappresentati con il metodo del complemento a 2, utilizzando il bit più pesante come bit di segno:  
- 0=numero positivo  
- 1=numero negativo  
quindi in un sistema a 4 bit avremo le seguenti eventualità:

![[Pasted image 20241226223733.png]]

I circuiti sommatori sono indispensabili anche in questo caso. Il circuito disegnato sotto ci permette di eseguire il complemento a 2 di un numero a 4 bit.  
- Se il terminale $A_{0}=1$ si ha la complementazione a 2 dei bit in ingresso X che saranno rappresentati dai bit Y in uscita ; 
- se $A_{0}=0$ il numero rimane invariato($X_{3}X_{2}X_{1}X_{0}=Y_{3}Y_{2}Y_{1}Y_{0}$).

![[Pasted image 20241226223935.png]]

Supponiamo infatti di voler complementare il numero +5=0101, dopo aver posto $A_{0}=1$ ecco cosa accade

![[Pasted image 20241226223959.png]]

infatti 1011=-5. 

Se teniamo conto che nel sistema binario con rappresentazione a complemento a 2, la **differenza** tra due numeri positivi avviene complementando a 2 il sottraendo e poi sommando quest'ultimo valore al minuendo.  

Il dispositivo precedente può anche essere facilmente usato per ricavare il modulo (*invertire il complemento a 2*) del numero in ingresso, se infatti siamo in presenza di un numero negativo il bit $X_{3}$ può pilotare l'ingresso di complementazione $A_{0}$. Supponiamo, infatti di voler calcolare il modulo di $1101_{C_{2}}$ (*in complemento a 2*) basterà porre $X_{3}=A_{0}$.

![[Pasted image 20241226224520.png]]Infatti $1101_{C_{2}}=-3$ con $|-3|=3=0011_{C_{2}}$.





Quindi è un full adder, con una differenza:
- Le entrate sono in XOR tra il bit da complementare e 1, ovvero l'input del primo pin.


