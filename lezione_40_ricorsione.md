# Ricorsione

La ricorsione è un concetto fondamentale nella programmazione che consiste nell'utilizzare una funzione per chiamare se stessa. Questo approccio permette di risolvere problemi complessi in modo elegante e efficiente, suddividendoli in casi più piccoli.

## Funzioni ricorsive

Le funzioni ricorsive sono composte da due elementi fondamentali:
- **Caso base**: rappresenta il punto in cui la funzione smette di richiamare se stessa e restituisce un valore. È essenziale per evitare un loop infinito.
- **Caso ricorsivo**: rappresenta il punto in cui la funzione si chiama nuovamente con argomenti diversi, procedendo verso il caso base.

Un esempio classico di funzione ricorsiva è il calcolo del fattoriale di un numero. La definizione matematica del fattoriale di un numero n è:
```
n! = n * (n-1) * (n-2) * ... * 1
```

## Esempio di funzione ricorsiva per il calcolo del fattoriale

Di seguito è riportato un esempio di funzione ricorsiva in Python per il calcolo del fattoriale di un numero:

```python
def fattoriale(n):
    if n == 0:
        return 1
    else:
        return n * fattoriale(n-1)
```

In questo caso, il caso base è rappresentato da `n == 0`, mentre il caso ricorsivo è dato dalla formula `n * fattoriale(n-1)`.

## Vantaggi e svantaggi della ricorsione

La ricorsione offre alcuni vantaggi, tra cui:
- Chiarezza del codice: permette di esprimere in modo elegante soluzioni a problemi complessi.
- Modularità: consente di suddividere il problema in sottoproblemi più semplici.

Tuttavia, la ricorsione presenta anche alcuni svantaggi, tra cui:
- Consumo di memoria: ogni chiamata ricorsiva aggiunge uno stack frame alla memoria, potenzialmente causando problemi di stack overflow.
- Prestazioni: in alcuni casi, l'implementazione ricorsiva può essere meno efficiente di una soluzione iterativa.

## Conclusioni

La ricorsione è un potente strumento nella programmazione che consente di risolvere problemi complessi in modo elegante e efficiente. È importante comprendere i concetti di base delle funzioni ricorsive, come i casi base e ricorsivi, per utilizzare al meglio questo approccio. Tuttavia, è fondamentale valutare attentamente i vantaggi e gli svantaggi della ricorsione per scegliere la soluzione più adatta al problema da risolvere.