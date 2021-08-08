.. _imprimirfLink:

.. meta::
   :description: Función base imprimirf() en Latino
   :keywords: manual, documentacion, latino, funciones, funcion base, imprimirf

=============
imprimirf( )
=============
The **imprimirf\( \)** function is inspired by the command **printf\( \)** in C, but the command is more limited in Latino.

This command is essentially similar to **imprimir\( \)**, **escribir\( \)** and **poner\( \)** but with some differences.

The command **imprimirf\( \)** requires **\\n** at the end of each string to **escribir** on the screen, which is NOT the case with the other commands.

This command allows you to **format** an ASCII character or value.

The command **imprimirf\( \)** operates with the following format:

  * **\%c**, Converts to a character an ASCII value.
  * **\%i**, Converts to an integer.
  * **\%f**, Converts to a float.
  * **\%d**, Converts to a number.
  * **\%o**, Converts to an octal number
  * **\%x**, Converts to a hexadecimal.
  * **\%e**, Converts to a scientific expression.
  * **\%s**, Converts to a character or a string.
  * **\%%**, Returns the **porcentage (\%)** sign.

.. raw:: html

   <pre><code class="language-latino line-numbers">x = "hello"
   escribir(cadena.formato("%c",x))                //Returns h
   escribir(cadena.formato("%i",x))                //Returns 104
   escribir(cadena.formato("%f",x))                //Returns 104.000000
   escribir(cadena.formato("%d",x))                //Returns 104
   escribir(cadena.formato("%o",x))                //Returns 150
   escribir(cadena.formato("%x",x))                //Returns 68
   escribir(cadena.formato("%e",x))                //Returns 5.556763e-307
   escribir(cadena.formato("%s",x))                //Returns hello
   escribir(cadena.formato("%%",x))                //Returns %
   escribir(cadena.formato("%c",75))               //Returns K
   escribir(cadena.formato("%c%c%c",75,76,77))     //Returns KLM</code></pre>
