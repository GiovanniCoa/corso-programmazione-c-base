# Bitwise operators

I **bitwise operators** sono operatori utilizzati nella programmazione per manipolare i valori a livello di bit. Questi operatori permettono di eseguire operazioni logiche bit a bit su numeri interi. I principali bitwise operators sono:

- **& (AND)**: restituisce 1 se entrambi i bit sono 1, altrimenti restituisce 0.
- **| (OR)**: restituisce 1 se almeno uno dei bit è 1, altrimenti restituisce 0.
- **^ (XOR)**: restituisce 1 se i bit sono diversi, altrimenti restituisce 0.
- **~ (NOT)**: inverte tutti i bit di un numero.
- **<< (Shift left)**: sposta i bit a sinistra di un numero specificato di posizioni.
- **>> (Shift right)**: sposta i bit a destra di un numero specificato di posizioni.

Questi operatori sono ampiamente utilizzati per ottimizzare il codice e per eseguire operazioni precise sui bit di un numero. Ad esempio, è possibile controllare se un bit specifico è impostato o cancellato, o combinare più flag in un unico numero utilizzando i bitwise operators.

Ecco un esempio di come utilizzare i bitwise operators in C++ per verificare se il terzo bit di un numero è impostato:

```cpp
#include <iostream>
using namespace std;

int main() {
    int num = 5; // numero binario: 101
    int mask = 1 << 2; // shift left di 2 posizioni per impostare il terzo bit

    if(num & mask) {
        cout << "Il terzo bit è impostato." << endl;
    } else {
        cout << "Il terzo bit non è impostato." << endl;
    }

    return 0;
}
```

Questo codice utilizzerà l'operatore **&** per verificare se il terzo bit di `num` è impostato confrontandolo con la maschera `mask`. Se il terzo bit è 1, la condizione sarà vera e stamperà "Il terzo bit è impostato".

In conclusione, i bitwise operators sono strumenti potenti per manipolare i valori a livello di bit e sono fondamentali per ottimizzare le prestazioni e implementare funzionalità avanzate nei linguaggi di programmazione.