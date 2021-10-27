.. _asignacionLink:

.. meta::
   :description: Asignación en Latino
   :keywords: manual, documentacion, latino, sintaxis, asignacion

============
Assignment
============

+----------+---------+------------+
| Operator | Example | Equal to   |
+==========+=========+============+
| =        | x = y   | x = y      |
+----------+---------+------------+
| +=       | x += y  | x = x + y  |
+----------+---------+------------+
| \-=      | x -= y  | x = x - y  |
+----------+---------+------------+
| \*=      | x \*= y | x = x \* y |
+----------+---------+------------+
| \/=      | x \/= y | x = x \/ y |
+----------+---------+------------+
| \%=      | x \%= y | x = x \% y |
+----------+---------+------------+

----

Operator =
-----------
The operator **=** assigns a value to the variable **x**

.. raw:: html

   <pre><code class="language-latino line-numbers">x = 100</code></pre>

Operator +=
------------
The operator **+=** sums the values ​​of the variables **x** plus **y** and assigns them to the variable **x**

.. raw:: html

   <pre><code class="language-latino line-numbers">x = 10
   y = 5
   x += y
   escribir(x)  //The result will be 15</code></pre>

Operator -=
------------
The operator **-=** subtracts the values ​​of the variables **x** minus **y** and assigns them to the variable **x**

.. raw:: html

   <pre><code class="language-latino line-numbers">x = 10
   y = 5
   x -= y
   escribir(x)  //The result will be 5</code></pre>

Operator \*=
-------------
The operator **=** multiplies the values ​​of the variables **x** by **y** and assigns them to the variable **x**

.. raw:: html

   <pre><code class="language-latino line-numbers">x = 10
   y = 5
   x *= y
   escribir(x)  //The result will be 50</code></pre>

Operator /=
------------
The operator **/=** divides the values ​​of the variables **x** by **y** and assigns them to the variable **x**

.. raw:: html

   <pre><code class="language-latino line-numbers">x = 10
   y = 5
   x /= y
   escribir(x)  //The result will be 2</code></pre>

Operator %=
------------
The operator **%=** returns the remainder (module) that divides the values ​​of the variables **x** by **y** and assigns them to the variable **x**

.. raw:: html

   <pre><code class="language-latino line-numbers">x = 10
   y = 5
   x %= y
   escribir(x)  //The result will be 0</code></pre>