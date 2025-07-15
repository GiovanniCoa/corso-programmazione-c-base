# Strutture dati: stack e queue

Le strutture dati stack e queue sono fondamentali nel campo dell'informatica e della programmazione. Esse permettono di gestire e organizzare i dati in modo efficiente, consentendo l'accesso e la manipolazione dei dati in modo rapido ed efficace.

## Stack

Lo stack, o pila, è una struttura dati in cui l'accesso ai dati avviene secondo il principio LIFO (Last In First Out). Questo significa che l'ultimo elemento inserito è il primo ad essere estratto. Lo stack può essere implementato sia tramite array che tramite puntatori.

### Implementazione con array

Nell'implementazione con array, uno stack può essere rappresentato come un array di dimensione fissa. Per gestire lo stack, è necessario tener traccia dell'indice del top dello stack, ovvero dell'elemento più recentemente inserito. Le operazioni fondamentali su uno stack implementato con array sono la push (inserimento di un elemento) e la pop (estrazione di un elemento).

```c
#define MAX_SIZE 100

typedef struct {
    int data[MAX_SIZE];
    int top;
} Stack;

void push(Stack *stack, int value) {
    if (stack->top < MAX_SIZE) {
        stack->data[stack->top++] = value;
    }
}

int pop(Stack *stack) {
    if (stack->top > 0) {
        return stack->data[--stack->top];
    }
    return -1; // stack vuoto
}
```

### Implementazione con puntatori

Nell'implementazione con puntatori, uno stack può essere rappresentato come una lista concatenata di nodi, in cui ogni nodo contiene un valore e un puntatore al nodo successivo. Le operazioni fondamentali su uno stack implementato con puntatori sono la push e la pop.

```c
typedef struct Node {
    int data;
    struct Node *next;
} Node;

typedef struct {
    Node *top;
} Stack;

void push(Stack *stack, int value) {
    Node *newNode = malloc(sizeof(Node));
    if (newNode) {
        newNode->data = value;
        newNode->next = stack->top;
        stack->top = newNode;
    }
}

int pop(Stack *stack) {
    if (stack->top) {
        int value = stack->top->data;
        Node *temp = stack->top;
        stack->top = stack->top->next;
        free(temp);
        return value;
    }
    return -1; // stack vuoto
}
```

## Queue

La queue, o coda, è una struttura dati in cui l'accesso ai dati avviene secondo il principio FIFO (First In First Out). Questo significa che il primo elemento inserito è il primo ad essere estratto. Anche la queue può essere implementata sia tramite array che tramite puntatori.

### Implementazione con array

Nell'implementazione con array, una queue può essere rappresentata come un array circolare. Per gestire la queue, è necessario tener traccia dell'indice del front e del rear della coda. Le operazioni fondamentali su una queue implementata con array sono l'enqueue (inserimento di un elemento) e la dequeue (estrazione di un elemento).

```c
#define MAX_SIZE 100

typedef struct {
    int data[MAX_SIZE];
    int front, rear;
}