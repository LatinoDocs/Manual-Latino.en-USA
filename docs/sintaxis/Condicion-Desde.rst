.. _desdeLink:

.. meta::
   :description: Condición desde en Latino
   :keywords: manual, documentacion, latino, sintaxis, desde, for

===========================
Desde loop(For Loop)
===========================
**Desde** repeats the same code over and over again until its expression is fulfilled (is true).

Typically, the **desde** loop is used to navigate between items in an **array** or **dictionary**, but also to execute code that will be repetitive.

----

"Desde" loop syntax
------------------------------------

**Syntax example**

.. code-block:: bash
   
   desde (declaration; expresion; statement)
     #Code block
   fin

+-----------------+--------------------------------------------------------------------+
| Declarations    | Description                                                        |
+=================+====================================================================+
| **Declaration** | This is executed (only once) before the execution of the code      |
+-----------------+--------------------------------------------------------------------+
| **Expresion**   | Define the conditions for the code block to be executed            |
+-----------------+--------------------------------------------------------------------+
| **Statement**   | This is executed (every time) after executing the code block       |
+-----------------+--------------------------------------------------------------------+

**Sample code**

.. raw:: html

   <pre><code class="language-latino line-numbers">/*
  In the following code
    as long as the variable i is less than or equal to 10
    the conditional from will continue to run.
   
   The program will print on the screen:
   0 1 2 3 4 5 6 7 8 9 10
   */

   desde (i = 0; i <= 10; i++)
     escribir(i)
   fin</code></pre>

.. raw:: html
   
   <pre><code class="language-latino line-numbers">/*
   In this other example
   the program will print on the screen:
   10 9 8 7 6 5 4 3 2 1 0
   */

   desde (i = 10; i >= 0; i--)
     escribir(i)
   fin
   #output: 10 9 8 7 6 5 4 3 2 1 0</code></pre>

----

A different way can be specified by changing the increment expression.

.. raw:: html

   <pre><code class="language-latino line-numbers">desde(i = 0; i < 50; i = i+10)
     imprimir(i)
   fin
   #output: 0 10 20 30 40</code></pre>

----

Use of libraries
-----------------
**Expresiones** of the **desde** loop can implement the use of :ref:`libraries <libreriasLink>`, like this:

.. raw:: html

   <pre><code class="language-latino line-numbers">/*
   This operation compare the amount
   of items in the fruit array and
   will write them on screen, like this:

   > apple
   > grape
   > cherry
   */

   fruit = ["apple", "grape", "cherry"]

   desde(i=0; i < lista.longitud(fruit); i++)
     imprimir(fruit[i])
   fin</code></pre>

----

Nesting "desde" loop
---------------------------
When a **desde** loop contains another **desde** loop within it, it's called **nested loop**.

When the **desde** loop ( parent ) executes and reaches a nested loop ( child ), the parent loop does not continue until the child loop completes all of its cycles (until it is true). This whole cycle will repeat itself until the parent loop is true.

.. raw:: html

   <pre><code class="language-latino line-numbers">/*
   This operation compares the quantity
   of elements in the fruit array and adjectives
   will write them on screen, like this:

   > green apple
   > green grape
   > green cherry
   > big apple 
   > big grape
   > big cherry
   > delicious apple
   > delicious grape
   > delicious cherry
   */
   
   fruit    = ["apple", "grape", "cherry"]
   adjectives = ["green", "big", "delicious"]

   desde(i=0; i < lista.longitud(adjectives); i++)
     desde (e=0; e < lista.longitud(fruit); e++)
       escribir (adjectives[i].." "..fruit[e])
     fin
   fin</code></pre>