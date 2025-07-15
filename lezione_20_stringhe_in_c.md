# Stringhe in C

Le stringhe in C sono gestite come array di caratteri terminati da un carattere nullo '\0'. Questo significa che una stringa in C è un'array di caratteri che termina con il carattere nullo che indica la fine della stringa.

## Gestione di array di caratteri

Per dichiarare una stringa in C, è possibile utilizzare la seguente sintassi:

```c
char stringa[10] = "Hello";
```

In questo caso, la stringa "Hello" è memorizzata nell'array di caratteri `stringa` di dimensione 10. È importante notare che il carattere nullo viene automaticamente aggiunto alla fine della stringa.

Per accedere ai singoli caratteri di una stringa, è possibile utilizzare l'indice dell'array come segue:

```c
char carattere = stringa[0]; // restituisce 'H'
```

## Funzioni utili per la gestione delle stringhe

In C sono disponibili diverse funzioni utili per la gestione delle stringhe, tra cui:

- `strlen()`: restituisce la lunghezza di una stringa
- `strcpy()`: copia una stringa in un'altra
- `strcat()`: concatena due stringhe
- `strcmp()`: confronta due stringhe

Esempio di utilizzo di queste funzioni:

```c
char stringa1[10] = "Hello";
char stringa2[10] = "World";

int lunghezza = strlen(stringa1); // restituisce 5
strcpy(stringa1, stringa2); // copia la stringa2 in stringa1
strcat(stringa1, " World"); // concatena " World" alla fine di stringa1
int confronto = strcmp(stringa1, stringa2); // confronta le due stringhe
```

Le stringhe in C sono un concetto fondamentale per la programmazione in C e la loro corretta gestione è essenziale per evitare problemi di buffer overflow e altri errori comuni. Utilizzando le funzioni disponibili e seguendo le best practice, è possibile gestire in modo efficiente le stringhe in C.