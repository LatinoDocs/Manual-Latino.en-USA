.. _leerLink:

.. meta::
   :description: Función base leer() en Latino
   :keywords: manual, documentacion, latino, funciones, funcion base, leer

============
leer( )
============
The **leer\( \)** function scans the numeric and alphanumeric keys entered by the user, until they press the **Enter** key .

It is recommended to assign this command to a variable, since any data entered by the user can be manipulated more easily.

.. code-block:: bash
   
   leer()

.. raw:: html

   <pre><code class="language-latino line-numbers">escribir("What's your name?")
   x = leer()
   escribir("Hi "..x)     //Returns "Hi (User name)"</code></pre>