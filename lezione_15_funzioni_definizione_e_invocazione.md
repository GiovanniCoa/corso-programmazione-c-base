# Funzioni: definizione e invocazione

Le funzioni sono blocchi di codice riutilizzabili che eseguono una specifica operazione. Definire e invocare funzioni è una pratica fondamentale nella programmazione, in quanto permette di organizzare il codice in modo modulare e di evitare la ripetizione di istruzioni.

## Definizione di una funzione

Per definire una funzione in un linguaggio di programmazione, è necessario specificare il nome della funzione, i parametri che accetta (opzionali) e il blocco di codice da eseguire quando la funzione viene invocata. Ad esempio, la seguente è la sintassi generale per definire una funzione in Python:

```python
def nome_funzione(parametro1, parametro2):
    # blocco di codice da eseguire
    return risultato
```

Nell'esempio sopra, `nome_funzione` è il nome della funzione, `parametro1` e `parametro2` sono i parametri che la funzione accetta e `risultato` è il valore restituito dalla funzione.

## Invocazione di una funzione

Una volta che una funzione è stata definita, è possibile invocarla nel codice principale per eseguire l'operazione specificata. Per invocare una funzione, è sufficiente scrivere il nome della funzione seguito dai valori dei parametri tra parentesi. Ad esempio, se vogliamo invocare la funzione `nome_funzione` definita sopra con i valori `valore1` e `valore2` come parametri, possiamo farlo nel seguente modo:

```python
risultato = nome_funzione(valore1, valore2)
```

## Esempio completo

Per comprendere meglio come funzionano la definizione e l'invocazione di una funzione, consideriamo il seguente esempio in Python:

```python
def somma(a, b):
    return a + b

risultato = somma(3, 4)
print(risultato)  # Output: 7
```

Nell'esempio sopra, abbiamo definito una funzione `somma` che accetta due parametri `a` e `b` e restituisce la somma dei due valori. Successivamente, abbiamo invocato la funzione `somma` con i valori `3` e `4` come parametri e stampato il risultato, che è `7`.

In conclusione, la definizione e l'invocazione di funzioni sono concetti fondamentali nella programmazione che consentono di organizzare il codice in modo modulare e di rendere il codice più leggibile e manutenibile. Utilizzare le funzioni in modo efficace può migliorare notevolmente l'efficienza e la qualità del codice scritto.