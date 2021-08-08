.. _anumeroLink:

.. meta::
   :description: Función base anumero() en Latino
   :keywords: manual, documentacion, latino, funciones, funcion base, anumero

============
anumero( )
============
The **anumero\( \)** function convers strings (text) to numbers.

Quotation marks without characters, such as **\'\'** will return **Nulo** the same as the number **0**.

Blanks **\' \'** or whatever number that has a blank, such as **\'7 \'** will be converted to `ALT Code`_.

**Example**

.. raw:: html

   <pre><code class="language-latino line-numbers">escribir(anumero("3.14"))     //Returns 3.14
   escribir(anumero(""))         //Returns nulo
   escribir(anumero("0"))        //Returns nulo
   escribir(anumero(" "))        //Returns 32 (This is the same in ALT Code)
   escribir(anumero("9"))        //Returns 9
   escribir(anumero("9 "))       //Returns 57(Since it has a blankm it returns its ALT Code)</code></pre>

----

Convert booleans to numbers
-----------------------------
The **anumero\( \)** function can be used to convert boolean (logical) values ​​to a numeric value.

.. raw:: html

   <pre><code class="language-latino line-numbers">anumero(verdadero)     //Returns 1
   anumero(falso)         //Returns "nulo" (It doesn't return 0, because its value is represented by a null)</code></pre>

.. Enlaces

.. _ALT Code: https://en.wikipedia.org/wiki/Alt_code