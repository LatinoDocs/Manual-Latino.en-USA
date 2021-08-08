.. _tipoLink:

.. meta::
   :description: Función base tipo() en Latino
   :keywords: manual, documentacion, latino, funciones, funcion base, tipo

============
tipo( )
============
The **tipo\( \)** function returns the type of value stored in a variable or memory.

The values ​​that this function can return can be found in :ref:`data types <tiposDeDatosLink>`.

.. raw:: html

   <pre><code class="language-latino line-numbers">x = 123
   escribir(tipo(x))     //Returns decimal

   x = "Hello world"
   escribir(tipo(x))     //Returns cadena

   x = ["Hello", "world"]
   escribir(tipo(x))     //Returns lista

   x = {"Message":"Hello", "Planet":"world"}
   escribir(tipo(x))     //Returns diccionario
   
   x = verdadero
   escribir(tipo(x))     //Returns logico
   
   x = nulo
   escribir(tipo(x))     //Returns nulo</code></pre>