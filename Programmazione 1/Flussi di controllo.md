---
~
---


### Modello concorrente

Esegue più alternative (programmi) contemporaneamente, quindi ha più flussi di controllo contemporaneamente.
Alla fine, i flussi si riuniscono in uno solo.

Fork -> dividi in più flussi
Join -> Unisci più flussi in uno

``` mermaid
stateDiagram-v2
    INIZIO --> flusso1
    INIZIO --> flusso2
    INIZIO --> flusso3
    INIZIO --> flusso4
    flusso1 --> FINE
    flusso2 --> FINE
    flusso3 --> FINE
    flusso4 --> FINE
```

### Modello non deterministico

Il suo funzionamento è determinato da fattori non controllabili dal programmatore, per esempio un telefono può fare diverse cose, ma non è stato direttamente programmato per risolvere un problema ad una certa ora di un determinato giorno, è l'utente che lo utilizza in questo modo.

#### Event-driven
Computazione tramite l'interfaccia uomo-macchina

