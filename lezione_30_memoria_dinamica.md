# Memoria dinamica

La memoria dinamica è un aspetto fondamentale della programmazione, che consente di gestire in modo flessibile e efficiente l'allocazione e la deallocazione della memoria durante l'esecuzione di un programma. In questo articolo ci concentreremo su quattro funzioni chiave per la gestione della memoria dinamica: `malloc`, `calloc`, `realloc` e `free`.

## malloc

La funzione `malloc` è utilizzata per allocare una certa quantità di memoria non inizializzata. La sua firma è la seguente:

```c
void* malloc(size_t size);
```

La funzione restituisce un puntatore al blocco di memoria allocato, di dimensione `size` in byte. È importante notare che il contenuto della memoria allocata da `malloc` non è inizializzato, quindi potrebbe contenere valori indeterminati.

Esempio di utilizzo di `malloc`:

```c
int* array = (int*)malloc(10 * sizeof(int));
```

## calloc

La funzione `calloc` è simile a `malloc`, ma alloca e inizializza la memoria a zero. La sua firma è la seguente:

```c
void* calloc(size_t num, size_t size);
```

La funzione restituisce un puntatore al blocco di memoria allocato, composto da `num` elementi di dimensione `size` in byte ciascuno.

Esempio di utilizzo di `calloc`:

```c
int* array = (int*)calloc(10, sizeof(int));
```

## realloc

La funzione `realloc` è utilizzata per ridimensionare un blocco di memoria precedentemente allocato con `malloc` o `calloc`. La sua firma è la seguente:

```c
void* realloc(void* ptr, size_t size);
```

La funzione restituisce un puntatore al blocco di memoria ridimensionato, di dimensione `size` in byte. Il contenuto del blocco di memoria viene preservato nella misura del possibile durante il ridimensionamento.

Esempio di utilizzo di `realloc`:

```c
array = (int*)realloc(array, 20 * sizeof(int));
```

## free

La funzione `free` è utilizzata per deallocare un blocco di memoria precedentemente allocato con `malloc`, `calloc` o `realloc`. La sua firma è la seguente:

```c
void free(void* ptr);
```

Dopo aver chiamato `free`, il puntatore `ptr` non è più valido e non deve essere utilizzato. È importante ricordare di deallocare la memoria allocata per evitare memory leak.

Esempio di utilizzo di `free`:

```c
free(array);
```

In conclusione, la gestione della memoria dinamica è un aspetto critico della programmazione, che richiede attenzione e cura. Utilizzando correttamente le funzioni `malloc`, `calloc`, `realloc` e `free`, è possibile allocare e deallocare la memoria in modo efficiente e sicuro, evitando problemi di allocazione e deallocazione della memoria.