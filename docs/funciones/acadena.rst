.. _acadenaLink:

.. meta::
   :description: Función base acadena() en Latino
   :keywords: manual, documentacion, latino, funciones, funcion base, acadena

============
acadena( )
============
The function **acadena\( \)** converts numbers to strings(text).

This function can be used in any type of numbers, decimals, variables, or expressions.

.. code-block:: bash

   acadena(x)            //Returns as text the numeric value of the variable X
   acadena(123)          //Returns as text the numeric value 123
   acadena(100 + 23)     //Returns as text the result of the expression

**Example**

.. raw:: html

   <pre><code class="language-latino line-numbers">x = 123
   y = acadena(x)

   escribir(x)           //Returns 123
   escribir(y)           //Returns 123
   
   /*Although visually it seems that nothing has changed if you use the tipo() function, you will see the difference*/
   
   escribir(tipo(x))     //Returns float 
   escribir(tipo(y))     //Returns string</code></pre>

----

Convert booleans to srings(textos)
-------------------------------------
The **acadena\( \)** function can be used to convert boolean (logical) values ​​to strings (texts).

.. raw:: html

   <pre><code class="language-latino line-numbers">acadena(verdadero)     //Returns "verdadero"
   acadena(falso)         //Returns "falso"</code></pre>