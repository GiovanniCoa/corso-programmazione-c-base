# File: lettura e scrittura

Nell'ambito della programmazione, la gestione dei file è un'attività fondamentale per poter manipolare e salvare dati in modo permanente su un supporto di memorizzazione. In questo articolo ci concentreremo sull'utilizzo delle funzioni di lettura e scrittura dei file in linguaggio C.

## Funzioni di lettura e scrittura

Le principali funzioni utilizzate per la manipolazione dei file in C sono `fprintf`, `fscanf`, `fread` e `fwrite`.

### fprintf

La funzione `fprintf` permette di scrivere su un file di testo formattato secondo un determinato pattern. La sintassi di base è la seguente:

```c
int fprintf(FILE *file, const char *format, ...);
```

dove `file` è un puntatore a un oggetto di tipo `FILE`, `format` è una stringa di formattazione e i parametri successivi sono i valori da scrivere sul file.

### fscanf

La funzione `fscanf` permette di leggere da un file di testo seguendo un determinato pattern di formattazione. La sintassi è simile a quella di `fprintf`:

```c
int fscanf(FILE *file, const char *format, ...);
```

### fread

La funzione `fread` permette di leggere un blocco di dati da un file binario. La sintassi di base è la seguente:

```c
size_t fread(void *ptr, size_t size, size_t count, FILE *file);
```

dove `ptr` è un puntatore al buffer in cui verranno memorizzati i dati letti, `size` è la dimensione in byte di ciascun elemento da leggere, `count` è il numero di elementi da leggere e `file` è il puntatore al file da cui leggere i dati.

### fwrite

La funzione `fwrite` permette di scrivere un blocco di dati su un file binario. La sintassi è simile a quella di `fread`:

```c
size_t fwrite(const void *ptr, size_t size, size_t count, FILE *file);
```

dove `ptr` è un puntatore ai dati da scrivere, `size` è la dimensione in byte di ciascun elemento da scrivere, `count` è il numero di elementi da scrivere e `file` è il puntatore al file su cui scrivere i dati.

## Conclusioni

Le funzioni `fprintf`, `fscanf`, `fread` e `fwrite` sono fondamentali per la gestione dei file in linguaggio C. Utilizzando correttamente queste funzioni è possibile leggere e scrivere dati in modo efficiente e sicuro. La conoscenza di queste funzioni è quindi essenziale per ogni programmatore che si occupa della manipolazione dei file.