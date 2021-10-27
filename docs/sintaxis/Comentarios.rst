.. meta::
   :description: Comentarios en Latino
   :keywords: manual, documentacion, latino, sintaxis, comentario

============
Comments
============
Like other programming languages, Latino has comments. These comments can be used to create notes that help explain some code that we have written or also use it to prevent the execution of any line of code when executing the program.

----

Single line comments
--------------------------------
Single line comments can start with a **#** or **//** mark. Any text or code that is after these signs will be ignored by Latino (they will not be executed).

This example will use the one-line comment before each line of code:

.. raw:: html
   
   <pre><code class="language-latino line-numbers">//This line of code will show the message <code class="l">Hello world</code> when executing the program
   escribir ("Hello world")
   #The following line of code will add the values and its result will be written on the screen
   escribir (5+5)</code></pre>

This example uses a single line comment at the end of each line to explain the code:

.. raw:: html
   
   <pre><code class="language-latino line-numbers">x = 5            #We declare a variable with the name of X, and we have assigned it a value of 5
   y = x + 2        #We declare a variable with the name of Y, and we have assigned the value of X plus 2
   escribir (y)     //In this line of code we will write on the screen the value of Y which has the value of X + 2</code></pre>

----

Multi-line comments
--------------------------------
Multi-line comments start with /* and end with * /. Any text or code that is within these signs will be ignored by Latino (they will not be executed)..

This example will use the multiline comment:

.. raw:: html
   
   <pre><code class="language-latino line-numbers">/*
    The following code
    repeat the same example we saw a moment ago above
    with the same variables X and Y as variables to use
   */

   x = 5
   y = x + 2
   escribir (y)</code></pre>

----

Using comments to prevent code execution:
----------------------------------------------------------
Using comments to prevent the execution of a line of code can be very useful when we are testing our code. Adding the **#** or **//** signs in front of any line of code will make this single line invisible to the program when it is run.

In this example, the **//** sign will be used to prevent the execution of the first line of code:

.. raw:: html
   
   <pre><code class="language-latino line-numbers">//escribir ("This code will NOT run")
   escribir ("This code WILL run")</code></pre>

In this example, the execution of a code block with the multi-line comments will be prevented:

.. raw:: html
   
   <pre><code class="language-latino line-numbers">/*
   This whole block of code being a comment
   will not run when starting the program
   
   x = 5
   y = x + 2
   escribir (y)
   */</code></pre>