# Controllo del flusso: switch

Il costrutto switch-case è un'alternativa molto utile per gestire il flusso di esecuzione in un programma, in particolare quando si ha la necessità di confrontare una variabile con diversi valori. Rispetto alla sequenza di istruzioni if-else, lo switch-case risulta essere più leggibile e manutenibile quando si devono gestire molteplici casi.

## Struttura del costrutto switch-case

La struttura di base di uno switch-case è la seguente:

```markdown
switch (espressione) {
    case valore1:
        // istruzioni da eseguire se espressione equivale a valore1
        break;
    case valore2:
        // istruzioni da eseguire se espressione equivale a valore2
        break;
    ...
    default:
        // istruzioni da eseguire se nessun caso corrisponde a espressione
        break;
}
```

Nella parte `switch (espressione)` viene specificata la variabile da confrontare con i valori dei casi successivi. Per ogni caso si specifica il valore da confrontare e le istruzioni da eseguire nel caso in cui la variabile corrisponda a quel valore. Il blocco `default` è facoltativo e viene eseguito nel caso in cui nessuno dei casi precedenti corrisponda al valore della variabile.

## Vantaggi dello switch-case

L'utilizzo dello switch-case presenta diversi vantaggi rispetto alla sequenza di istruzioni if-else:

- **Leggibilità**: la struttura dello switch-case rende più chiara la logica di controllo del flusso, soprattutto quando si hanno molti casi da gestire.
- **Velocità**: lo switch-case è generalmente più veloce delle istruzioni if-else quando si hanno molti casi, in quanto l'interprete può ottimizzare la gestione dei salti.
- **Manutenibilità**: la struttura dello switch-case facilita l'aggiunta e la modifica dei casi, rendendo il codice più flessibile e meno soggetto a errori.

## Esempio di utilizzo

Ecco un esempio di utilizzo dello switch-case in un programma in C per determinare il giorno della settimana in base a un numero fornito in input:

```c
#include <stdio.h>

int main() {
    int giorno;

    printf("Inserisci un numero da 1 a 7: ");
    scanf("%d", &giorno);

    switch (giorno) {
        case 1:
            printf("Lunedì\n");
            break;
        case 2:
            printf("Martedì\n");
            break;
        case 3:
            printf("Mercoledì\n");
            break;
        case 4:
            printf("Giovedì\n");
            break;
        case 5:
            printf("Venerdì\n");
            break;
        case 6:
            printf("Sabato\n");
            break;
        case 7:
            printf("Domenica\n");
            break;
        default:
            printf("Numero non valido\n");
            break;
    }

    return 0;
}
```

In questo esempio, vengono confrontati i valori da 1 a 7 con la variabile `giorno` e stampato il corrispond