# Strutture dati: liste semplici

Le liste collegate rappresentano una delle strutture dati fondamentali nella programmazione, poiché consentono di organizzare e gestire collezioni di elementi in modo dinamico e flessibile. Nell'ambito delle liste, le liste semplici rappresentano una delle forme più comuni e utilizzate.

## Creazione di una lista semplice

Per creare una lista semplice, è necessario definire una struttura di dato che contenga due campi: il valore dell'elemento e un puntatore al successivo elemento della lista. Ad esempio, in linguaggio C, la struttura potrebbe essere definita come segue:

```c
typedef struct nodo {
    int valore;
    struct nodo* successivo;
} Nodo;
```

Una volta definita la struttura, è possibile creare una lista semplice utilizzando i puntatori per collegare gli elementi tra loro.

## Gestione di una lista semplice

La gestione di una lista semplice prevede l'inserimento, la rimozione e la ricerca degli elementi. Per inserire un nuovo elemento in testa alla lista, è sufficiente creare un nuovo nodo e collegarlo al primo elemento della lista:

```c
Nodo* nuovoNodo = (Nodo*)malloc(sizeof(Nodo));
nuovoNodo->valore = 10;
nuovoNodo->successivo = primoElemento;
primoElemento = nuovoNodo;
```

Per rimuovere un elemento dalla lista, è necessario aggiornare i puntatori in modo da "saltare" l'elemento da eliminare:

```c
Nodo* nodoCorrente = primoElemento;
while (nodoCorrente->successivo != elementoDaRimuovere) {
    nodoCorrente = nodoCorrente->successivo;
}
nodoCorrente->successivo = elementoDaRimuovere->successivo;
free(elementoDaRimuovere);
```

Per cercare un elemento all'interno della lista, è possibile utilizzare un approccio iterativo o ricorsivo, scorrendo la lista e confrontando il valore di ciascun nodo con quello cercato.

## Conclusioni

Le liste semplici rappresentano una struttura dati essenziale nella programmazione, che consente di gestire collezioni di elementi in modo efficiente. Conoscere le tecniche per la creazione e la gestione di liste collegate è fondamentale per sviluppare applicazioni efficienti e robuste.