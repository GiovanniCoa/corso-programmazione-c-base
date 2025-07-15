# Libreria standard: stdio.h

La libreria stdio.h è una delle librerie standard del linguaggio di programmazione C, che fornisce le funzioni di input/output fondamentali per la gestione dei flussi di dati. Tra le principali funzioni presenti in questa libreria troviamo `printf`, `scanf`, `getchar` e `putchar`, che consentono di effettuare operazioni di input e output su console.

## Funzioni di output

La funzione `printf` è utilizzata per stampare su console dei messaggi formattati, permettendo di visualizzare testo, numeri e altri tipi di dati in maniera controllata. La sua sintassi prevede l'utilizzo di stringhe di formattazione, in cui è possibile specificare il tipo di dato da visualizzare e eventuali modificatori di formato.

Ad esempio, il seguente codice stampa un messaggio di saluto seguito dal valore di una variabile intera:

```c
int numero = 10;
printf("Ciao! Il numero è %d.\n", numero);
```

## Funzioni di input

La funzione `scanf` permette di acquisire dati da console, consentendo all'utente di inserire valori che verranno memorizzati in variabili definite dal programmatore. Anche in questo caso è possibile specificare il tipo di dato atteso e eventuali modificatori di formato.

Il seguente esempio illustra come leggere un numero intero inserito dall'utente:

```c
int numero;
scanf("%d", &numero);
printf("Hai inserito il numero %d.\n", numero);
```

## Funzioni di gestione dei caratteri

Le funzioni `getchar` e `putchar` permettono di leggere un singolo carattere da console e stampare un carattere su console, rispettivamente. Queste funzioni sono utili per gestire l'input carattere per carattere e per visualizzare dati senza formattazione aggiuntiva.

Il seguente esempio illustra come leggere un carattere inserito dall'utente e stamparlo su console:

```c
char carattere;
carattere = getchar();
putchar(carattere);
```

## Conclusioni

La libreria stdio.h fornisce le funzioni di base per gestire l'input e l'output su console in linguaggio C, consentendo ai programmatori di interagire con l'utente e visualizzare dati in maniera controllata. La conoscenza di queste funzioni è fondamentale per lo sviluppo di programmi efficienti e user-friendly.

---
Tag: stdio.h, C, programmazione, input/output, printf, scanf, getchar, putchar