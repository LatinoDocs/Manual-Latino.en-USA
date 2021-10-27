.. _aritmeticaLink:

.. meta::
   :description: Aritmética en Latino
   :keywords: manual, documentacion, latino, sintaxis, aritmetica

============
Arithmetic
============

Arithmetic operators
-----------------------
Arithmetic operators perform basic mathematical operations such as addition, subtraction, multiplication, and division on numeric values ​​(constants and variables).

+----------+--------------------------------+
| Operator | Description                    |
+==========+================================+
| \+       | Addition                       |
+----------+--------------------------------+
| \-       | Subtraction                    |
+----------+--------------------------------+
| \*       | Multiplication                 |
+----------+--------------------------------+
| \/       | Division                       |
+----------+--------------------------------+
| \%       | Modulo (Remainder)             |
+----------+--------------------------------+
| \^       | Power (Exponential)            |
+----------+--------------------------------+

----

**Examples:**

A common arithmetic operation would be with two numbers.

With two literal numbers:

.. raw:: html

   <pre><code class="language-latino line-numbers">x = 100 + 50</code></pre>

or also with variables:

.. raw:: html

   <pre><code class="language-latino line-numbers">x = a + b</code></pre>

or also with expressions:

.. raw:: html

   <pre><code class="language-latino line-numbers">x = (100 + 50) * a</code></pre>

----

Addition
+++++
The **sum** operator(\+):

.. raw:: html

   <pre><code class="language-latino line-numbers">x = 5
   y = 2
   z = x + y
   escribir(z)    //The result would be 7</code></pre>

Substraction
++++++
The **substaction** operator (\-):

.. raw:: html

   <pre><code class="language-latino line-numbers">x = 5
   y = 2
   z = x - y
   escribir(z)    //The result would be 3</code></pre>

Multiplication
+++++++++++++++
The **multiplication** operator (\*):

.. raw:: html

   <pre><code class="language-latino line-numbers">x = 5
   y = 2
   z = x * y
   escribir(z)    //The result would be 10</code></pre>

Division
+++++++++
The **division** operator (/):

.. raw:: html

   <pre><code class="language-latino line-numbers">x = 5
   y = 2
   z = x / y
   escribir(z)    //The result would be 2.5</code></pre>

Modulo (Remainder)
+++++++++++++++++++
The **remainder** operator (\%):

.. raw:: html

   <pre><code class="language-latino line-numbers">x = 5
   y = 2
   z = x % y
   escribir(z)    //The result would be 1</code></pre>

Power
+++++++++
The **exponential** operator (\^):

.. raw:: html

   <pre><code class="language-latino line-numbers">x = 5
   y = 2
   z = x ^ y
   escribir(z)    //The result would be 25</code></pre>

.. note:: For power calculations, you can achieve the same result using the math library **mate.pot(x,y)**
   
   .. raw:: html
   
      <pre><code class="language-latino line-numbers">x = 5
      y = 2
      escribir(mate.pot(x,y))    //The result would be 25</code></pre>

----

.. _aritmeticaIncre:

Increment and decrement operators
--------------------------------------

Increment
++++++++++++++
The increment operator is represented by a **double addition** (+ +).

.. raw:: html

   <pre><code class="language-latino line-numbers">x = 5         //Declare a variable with value 5
   x++           //The value of the variable X increments by 1
   escribir(x)   //The result would be 6</code></pre>

Decrement
+++++++++++++++
The decrement operator is represented by a **double substraction** (\- \-).

.. raw:: html

   <pre><code class="language-latino line-numbers">x = 5         //Declare a variable with value 5
   x--           //The value of the variable X decrease by 1
   escribir(x)   //The result would be 4</code></pre>

----

Precedence in Operators
------------------------------
In arithmetic, all operators (arithmetic, logical, and relational) have **precedence rules** that apply when several operators act together, and Latino makes use of those rules.

Arithmetic operators, such as multiplication and division, are performed before addition or subtraction.

To override these precedence rules, **parentheses ()** can be used .

.. raw:: html

   <pre><code class="language-latino line-numbers">x = 100 + 50 * 3       //Returns 250
   y = (100 + 50) * 3     //Returns 450
   escribir ("Value of X: " .. x .. ", Value of Y: ".. y)</code></pre>