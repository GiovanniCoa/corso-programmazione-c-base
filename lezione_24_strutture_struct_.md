# Strutture (struct)

Le strutture (struct) sono un tipo di dato composto in linguaggi di programmazione che consentono di raggruppare diverse variabili correlate sotto un'unica entità. Le strutture permettono di definire nuovi tipi di dati personalizzati, facilitando la gestione e l'organizzazione delle informazioni all'interno di un programma.

## Definizione

Una struttura è costituita da un insieme di campi, o membri, che possono essere di diversi tipi di dati come interi, float, char, array, puntatori, o addirittura altre strutture. I membri di una struttura vengono definiti all'interno di un blocco `struct` e possono essere accessibili utilizzando l'operatore `.` (punto).

Ad esempio, consideriamo la seguente definizione di una struttura `Persona`:

```c
struct Persona {
    char nome[20];
    int eta;
    float altezza;
};
```

In questo caso, la struttura `Persona` è composta dai campi `nome`, `eta` e `altezza`, di tipo `char`, `int` e `float` rispettivamente.

## Utilizzo

Le strutture sono ampiamente utilizzate in programmazione per modellare concetti complessi e organizzare dati in modo più efficiente. Le strutture permettono di creare oggetti personalizzati che possono essere passati come argomenti alle funzioni, restituiti come valori di ritorno o memorizzati in variabili.

Ad esempio, possiamo utilizzare la struttura `Persona` definita in precedenza per creare un oggetto di tipo `Persona` e accedere ai suoi campi:

```c
struct Persona persona1;

strcpy(persona1.nome, "Mario");
persona1.eta = 30;
persona1.altezza = 1.80;

printf("Nome: %s\n", persona1.nome);
printf("Età: %d anni\n", persona1.eta);
printf("Altezza: %.2f metri\n", persona1.altezza);
```

In questo modo, le strutture consentono di organizzare dati correlati in modo più intuitivo e leggibile, migliorando la manutenibilità e la comprensibilità del codice.

In conclusione, le strutture sono un prezioso strumento in programmazione per gestire dati complessi in modo strutturato e organizzato. La loro flessibilità e versatilità le rendono un elemento fondamentale nella progettazione di software efficiente e scalabile.