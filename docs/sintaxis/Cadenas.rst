.. _cadenaLink:

.. meta::
   :description: Cadenas(Textos o Strings) en Latino
   :keywords: manual, documentacion, latino, sintaxis, datos, cadenas, string, texto

==================
Strings
==================
**Strings** are used to store and manipulate text.

**Strings** are surrounded by **single quotes ( \\' )** or **double quotes ( \' )**.

.. code-block:: bash
   
   escribir("hello")
   escribir('hello')

Quotation marks can be used within a string, as long as they do not match the surrounding quotation marks.

.. raw:: html

   <pre><code class="language-latino line-numbers">escribir("His name is 'Melvin'")     //Returns: His name is 'Melvin'
   escribir('His name is "Melvin"')     //Returns: His name is "Melvin"</code></pre>

.. note:: Latino has a library for managing strings, :ref:`here <cadenalibLink>`.

----

Concatenate strings (texts)
---------------------------
To concatenate or join texts in Latino, **double periods (..)** are used , which unlike other programming languages ​​which use the plus sign **(+)**.

The **double period (..)** mark is not only useful to join texts, but also numbers.

.. raw:: html

   <pre><code class="language-latino line-numbers">x = "Hello World"
   y = ", Latino"
   escribir(x..y)     //Returns Hello World, Latino
   escribir(1..2)     //Returns 12</code></pre>

----

.. _cCaracterEspLink:

Special characters
----------------------
If strings are written in quotes, an error could occur with the following syntax:

.. raw:: html

   <pre><code class="language-latino line-numbers">escribir("Hello World, "Latino!" How are you?")</code></pre>

In the example above, the sentence would be cut to "Hello world," and Latino would think the name **Latino!** is a variable, thus producing a syntax error.

The solution to this problem would be to use a **backslash (\)** .

The **backslash (\)** converts special characters to text:

.. raw:: html

   <pre><code class="language-latino line-numbers">/*
   Returns:
   Hello World, "Latino" How are you?
   */
   
   escribir("Hello World, \"Latino!\" How are you?")</code></pre>

In addition to using the backslash to write texts, it is also used to indicate functions.

Below are the characters available for use in Latin.

Character table
+++++++++++++++++++++
+----------+-------------------------------------------------+
| Character| Description                                     |
+==========+=================================================+
| \\ \'    | Doubles quotes                                  |
+----------+-------------------------------------------------+
| \\ \\'   | Single quotes                                   |
+----------+-------------------------------------------------+
| \\n      | New line                                        |
+----------+-------------------------------------------------+
| \\r      | Carriage return                                 |
+----------+-------------------------------------------------+
| \\b      | Backspace                                       |
+----------+-------------------------------------------------+
| \\t      | Horizontal tab                                  |
+----------+-------------------------------------------------+
| \\v      | Vertical tab                                    |
+----------+-------------------------------------------------+
| \\f      | Form feed                                       |
+----------+-------------------------------------------------+
| \\a      | Beep                                            |
+----------+-------------------------------------------------+
| \\0      | Null character                                  |
+----------+-------------------------------------------------+
| \\nnn    | Character with octal value                      |
+----------+-------------------------------------------------+

.. note:: Special characters described in the table above were originally designed for `typewriter`_, teletype_, and `fax`_.

 Double quotation marks
****************
Character to use: **\\ \'**

.. raw:: html

   <pre><code class="language-latino line-numbers">/*
   Returns:
   Hello "world"
   */
   
   escribir("Hello \"world\"")</code></pre>

 Single quotes
*****************
Character to use: **\\ \\'**

.. raw:: html

   <pre><code class="language-latino line-numbers">/*
   Returns:
   Hello 'world'
   */
   
   escribir('Hello \'world\'')</code></pre>

New line
************
Character to use: **\\n**

.. raw:: html

   <pre><code class="language-latino line-numbers">/*
   Returns:
   Hello
   world
   */

   escribir("Hello\nworld")</code></pre>

Carriage return
*****************
Character to use: **\\r**

.. raw:: html

   <pre><code class="language-latino line-numbers">/*
   Unlike \n, \r does not create a new line but returns the cursor to the starting point and continues typing. This makes an overwriting.

   Returns:
   Latinoundo,
   */

   escribir("Hello World,\rLatino")</code></pre>

.. note:: To know the difference between **\\n** and **\\r** click `here`_

Backspace
********
Character to use: **\\b**

.. raw:: html

   <pre><code class="language-latino line-numbers">/*
   This command removes the previous character.

   Returns:
   Holworld
   */

   escribir("Hello\bworld")</code></pre>

Horizontal tab
**********************
Character to use: **\\t**

.. raw:: html

   <pre><code class="language-latino line-numbers">/*
   Returns:
   Hello    world
   */

   escribir("Hello\tworld")</code></pre>

Beep
*******
Character to use: **\\a**

.. raw:: html

   <pre><code class="language-latino line-numbers">/*
   It will sound the PC Beep and returns:
   Hello World
   */

   escribir("Hello World\a")</code></pre>

Null character
**************
Character to use: **\\0 \*(zero)**

.. raw:: html

   <pre><code class="language-latino line-numbers">/*
   Delete all the text after the command until the closing of the quotation marks and returns:
   Hello World Latino and happy new 2020
   */

   year = "2020"
   escribir("Hello World,\0 Latino! and happy new "..year)</code></pre>

.. note:: In the same way \0 being a null value, it can also be used in logical conditionals:
   
   **Example 1**
   
   .. raw:: html

      <pre><code class="language-latino line-numbers">/*
      Returns:
      The value is not null
      */

      x = 5
      
      si x != "\0"
        escribir ("The value is not null") 
      fin</code></pre>
   
   **Example 2**

   .. raw:: html

      <pre><code class="language-latino line-numbers">/*
      Returns:
      It is not null
      */

      x = 5

      si x == "\0"
        escribir ("It is null")
      sino
        escribir ("It is not null")
      fin</code></pre>

Character with octal value
*************************
Character to use: **\\nnn**

.. raw:: html

   <pre><code class="language-latino line-numbers">/*
   Returns:
   Hello World
   */

   text = "\110\157\154\141\040\155\165\156\144\157"
   escribir(text)</code></pre>

----

Multiple line texts
---------------------------
We saw previously that strings can be linear texts, but they can also be multi-line texts.

To indicate when a string will be multi-line, just leave one of the quotation marks at the beginning and another at the end of the paragraph.

.. raw:: html

   <pre><code class="language-latino line-numbers">escribir("Sample multiple line text:
   ---------------------------------------
   In this example we can observe   
   that Latino is perfectly capable of
   process multi-line texts
   as long as one of the two quotes
   is at the beginning of the paragraph and another at the end")</code></pre>

----

Texts as arrays
--------------------
As in many other programming languages, texts are :ref:`arrays <listaLink>`.

.. raw:: html

   <pre><code class="language-latino line-numbers">/*
   Returns:
   the letter "e"
   */

   x = "Hello"
   escribir(x[1])</code></pre>

----

Convert numbers to strings
----------------------------
In Latino there is a pre-defined function called **acadena( )** that converts a number to a string (text).

.. raw:: html
   
   <pre><code class="language-latino line-numbers">x = 100
   escribir(tipo(x))     //Returns decimal
   
   x = acadena("100")
   escribir(tipo(x))     //Returns string</code></pre>

.. Enlaces:

.. _typewriter: https://es.wikipedia.org/wiki/Máquina_de_escribir
.. _teletype: https://es.wikipedia.org/wiki/Teletipo
.. _fax: https://es.wikipedia.org/wiki/Fax
.. _here: https://es.stackoverflow.com/a/172368/183823