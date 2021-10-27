.. meta::
   :description: Condición elegir en Latino
   :keywords: manual, documentacion, latino, sintaxis, elegir, switch

==========================
Elegir conditional (Switch)
==========================
The **Elegir condiditional** is an alternative to :ref:`si conditional <siLink>` that we saw in the previous chapter.

This conditional is used to perform different actions based on different logical conditions. In other words, this conditional evaluates an option in multiple possible cases and selects one of several code blocks to be executed.

The choose conditional contains the following statements:

+-------------+--------------------------------------------------------------------------------------------------------------+
| Commands    | Description                                                                                                  |
+=============+==============================================================================================================+
| **elegir**  | Beginning of the declaration. It evaluates the conditional expression.                                             |
+-------------+--------------------------------------------------------------------------------------------------------------+
| **caso**    | The result of the expression is evaluated and if it matches any case it is executed.        |
+-------------+--------------------------------------------------------------------------------------------------------------+
| **defecto** | If there is no match in any of the cases, this block of code will be executed. |
+-------------+--------------------------------------------------------------------------------------------------------------+
| **otro**    | It is exactly the same as the **defecto** command only with another name.                                 |
+-------------+--------------------------------------------------------------------------------------------------------------+
| **fin**     | 	It marks the end of the statement.                                                                             |
+-------------+--------------------------------------------------------------------------------------------------------------+
| **romper**  | Stops code execution.                                                                         |
+-------------+--------------------------------------------------------------------------------------------------------------+

----

Syntax of the "elegir" conditional
------------------------------------

**Syntax example**

.. code-block:: bash
   
   elegir(expression)
     caso 1:
       #Code block
       romper
     caso 2:
       #Code block
       romper
     defecto:
       #Code block
   fin

**Code example**

.. raw:: html

   <pre><code class="language-latino line-numbers">/*
   Depending on which condition is fulfilled, it will execute the code in its corresponding case. 
   
   In this example the program will write on the screen 
   
   Well done!.
   */
   score = 'B'

   elegir(score)
     caso 'A':
       escribir("¡Excellent!.")
     caso 'B':
       escribir("¡Well done!.")
     caso 'C':
       escribir("¡Well done!.")
     caso 'D':
       escribir("You need to improve")
     caso 'F':
       escribir("You failed.")
     otro:
       escribir("Invalid score")
   fin</code></pre>

.. note:: Note that the case has to be repeated for B and C at the moment, multiple cases are not allowed as a single option.
