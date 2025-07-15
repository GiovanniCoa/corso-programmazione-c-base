# Libreria standard: string.h

La libreria `string.h` è una delle librerie standard del linguaggio di programmazione C che fornisce un insieme di funzioni per la manipolazione delle stringhe. Questa libreria è ampiamente utilizzata per la gestione delle operazioni di base sulle stringhe come la copia, la concatenazione e la comparazione.

## Funzioni principali

Le principali funzioni della libreria `string.h` includono:

- `strlen`: restituisce la lunghezza di una stringa data.
- `strcpy`: copia una stringa in un'altra.
- `strcmp`: confronta due stringhe e restituisce un valore che indica se sono uguali o meno.

Oltre a queste funzioni, la libreria `string.h` fornisce molte altre funzioni utili per la manipolazione delle stringhe, come `strcat` per la concatenazione di stringhe, `strchr` per la ricerca di un carattere all'interno di una stringa e `strstr` per la ricerca di una sottostringa all'interno di una stringa.

## Utilizzo

Per utilizzare le funzioni della libreria `string.h`, è necessario includere l'header file `string.h` all'inizio del programma. Ad esempio, per calcolare la lunghezza di una stringa si può utilizzare la funzione `strlen` nel seguente modo:

```c
#include <string.h>
#include <stdio.h>

int main() {
    char str[] = "Hello, world!";
    int length = strlen(str);
    printf("La lunghezza della stringa è %d\n", length);
    return 0;
}
```

## Conclusioni

La libreria `string.h` è uno strumento essenziale per la manipolazione delle stringhe in linguaggio C. Le sue funzioni standard offrono un modo semplice ed efficiente per eseguire operazioni comuni su stringhe come la copia, la concatenazione e la comparazione. Grazie alla sua versatilità e alla sua ampia disponibilità, la libreria `string.h` è ampiamente utilizzata in applicazioni di programmazione in C.