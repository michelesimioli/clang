Programma più complesso
=======================

Il programma converte libbre in formato US e UK in chilogrammi.

*(convert.c)*

.. code-block:: c

  #include <stdio.h>
  #define KILOS*PER*POUND .45359

  int main() {       
      int pounds;

      printf(" US lbs      UK st. lbs       INT Kg\n");
      for(pounds=10; pounds < 250; pounds+=10){
          int stones = pounds / 14;
          int uklbs = pounds % 14;
          float kilos = pounds * KILOS*PER*POUND;
          printf("   %d           %d   %d        %f\n",
                  pounds, stones, uklbs, kilos);
      }
      return 0;
  }


Componenti del programma
------------------------

``#define KILOS*PER*POUND .45359``

* Definizione di macro per il preprocessore: ``#define nome valore``

  * Il preprocessore opera una pura sostituzione lessicale

``{ ... }``

* Blocco di istruzioni (del ``main``, del ``for``, ...)

``int pounds;``

* Dichiarazione della variabile ``pounds``

  * Tutte le variabili devono essere dichiarate all'inizio del blocco in cui si usano
  * Sono visibili nei sottoblocchi ma non nei blocchi sopra

``int stones = pounds / 14;``

* Variabile inizializzata alla dichiarazione

``for(pounds=10; pounds < 250; pounds+=10){ ... }``

* Ciclo di ``for`` (iterazione)
