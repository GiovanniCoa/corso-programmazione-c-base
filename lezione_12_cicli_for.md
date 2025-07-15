# Cicli: for

Il ciclo `for` è uno dei costrutti fondamentali nei linguaggi di programmazione, che permette di eseguire iterazioni controllate su una sequenza di elementi. In particolare, il ciclo `for` è ampiamente utilizzato per attraversare gli elementi di una lista, di un array o di qualsiasi altra struttura dati che permetta l'accesso sequenziale.

La sintassi del ciclo `for` è generalmente la seguente:

```python
for elemento in sequenza:
    # blocco di istruzioni da eseguire per ogni elemento della sequenza
```

Nel blocco di istruzioni all'interno del ciclo `for`, è possibile manipolare l'elemento corrente della sequenza attraverso la variabile di ciclo `elemento`.

La variabile di ciclo viene aggiornata automaticamente ad ogni iterazione, permettendo di accedere in modo semplice e intuitivo agli elementi della sequenza. Ad esempio, nel caso di una lista di numeri, è possibile eseguire operazioni aritmetiche su ciascun numero utilizzando la variabile di ciclo.

Un esempio di utilizzo del ciclo `for` in Python potrebbe essere il seguente:

```python
numeri = [1, 2, 3, 4, 5]

for numero in numeri:
    quadrato = numero ** 2
    print(f"Il quadrato di {numero} è {quadrato}")
```

In questo caso, il ciclo `for` attraversa la lista di numeri e per ciascun numero calcola il suo quadrato, stampando il risultato a schermo.

Il ciclo `for` è particolarmente utile quando si conosce a priori il numero di iterazioni da eseguire, ad esempio quando si deve attraversare una lista di elementi o eseguire un'operazione un certo numero di volte.

In conclusione, il ciclo `for` è uno strumento potente e flessibile per gestire iterazioni controllate su sequenze di elementi, grazie alla presenza della variabile di ciclo che semplifica l'accesso e la manipolazione degli elementi. La sua sintassi chiara e intuitiva lo rende uno dei costrutti più utilizzati nella programmazione strutturata.