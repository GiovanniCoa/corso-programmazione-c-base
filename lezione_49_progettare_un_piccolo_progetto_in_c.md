# Progettare un piccolo progetto in C

Quando si progetta un piccolo progetto in linguaggio C, è fondamentale strutturare il codice in modo efficiente, organizzato e facilmente gestibile. Una delle tecniche più utilizzate per raggiungere questo obiettivo è suddividere il codice in moduli e file separati.

## Suddivisione in moduli

La suddivisione del codice in moduli consente di isolare le diverse parti del programma in unità funzionali distinte. Ogni modulo dovrebbe contenere funzioni o variabili correlate tra loro, in modo da facilitare la comprensione e la manutenzione del codice.

Ad esempio, se stiamo sviluppando un programma che gestisce una rubrica telefonica, potremmo creare moduli separati per la gestione dei contatti, la visualizzazione dei contatti, l'aggiunta di nuovi contatti, ecc.

## Utilizzo dei file

Oltre alla suddivisione in moduli, è consigliabile anche organizzare il codice in file separati. Questo permette di mantenere la struttura del progetto più pulita e ordinata, facilitando la ricerca e la modifica delle diverse parti del codice.

Ad esempio, potremmo creare un file per ogni modulo del programma, in modo da avere una struttura gerarchica e ben definita. Inoltre, l'utilizzo dei file consente anche di riutilizzare facilmente le funzioni e le variabili definite nei vari moduli, semplicemente includendo i file necessari nel codice sorgente principale.

## Esempio pratico

Di seguito vi proponiamo un esempio pratico di come potrebbe essere strutturato un piccolo progetto in C utilizzando la suddivisione in moduli e file:

```
rubrica.h     // File degli header
rubrica.c     // File sorgente principale
contatti.c    // Modulo per la gestione dei contatti
visualizzazione.c    // Modulo per la visualizzazione dei contatti
aggiunta.c    // Modulo per l'aggiunta di nuovi contatti
```

All'interno di ciascun file potremmo definire le funzioni e le variabili necessarie per il corretto funzionamento del modulo, garantendo una maggiore coesione e un migliore isolamento delle diverse parti del programma.

In conclusione, la suddivisione del codice in moduli e file separati è una pratica fondamentale per progettare e sviluppare in modo efficiente e organizzato un piccolo progetto in linguaggio C. Questo approccio permette di semplificare la manutenzione del codice, favorire il riutilizzo delle risorse e migliorare la leggibilità e la gestibilità del programma.