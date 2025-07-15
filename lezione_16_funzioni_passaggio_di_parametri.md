# Funzioni: passaggio di parametri

Il passaggio di parametri nelle funzioni rappresenta un concetto fondamentale nella programmazione, in quanto permette di comunicare informazioni tra diverse parti del codice. Nello sviluppo di un programma, è possibile passare i parametri alle funzioni in due modi principali: per valore e per riferimento.

## Passaggio per valore
Nel passaggio per valore, il valore di una variabile viene copiato e passato alla funzione, senza influenzare la variabile originale all'esterno della funzione stessa. In questo modo, la funzione lavora con una copia del valore e le modifiche apportate all'interno della funzione non influenzano la variabile originale.

```c
void funzione(int x) {
    x = x * 2;
}

int main() {
    int num = 5;
    funzione(num);
    // Il valore di 'num' rimane 5
    return 0;
}
```

## Passaggio per riferimento
Nel passaggio per riferimento, invece, viene passato l'indirizzo di memoria della variabile, consentendo alla funzione di accedere direttamente alla variabile originale e modificarla. Questo approccio è particolarmente utile quando si desidera modificare il valore di una variabile all'interno di una funzione e rendere tale modifica visibile anche al di fuori della funzione stessa.

```c
void funzione(int* x) {
    *x = *x * 2;
}

int main() {
    int num = 5;
    funzione(&num);
    // Il valore di 'num' diventa 10
    return 0;
}
```

Il passaggio per riferimento è spesso implementato utilizzando puntatori, che consentono di manipolare direttamente la memoria e rendere le modifiche persistenti al di fuori della funzione chiamante.

In conclusione, il passaggio di parametri nelle funzioni tramite valore e riferimento rappresenta due approcci distinti con differenti effetti sulle variabili coinvolte. È importante comprendere le differenze tra i due metodi e scegliere quello più adatto alle proprie esigenze di programmazione.