# Unioni e enumerazioni

Le unioni e le enumerazioni sono due costrutti fondamentali nel linguaggio di programmazione C che consentono di gestire in modo efficiente e organizzato dati di diversi tipi.

## Unioni

Le unioni permettono di definire una struttura dati in cui diversi tipi di variabili condividono lo stesso spazio di memoria. Questo significa che una variabile di tipo union può essere utilizzata per memorizzare dati di diversi tipi, ma solo uno alla volta. Quando si assegna un valore a una variabile di tipo union, il valore sovrascrive quello precedente.

La dichiarazione di una union avviene nel seguente modo:

```c
union nome_union {
    tipo1 variabile1;
    tipo2 variabile2;
    ...
};
```

Per accedere ai membri di una union si utilizza l'operatore `.` seguito dal nome del membro. È importante notare che, a differenza delle struct, i membri di una union condividono lo stesso spazio di memoria e quindi la dimensione totale della union corrisponde alla dimensione del membro più grande.

Le unioni sono particolarmente utili quando si ha la necessità di gestire dati di diversi tipi in modo efficiente, ad esempio durante la lettura di dati da un file o durante la comunicazione con dispositivi esterni.

## Enumerazioni

Le enumerazioni permettono di definire un nuovo tipo di dato composto da un insieme di costanti intere. Ogni costante all'interno di un'enumerazione ha un valore intero associato che di default parte da 0 e viene incrementato di uno per ogni costante definita.

La dichiarazione di un'enumerazione avviene nel seguente modo:

```c
enum nome_enum {
    costante1,
    costante2,
    ...
};
```

È possibile specificare il valore associato a ciascuna costante all'interno dell'enumerazione:

```c
enum giorni_settimana {
    lunedi = 1,
    martedi,
    mercoledi,
    giovedi,
    venerdi,
    sabato,
    domenica
};
```

Per accedere alle costanti di un'enumerazione si utilizza il nome dell'enumerazione seguito dalla costante desiderata.

Le enumerazioni sono particolarmente utili quando si ha la necessità di gestire un insieme limitato di costanti che rappresentano uno stato o una scelta specifica all'interno del programma.

In conclusione, unioni e enumerazioni sono due costrutti essenziali nel linguaggio di programmazione C che consentono di gestire dati di diversi tipi in modo efficiente e organizzato. La loro corretta utilizzo contribuisce a migliorare la leggibilità e la manutenibilità del codice.