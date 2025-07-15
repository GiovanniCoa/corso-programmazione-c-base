# Struttura di un programma C

Un programma in linguaggio C è generalmente strutturato in diverse sezioni che ne definiscono il funzionamento e l'organizzazione. In questo articolo analizzeremo le sezioni principali di un programma C, tra cui le direttive, la funzione main e le istruzioni.

## Direttive

Le direttive sono istruzioni che vengono interpretate dal preprocessore prima della compilazione del codice sorgente. Le direttive più comuni includono `#include` per l'inclusione di file di intestazione, `#define` per la definizione di costanti simboliche e macro sostitutive, e `#ifdef`, `#ifndef`, `#if`, `#else`, `#elif` e `#endif` per l'inclusione condizionale di codice.

## Funzione main

La funzione `main` è il punto di ingresso di un programma C e viene eseguita per prima. La sua firma è di solito `int main(void)` o `int main(int argc, char *argv[])`, dove `argc` rappresenta il numero di argomenti passati al programma e `argv` è un array di stringhe contenente tali argomenti. La funzione `main` restituisce un valore intero che rappresenta lo stato di uscita del programma.

## Istruzioni

Le istruzioni in un programma C definiscono le azioni da eseguire dal programma. Le istruzioni possono essere di diversi tipi, tra cui assegnazioni, chiamate di funzioni, istruzioni di controllo come `if`, `else`, `switch` e cicli come `while`, `for` e `do-while`.

## Esempio di struttura di un programma C

```c
#include <stdio.h>

#define PI 3.14159

int main(void) {
    int r = 5;
    float area;

    area = PI * r * r;

    printf("L'area del cerchio di raggio %d è: %.2f\n", r, area);

    return 0;
}
```

In questo esempio, vengono utilizzate direttive per includere il file di intestazione `stdio.h` e definire la costante `PI`. La funzione `main` calcola l'area di un cerchio di raggio 5 e stampa il risultato a schermo.

In conclusione, la struttura di un programma C è composta da diverse sezioni che definiscono il comportamento del programma. Comprendere e utilizzare correttamente queste sezioni è fondamentale per la scrittura di codice C efficiente e ben organizzato.