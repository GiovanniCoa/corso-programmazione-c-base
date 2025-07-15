# Il primo programma: Hello World

Nel vasto mondo della programmazione, il primo passo per chiunque si avvicini a questo affascinante universo è scrivere il famoso programma "Hello World". Questo semplice programma, che consiste nel stampare a schermo la frase "Hello, World!", è spesso utilizzato come punto di partenza per imparare un nuovo linguaggio di programmazione.

## Il linguaggio C

Per scrivere il nostro primo programma "Hello World", utilizzeremo il linguaggio di programmazione C. Il linguaggio C è uno dei linguaggi più diffusi e utilizzati al mondo, ed è noto per la sua potenza e flessibilità. Scrivere un programma in C richiede una certa attenzione ai dettagli e una buona comprensione dei concetti di base della programmazione.

## Scrivere il programma

Ecco il codice sorgente del nostro primo programma "Hello World" in C:

```c
#include <stdio.h>

int main() {
    printf("Hello, World!\n");
    return 0;
}
```

Questo breve programma utilizza la funzione `printf` per stampare a schermo la frase "Hello, World!". La riga `#include <stdio.h>` è una direttiva al preprocessore del compilatore per includere la libreria standard di input/output di C.

## Compilare ed eseguire il programma

Una volta scritto il programma, è necessario compilarlo per poterlo eseguire. Per compilare il programma "Hello World" in C, è possibile utilizzare un compilatore come GCC. Ecco i passi da seguire per compilare ed eseguire il programma:

1. Salvare il codice sorgente in un file con estensione `.c`, ad esempio `hello.c`.
2. Aprire una finestra del terminale e posizionarsi nella cartella in cui si trova il file `hello.c`.
3. Eseguire il comando `gcc -o hello hello.c` per compilare il programma. Questo comando genererà un file eseguibile chiamato `hello`.
4. Eseguire il comando `./hello` per avviare il programma. A questo punto, dovresti vedere la frase "Hello, World!" stampata a schermo.

## Conclusioni

Scrivere il nostro primo programma "Hello World" in C è un ottimo modo per iniziare a familiarizzare con il linguaggio di programmazione e acquisire le competenze di base necessarie per sviluppare software più complessi. Continuando a praticare e sperimentare con il linguaggio C, è possibile ampliare le proprie conoscenze e diventare un programmatore più esperto. Buona programmazione a tutti!