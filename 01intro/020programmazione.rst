Primo Programma
===============


*(ciao.c)*

.. code-block:: c

    #include <stdio.h>

    int main() {
        printf("Il mio primo programma\n");
        return 0;
    }


Osservazioni
------------

* File di testata (header) ``stdio.h``

  * Contiene la dichiarazione della funzione ``printf()``

* Direttiva del preprocessore ``#include``

  * Preprocessore lanciato prima del compilatore

* Tutti i programmi hanno la funzione ``main()``

  * Definisce il punto d'ingresso al programma
  * Ritorna un intero, il codice di ritorno
  * ``0`` se il programma ha avuto successo, ``>0`` se c'erano errori

* Funzione di libreria standard ``printf()``

  * Libreria standard sempre linkata con i programmi

* Tutte le istruzioni terminano con punto e virgola

  * Il formato è libero ma vi sono convenzioni di formattazione

**NB**: Il primo errore è di scordare il punro e virgola.

Compilazione ed esecuzione
--------------------------

Sintassi:


    cc [opzioni] sorgente ...


Nel nostro caso: ``cc -o ciao ciao.c``

* Tutti i file sorgente devono avere suffisso ``.c``
* L'opzione ``-o ciao`` determina il nome dell'eseguibile

  * Di default il nome è ``a.out``

* Le opzioni possono avere argomenti
* Flessibilità nell'ordine delle opzioni

Esecuzione in Unix/Linux:


    ./ciao

