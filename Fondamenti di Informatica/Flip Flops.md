Un flip flop è un circuito sequenziale che si comporta come un elemento di memoria, ovvero è in grado di contenere un bit di informazione.


#### Funzioni di eccitazione del flip flop
La funzione di eccitazione di un flip-flop indica quali ingressi applicare al flip-flop per ottenere una specifica transizione di stato desiderata. In altre parole, determina come manipolare gli ingressi del flip-flop per forzare il passaggio da uno stato all'altro.

#### Funzione di transizione
Questa funzione descrive lo stato futuro del flip-flop in base allo stato presente e agli ingressi


Esistono diversi tipi di flip flop. Si differenziano per il loro circuito logico e conseguente tabella di verità ma hanno lo stesso compito e funzionamento base.

- Flip-flop SR (FF-**SR**)
- Flip-flop JK (FF-**JK**)
- Delay flip-flop (FF-**D**)
- Trigger flip-flop (FF-**T**)


Pugli non chiede D e T all'esame perchè "troppo semplici".
Nella maggior parte delle prove ha chiesto la tipologia SR, ma capita anche JK



# Flip-Flop SR

## Funzione di Transizione
La funzione di transizione per il flip-flop SR è:
$\ Q(t+1) = S + \overline{R} \cdot Q(t)$

## Tabella della Funzione di Transizione
![[Pasted image 20250104145716.png]]
## Funzione di Eccitazione
Le funzioni di eccitazione per il flip-flop SR sono:
- $S = Q'(t) \cdot Q(t+1)$
- $R = Q(t) \cdot Q'(t+1)$ 


## Schema Logico
(esistono diverse rappresentazioni, questa con porte NOR)
Il flip-flop SR può essere implementato con due porte **NOR**:

![[Pasted image 20250103154534.png]]


---

# Flip-Flop JK

## Funzione di Transizione
La funzione di transizione per il flip-flop JK è:
$$ Q(t+1) = J \cdot \overline{Q(t)} + \overline{K} \cdot Q(t) $$

## Tabella della Funzione di Transizione
| $ J $ | $ K $ | $ Q(t) $ | $ Q(t+1) $ | Descrizione          |
|-------|-------|----------|------------|----------------------|
| 0     | 0     | 0        | 0          | Nessun cambiamento   |
| 0     | 0     | 1        | 1          | Nessun cambiamento   |
| 0     | 1     | X        | 0          | Reset                |
| 1     | 0     | X        | 1          | Set                  |
| 1     | 1     | 0        | 1          | Toggle               |
| 1     | 1     | 1        | 0          | Toggle               |

## Funzione di Eccitazione
Le funzioni di eccitazione per il flip-flop JK sono:
- $J = Q'(t) \cdot Q(t+1)$
- $K = Q(t) \cdot Q'(t+1)$

## Tabella della Funzione di Eccitazione
|  Q(t)  | Q(t+1) | J   | K   |
| ------ | ------ | --- | --- |
| 0      | 0      | 0   | 0   |
| 0      | 1      | 1   | 0   |
| 1      | 0      | 0   | 1   |
| 1      | 1      | 1   | 0   |

## Schema Logico
Il flip-flop JK può essere implementato con porte logiche come segue:

![[Pasted image 20250103154759.png]]