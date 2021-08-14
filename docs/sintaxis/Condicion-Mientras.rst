.. meta::
   :description: Condición mientras en Latino
   :keywords: manual, documentacion, latino, sintaxis, mientras, while

================================
Mientras loop (While Loop)
================================
The **mientras loop** executing a block of code repeatedly as long as its **condition** is still met (is true).

This loop first verifies that its condition is met before executing the code.
----

Syntax of the loop "mientras"
--------------------------------------

**Syntax example**

.. code-block:: bash
   
   mientras (condition)
     #Code block
   fin

**Code example**

.. raw:: html

   <pre><code class="language-latino line-numbers">/*
   As long as the operation is true
   this code will write on screen
   the following numbers:
   0 1 2 3 4 5 6 7 8 9
   */

   i=0
   
   mientras i < 10
     escribir(i)
     i++            //Increases the value of i
   fin</code></pre>

.. note:: In this example, if the value of the variable **i** is not increased, this loop would repeat infinitely without stopping, producing an error in memory.

----

Difference between "mientras" and "desde"
---------------------------------------
As you may have noticed, the **mientras** command and the **desde** command are very similar to each other, with the difference that the **mientras** command does not require a declaration or statement as in the **desde** command .

**Example #1: "desde"**

This example uses the command **desde** to acquire the car brands in a variable.

.. raw:: html

   <pre><code class="language-latino line-numbers">/*
   In this example, print on screen:
   BMW
   Volvo
   Ford
   Nissan
   */
   
   cars = ["BMW", "Volvo", "Ford", "Nissan"]
   text = ""

   desde (i=0; i < lista.longitud(cars); i++)
     text = text..cars[i].."\n"     # \n means new line
   fin
   
   escribir(text)</code></pre>

**Example #2: "mientras"**

This example is similar to the previous one with the difference that the **mientras** command will be used .

.. raw:: html

   <pre><code class="language-latino line-numbers">/*
   In this example, print on screen:
   BMW
   Volvo
   Ford
   Nissan
   */

   cars = ["BMW", "Volvo", "Ford", "Nissan"]
   i = 0
   text = ""

   mientras(i < lista.longitud(cars))
     text = text..cars[i].."\n"     # \n means new line
   i++
   fin

   escribir(text)</code></pre>